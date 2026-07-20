# Week 7 — Secure FastAPI Registration Endpoint

```python
@app.post("/api/users/register", status_code=201)
def register(user: RegisterRequest, session: Session = Depends(get_session)):
    if session.query(User).filter_by(email=user.email).first():
        raise HTTPException(409, "Email already registered")
    record = User(email=user.email, password_hash=bcrypt.hash(user.password))
    session.add(record); session.commit()
    return {"access_token": create_jwt(record.id), "token_type": "bearer"}
```

Validate email and password length in `RegisterRequest`; never store or return a plaintext password.

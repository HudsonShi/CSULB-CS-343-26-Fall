# Week 8 — API Validation Tests

```python
import pytest

@pytest.mark.parametrize("email", ["missing-at", "@example.com", "a@"])
def test_registration_rejects_invalid_email(client, email):
    response = client.post("/api/users/register", json={
        "name": "Ada", "email": email, "password": "safe-pass-123"
    })
    assert response.status_code == 422
```

Keep unit tests fast; reserve database and HTTP interactions for integration tests.

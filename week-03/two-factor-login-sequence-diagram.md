# Week 3 — Login with 2FA

```mermaid
sequenceDiagram
    actor User
    participant App
    participant Identity
    participant Email
    User->>App: Submit email and password
    App->>Identity: Validate password
    Identity->>Email: Send one-time password
    User->>App: Submit OTP
    App->>Identity: Verify OTP
    Identity-->>App: Issue access token
    App-->>User: Open dashboard
```

Audit the draft for expired OTPs, invalid passwords, and duplicate actors.

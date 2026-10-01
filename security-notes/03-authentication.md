# Authentication Security Basics

Authentication establishes who a user or service is. Security controls should protect credentials and session establishment.

## Baseline controls
- Use established password-hashing algorithms rather than custom cryptography.
- Apply rate limiting and abuse detection to login and recovery endpoints.
- Prefer phishing-resistant MFA where available.
- Keep session identifiers unpredictable and short-lived when risk is high.
- Rotate or invalidate sessions after credential changes and sensitive events.
- Avoid revealing whether a username or account exists.

Review login, logout, password reset, MFA enrollment, MFA recovery, remember-me, and session expiration paths independently.

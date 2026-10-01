# Security Logging and Monitoring

Good security logging helps detect abuse, investigate incidents, and validate controls.

## What to capture
Record security-relevant events such as authentication failures, privilege changes, sensitive configuration changes, suspicious input handling failures, and important administrative actions. Include a timestamp, actor or service identity, action, and outcome where appropriate.

## What not to capture
Do not log passwords, session tokens, private keys, authorization headers, or unnecessary personal data. Protect logs from unauthorized modification and restrict access.

Define alerts for repeated authentication failures, unusual privilege changes, unexpected access patterns, and integrity failures.

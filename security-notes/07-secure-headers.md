# Secure HTTP Response Headers

HTTP response headers can add browser-side security controls and reduce common web attack impact.

## Useful controls
- Content-Security-Policy can constrain executable content and resource origins.
- Strict-Transport-Security can tell browsers to prefer HTTPS after a secure connection.
- X-Content-Type-Options can reduce MIME-sniffing behavior.
- Referrer-Policy controls how much referrer information is sent.
- Permissions-Policy can limit selected browser capabilities.
- Frame-ancestors in CSP can control framing and reduce clickjacking risk.

Choose policies based on the application and test them in staging before enforcement.

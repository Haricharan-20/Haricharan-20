# TLS and Transport Security

Transport security protects data in transit between clients, services, and administrative systems.

## Baseline
- Redirect HTTP to HTTPS where appropriate.
- Use certificates from trusted authorities and monitor expiration.
- Disable obsolete protocol versions and weak cryptographic options according to current platform guidance.
- Protect private keys and restrict access to them.
- Validate certificates on clients instead of disabling verification to work around errors.
- Review internal service-to-service connections as well as public endpoints.

Automate certificate-expiry monitoring and renewal. TLS protects the channel but does not replace authentication, authorization, or secure application logic.

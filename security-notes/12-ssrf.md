# SSRF Defensive Design

Server-side request forgery can occur when an application fetches a URL influenced by an untrusted user.

## Mitigations
- Use allowlisted destinations for integrations whenever possible.
- Parse and validate URLs with a trusted library.
- Restrict outbound network access from workloads.
- Block access to sensitive internal administration paths through network policy.
- Re-check resolved destinations to reduce DNS-based bypasses.
- Do not follow arbitrary redirects without policy checks.

Combine application validation with network-level egress controls so unsafe destinations remain unreachable if application logic contains an error.

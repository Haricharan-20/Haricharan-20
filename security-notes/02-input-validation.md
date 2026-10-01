# Secure Input Validation

Input validation should happen at trust boundaries before data reaches sensitive operations.

## Defensive rules
- Prefer allowlists when the valid input space is known.
- Enforce type, length, range, and encoding constraints.
- Canonicalize data before security-sensitive comparisons.
- Reject malformed input rather than silently fixing dangerous values.
- Validate on the server even when a client also validates.
- Keep validation separate from output encoding.

Add tests for null values, excessive lengths, unexpected encodings, duplicate parameters, and boundary values.

Validation reduces attack surface, but it does not replace parameterized queries, authorization, or context-appropriate output encoding.

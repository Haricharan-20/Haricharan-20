# Authorization and Access Control

Authorization decides what an authenticated identity may access.

## Secure design
- Enforce authorization on the server for every protected action.
- Prefer deny-by-default policies.
- Check access to the specific object and operation, not only the UI route.
- Centralize policy logic where practical to reduce inconsistent checks.
- Avoid trusting user-supplied role, owner, tenant, or permission fields.

Test allowed access, denied access, cross-user access, cross-tenant access, expired sessions, and privilege changes. Hidden UI controls are not authorization.

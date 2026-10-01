# Threat Modeling for Security Projects

A practical threat model starts by defining assets, trust boundaries, entry points, and realistic adversaries.

## Core workflow
1. Identify sensitive assets: credentials, session tokens, personal data, cryptographic keys, and administrative functions.
2. Map trust boundaries between users, browsers, APIs, databases, workers, third-party services, and internal systems.
3. List entry points such as HTTP endpoints, file uploads, CLI arguments, environment variables, webhooks, and authentication flows.
4. Describe threats using a framework such as STRIDE.
5. Assign mitigations to concrete components and verify them with tests.

## Review questions
- What can an untrusted user control?
- Where is authorization enforced?
- What data crosses a trust boundary?
- What happens when a dependency or external service is unavailable?

Update the threat model whenever architecture or trust assumptions change.

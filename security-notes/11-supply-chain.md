# Software Supply Chain Security

A secure software supply chain protects source, dependencies, builds, artifacts, and deployment credentials.

## Controls
- Require code review for sensitive changes.
- Protect the default branch.
- Minimize CI token permissions.
- Separate build and release privileges.
- Prefer trusted and version-pinned build actions.
- Generate provenance or attestations when supported.
- Verify release artifacts before distribution.

Treat CI configuration as production security-sensitive code.

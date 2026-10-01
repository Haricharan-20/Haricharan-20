# Secrets Management

API keys, signing keys, database credentials, and tokens should be treated as high-value secrets.

## Secure handling
- Keep secrets outside source control.
- Prefer environment-specific secret stores or managed secret managers.
- Limit each secret to the minimum permissions and scope.
- Rotate compromised or long-lived credentials.
- Prevent secrets from appearing in logs, crash reports, and build artifacts.
- Scan commits and CI artifacts for accidental exposure.

Do not treat .gitignore as a security boundary. Once a secret is committed, assume it may have been copied and rotate it even after the file is deleted from the latest revision.

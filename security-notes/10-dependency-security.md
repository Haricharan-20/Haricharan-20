# Dependency Security

Third-party packages can become part of your attack surface.

## Defensive workflow
- Pin or constrain versions appropriately for the project.
- Review security advisories and update vulnerable dependencies.
- Remove unused packages.
- Generate a software bill of materials where practical.
- Verify provenance and integrity for critical build inputs.
- Test upgrades in CI before deployment.

Automated dependency alerts are helpful, but teams should still understand which production components depend on each package.

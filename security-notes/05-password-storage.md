# Password Storage

Passwords should be stored using a password-specific, adaptive one-way hash.

## Recommended practice
Use a modern password hashing function such as Argon2id, bcrypt, or scrypt with parameters appropriate for the deployment. Store the verifier and required salt or algorithm metadata; never store plaintext passwords or reversible encrypted copies for ordinary login verification.

## Additional controls
- Use a unique salt per password.
- Protect reset tokens and make them single-use and time-limited.
- Avoid logging credentials, reset links, or authorization headers.
- Consider breached-password screening during password creation.
- Rehash old passwords when stronger parameters become available.

Protect the reset path, session lifecycle, MFA recovery, and administrative access as well.

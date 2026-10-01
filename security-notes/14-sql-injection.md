# SQL Injection Prevention

SQL injection happens when untrusted input changes the structure of a database query.

## Primary defense
Use parameterized queries or prepared statements supplied by the database driver or ORM. Keep data values separate from SQL syntax.

## Additional controls
- Avoid building SQL with string concatenation.
- Validate identifiers and sort fields against explicit allowlists when dynamic SQL is unavoidable.
- Use least-privilege database accounts.
- Restrict database network exposure.
- Avoid returning raw database errors to end users.
- Add tests for authorization and query behavior at API boundaries.

Parameterized queries are the primary control; escaping strings manually is not a reliable substitute for them.

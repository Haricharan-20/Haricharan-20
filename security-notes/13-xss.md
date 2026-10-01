# Cross-Site Scripting (XSS) Prevention

XSS occurs when untrusted data is interpreted as executable content in a browser context.

## Defensive layers
- Prefer framework-provided escaping and safe templating.
- Apply context-appropriate output encoding.
- Avoid dangerous HTML or script sinks for untrusted data.
- Sanitize rich HTML with a well-maintained sanitizer when HTML input is genuinely required.
- Deploy a carefully tested Content-Security-Policy as an additional layer.
- Set session cookies with appropriate security attributes.

Do not rely on input filtering alone. Preserve the distinction between data and executable code at render time.

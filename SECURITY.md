# Security Policy

## Reporting a vulnerability

**Do not open a public issue.** Report privately by either:

- **GitHub:** the repository's **Security → Report a vulnerability** tab (private advisory), or
- **Email:** nguyen_danh_2002@outlook.com, subject `[SECURITY] <repository>`.

Include the affected repository and version/commit, reproduction steps, impact, and any suggested
fix.

| Step | Target |
|------|--------|
| Acknowledgement | 72 hours |
| Initial assessment | 7 days |
| Fix for critical / high issues | 30 days |
| Public disclosure | After a fix is released, coordinated with the reporter |

## Supported versions

Only the latest release (or the default branch, where there are no releases) receives security
fixes.

## Safety-critical systems

Firmware and control software here drive motors and aircraft. Issues that can cause uncommanded
actuation, bypass a failsafe or watchdog, or break a TrustZone boundary are treated as
**critical**, regardless of exploitability.

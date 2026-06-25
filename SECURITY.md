# Security Policy

## Reporting a vulnerability

Report security issues **privately** by email to `hello@septagon.dev`.

**Do not** open a public GitHub issue for security vulnerabilities.

### What to include

- Affected repository and version (tag, branch, or commit)
- Impact summary
- Reproduction steps
- Proposed mitigation (if known)

We aim to acknowledge reports within 48 hours and issue a fix in coordination with the reporter.

## Scope

The following repositories are within scope:

- All `github.com/septagon-oss/*` Go modules
- Published releases and tags

## Supported versions

Security fixes are released as patch or minor version bumps as soon as
possible. Because PlatformKit is pre-1.0 (v0.x), breaking security fixes
may increment the minor version. Always use the latest tag.

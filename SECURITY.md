# Security Policy

ReplicaMD runs AI coding agents with real shell access on your machine, so we
take security reports seriously. Thank you for helping keep users safe.

## Reporting a vulnerability

**Please do not open a public issue for security vulnerabilities.**

Report privately through either channel:

- **GitHub** - [open a private security advisory](https://github.com/Ardjun6/Replica.MD-releases/security/advisories/new)
  (Security → Report a vulnerability). This is the preferred method.
- **Email** - `ardjundebitewarie@gmail.com` with the subject line prefixed
  `[SECURITY]`.

Please include, as far as you can:

- the version (Help → About, or the release tag) and your OS;
- a description of the issue and its impact;
- reproduction steps or a proof of concept;
- any relevant logs, keeping secrets redacted.

## What to expect

- We aim to acknowledge a report within a few business days.
- We will confirm the issue, keep you updated on remediation, and credit you in
  the release notes once a fix ships - unless you prefer to remain anonymous.
- Please give us a reasonable window to release a fix before any public
  disclosure (coordinated disclosure).

## Supported versions

Security fixes are made against the latest release. Older releases are not
maintained; please update before reporting.

## Scope and design notes

A few things that are working as intended rather than vulnerabilities:

- **Agents run with elevated permissions by design.** Terminal presets launch
  coding agents in an unattended mode (e.g. `--dangerously-skip-permissions`)
  so they can work without prompting. This is a deliberate, user-initiated
  trade-off; run ReplicaMD only on repositories and with agents you trust.
- **Credentials are delegated, not owned.** Agent logins go through each tool's
  own CLI (e.g. `gh auth login`) and provider API keys are stored in the OS
  keyring via Electron `safeStorage`. ReplicaMD does not transmit your keys to
  any ReplicaMD-operated service.
- **Telemetry is opt-in and off by default.** No usage analytics are sent unless
  you explicitly enable them in Settings.

Reports that amount to "an agent given shell access can run shell commands" are
out of scope. Reports about credential leakage, sandbox/worktree escape,
privilege escalation, or code execution through untrusted input are in scope and
very welcome.

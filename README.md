# ReplicaMD

ReplicaMD is a local-first desktop workspace for persistent AI coding agents,
project terminals, and the built-in Knowledge app. This repository contains
public installers, update manifests, documentation and the beta issue tracker.
The source repository is private.

[Product website](https://replicamd.ardjun.chatgpt.site) · [Download the latest release](https://github.com/Ardjun6/Replica.MD-releases/releases/latest)

Windows x64 requires Git for Windows/Git Bash. Linux x64 downloads include an
AppImage, Debian package and Arch package. Choose an asset named **ReplicaMD**
or **replicamd**; older WorkFlow/ReplicaHive releases are different distributions.
macOS is not included in the current public beta.

- [Installation and first task](https://replicamd.ardjun.chatgpt.site/installation.html)
- [Privacy](https://replicamd.ardjun.chatgpt.site/privacy.html)
- [Licenses](https://replicamd.ardjun.chatgpt.site/terms.html)
- [Support and feedback](https://replicamd.ardjun.chatgpt.site/support.html)
- [Beta test session](BETA.md)
- [Report a problem](https://github.com/Ardjun6/Replica.MD-releases/issues/new/choose)

Local profiles do not require Google. Google integration is optional and its
Testing audience is limited to approved test users. Agent CLIs and provider
accounts are configured separately; their usage costs are separate.

The beta installers are unsigned. Release notes report performed checks and
remaining platform gaps. Keep tested backups of important work. Profile backups
include profile identity, layout and Logboek; project files and Knowledge vaults
need their own backups.

## Downloads and updates

Check the assets on the exact release. Verify downloads with `SHA256SUMS.txt`.
The `latest.yml` and `latest-linux.yml` assets are consumed by the updater.
Native Windows installation and update verification must be recorded separately
from a cross-compiled package or Wine module check.

## Sensitive reports

For vulnerabilities, email `ardjundebitewarie@gmail.com` with `[SECURITY]` in the
subject. Never post keys, tokens, personal calendars, or private backups in an
issue. There is no guaranteed support response time.

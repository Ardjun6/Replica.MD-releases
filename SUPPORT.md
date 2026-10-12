# ReplicaMD support

ReplicaMD is a local-first desktop application for Linux and Windows. Public beta releases may contain known limitations; release notes describe the checks performed and remaining platform gaps.

## Report a problem

Use the [ReplicaMD issue tracker](https://github.com/Ardjun6/Replica.MD-releases/issues). Include:

- ReplicaMD version and installer type (AppImage, Debian, Arch, Windows installer or ZIP).
- Operating system and architecture.
- The steps that reproduce the problem, expected result and actual result.
- Whether it happens in a fresh local profile.
- Relevant error text or a screenshot after removing private information.

Never post API keys, Google grants, authentication tokens, personal calendar events or unredacted profile/vault backups. For a security issue, follow [SECURITY.md](SECURITY.md).

## Data and recovery

Local profiles work without Google. Profile backups preserve identity, layout and Logboek records in current source; they do not contain project or Knowledge files. Use the Knowledge vault folder backup for notes, attachments and other regular files under that folder. Review its manifest exclusions and test a restore in a fresh folder. See the [administrator backup guide](admin-notes/08-data-security-and-backups.md).

## Platform limits

Windows terminal sessions require Git for Windows (Git Bash). Unsigned installers may prompt for confirmation. Linux packages use the system desktop libraries listed by the package manager. Google integration is optional and its current Testing audience is limited to configured test users.

There is no guaranteed response time or paid support entitlement. Check the [latest release notes](https://github.com/Ardjun6/Replica.MD-releases/releases/latest) before updating, and keep a tested backup of important work.

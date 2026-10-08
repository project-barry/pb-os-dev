# pb-os-dev: test builds for pb-os dev devices

> [!IMPORTANT]
> **This repository was set up with a coding agent:
> [Claude Code](https://www.anthropic.com/claude-code), running Anthropic's
> Claude Opus 5.5 (`claude-opus-5-5`).** Claude wrote this README and builds
> the packages published here; people set the goals, made the decisions and
> did the hands-on testing. See the
> [note from lavachemist](https://github.com/project-barry/pb-os#a-note-from-lavachemist-written-by-a-human)
> in pb-os. Review before you rely on it.

**Not for regular use.** These are test builds of pb-os that have not been
released. To install pb-os, use an image from
[project-barry/pb-os releases](https://github.com/project-barry/pb-os/releases);
regular updates come from
[pb-os-updates](https://github.com/project-barry/pb-os-updates).

## Who sees these

Only devices with **Dev updates** turned on: Quick Access → Decky →
**PB-OS Utils** → **Update** → **Dev updates** (or `pbosctl update-channel dev`).
They are offered whatever is newest here or in the regular releases. Every
other device ignores this repository. Turning Dev updates off never downgrades
a device; it follows the regular releases again once they are newer.

## From test to release

A test build carries the release number it would get. When it passes, the
same files (same signature) are published as a regular release in
pb-os-updates, with its images on pb-os for a feature release. A build that is
not released leaves a gap in the numbering.

Each release here has the update packages for each device, `SHA256SUMS`,
`SHA256SUMS.sig` (signed with the pb-os release key; devices check it) and
`release_notes.md`.

## Problems

Report them in [pb-os issues](https://github.com/project-barry/pb-os/issues)
and say it was a test build, with its version and your device.

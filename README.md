---
title: aida-core homebrew tap
description: Homebrew tap for aida-core projects
license: MIT
---

# aida-core/homebrew-tap

Homebrew tap for [aida-core](https://github.com/aida-core) projects.

## Available formulas

| Formula | Project | Description |
|---|---|---|
| `pacer` | [aida-core/pacer](https://github.com/aida-core/pacer) | Local rate-limiting daemon for outbound API calls — paces `git`/`gh` against per-host token buckets. |

## Install

```sh
brew tap aida-core/tap
brew install pacer
```

Or in one line:

```sh
brew install aida-core/tap/pacer
```

After install, run `pacer install` to set up the user-level service and shim symlinks, then `pacer doctor` to verify the installation.

## Formula updates

Formulas are managed automatically by each project's release pipeline. The pacer formula here is updated by goreleaser when [aida-core/pacer](https://github.com/aida-core/pacer) cuts a `v*` tag — see [pacer's `docs/RELEASE.md`](https://github.com/aida-core/pacer/blob/main/docs/RELEASE.md) for the maintainer-facing process.

**Do not edit `Formula/*.rb` by hand.** Manual changes will be overwritten on the next upstream release.

## Verifying installed binaries

Every pacer release artifact is cosign-signed and ships with CycloneDX + SPDX SBOMs plus SLSA build provenance. See [pacer's `docs/SUPPLY-CHAIN.md`](https://github.com/aida-core/pacer/blob/main/docs/SUPPLY-CHAIN.md) for the verification commands.

## License

MIT — see [`LICENSE`](./LICENSE). Individual formulas point at upstream projects under their own licenses (pacer: MPL-2.0).

# Changelog

All notable changes to this project are documented in this file. The format
follows [Keep a Changelog 1.1.0](https://keepachangelog.com/en/1.1.0/), and the
project follows [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

The catalog has no tagged release yet, so every change from the first commit to
`main` is under `[Unreleased]`. Commit references are short hashes on `main`.

## [Unreleased]

### Added

- Security policy in `SECURITY.md`, with the private reporting channel and the response times.
- Catalog `keepglide` with the `askaway` plugin (`3a49736`), pinned to a beta tag (`406bce4`).
- `master-jev-hook` listed in the catalog (`dc0440d`), pinned to `v1.3.0-beta.2` (`d085ea5`).

### Changed

- Plugin pins move with each new `askaway` beta, from `v0.4.0-beta.4` (`d3c8ca4`) to `v0.4.0-beta.45` (`3ec3ee5`), through 35 `chore(catalog)` pin commits.
- The README pair follows the KeepGlide README standard: banner, badges, Status, What it delivers with a plugin table, How it works, Known issues, Uninstall, Development (`claude plugin validate`) and Maintainer.
- Author credit: Sophia Phillipa (KeepGlide) is named as the catalog author (`7a0d6e4`).

### Fixed

- Removed a stray null `version` key from the `askaway` entry (`3c06cde`).

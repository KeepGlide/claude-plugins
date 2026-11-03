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

- Plugin ids renamed (DEC-W65, issue #130). `askaway` is now `askaway-user` (display name AskAway User), and `master-jev-hook` is now `askaway-model` (display name AskAway Model). The source repositories and the `plugins/askaway` path are unchanged; the MCP server is now `askaway-model`, and its tools keep their names (`request_decision`, `jev_classify`, `jev_verify`, `jev_score`, `jev_rank`). Migration: `claude plugin uninstall askaway@keepglide` and `claude plugin uninstall master-jev-hook@keepglide`, then `claude plugin install askaway-user@keepglide` and `claude plugin install askaway-model@keepglide`.
- Both plugins are pinned to `main` (`da5d746` for askaway, `b1318c3` for askaway-model) instead of the tags `v1.0.3` and `v1.3.0-beta.2`. The pins point at unreleased `main` until a release tag exists.
- The README pair links the product page on keepglide.com from the top navigation line.

- Plugin pins move with each new `askaway` beta, from `v0.4.0-beta.4` (`d3c8ca4`) to `v1.0.3`, through 47 `chore(catalog)` pin commits (`v1.0.0` was the first stable askaway).
- The README pair follows the KeepGlide README standard: banner, badges, Status, What it delivers with a plugin table, How it works, Known issues, Uninstall, Development (`claude plugin validate`) and Maintainer.
- Author credit: Sophia Phillipa (KeepGlide) is named as the catalog author (`7a0d6e4`).

### Fixed

- Removed a stray null `version` key from the `askaway` entry (`3c06cde`).

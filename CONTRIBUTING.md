# Contributing to Epix

Thank you for your interest in contributing! These guidelines apply to all repositories in the [EpixZone](https://github.com/EpixZone) organization unless a repository provides its own `CONTRIBUTING.md`.

## Ways to contribute

- **Code** — bug fixes, features, performance improvements
- **Documentation** — guides, API docs, fixing typos and outdated instructions
- **Testing** — running testnet nodes and EpixNet nodes, reporting bugs, writing tests
- **Translations** — EpixNet apps ship with multi-language support and welcome new locales
- **Ideas** — feature requests and design discussions via issues and [Discord](https://discord.gg/bF2GKHgrfv)

## Before you start

1. **Check existing issues and PRs** to avoid duplicating work.
2. **For large changes, open an issue first** to discuss the approach before investing significant time.
3. **Security vulnerabilities must not be reported in public issues** — see our [security policy](SECURITY.md).

## Pull request workflow

1. Fork the repository and create a branch from `main` (or the repo's default branch):
   ```bash
   git checkout -b feat/short-description
   ```
2. Make your changes. Match the style and conventions of the surrounding code.
3. Add or update tests where it makes sense, and make sure the existing test suite passes.
4. Keep commits focused; write clear commit messages that explain *why*, not just *what*.
5. Open a pull request against the default branch and fill out the template. Link related issues (e.g. `Closes #123`).
6. Be responsive to review feedback — maintainers may request changes before merging.

## Project-specific notes

| Project | Stack | Notes |
|---|---|---|
| [EpixChain](https://github.com/EpixZone/EpixChain) | Go (Cosmos SDK + EVM) | Main binary builds from `evmd/`; run `make test` before submitting |
| [EpixNet](https://github.com/EpixZone/EpixNet) | Rust | Build with `cargo build`; see the per-OS install docs in `docs/install/` |
| Xites (EpixTalk, EpixMail, EpixPost, …) | Plain ES6 JavaScript | No build step — files load via individual `<script>` tags and are wrapped in IIFEs |
| Smart contracts (epix-tipping, epix-airdrop, vrf-contracts) | Solidity | Include tests for any contract change |

## Code style

- **Go**: `gofmt`/`goimports`, idiomatic Cosmos SDK patterns
- **Rust**: `cargo fmt` and `cargo clippy` clean
- **JavaScript/TypeScript**: match the existing style of the repo you're working in
- **Solidity**: follow the existing patterns; prioritize clarity and safety over cleverness

## Licensing

By contributing, you agree that your contributions are licensed under the same license as the repository you contribute to.

## Questions?

Join us on [Discord](https://discord.gg/bF2GKHgrfv) — the community is happy to help you get started.

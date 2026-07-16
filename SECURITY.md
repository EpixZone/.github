# Security Policy

The Epix team takes the security of our blockchain, network stack, smart contracts, and applications seriously. We appreciate responsible disclosure of vulnerabilities.

## Reporting a vulnerability

**Please do not report security vulnerabilities through public GitHub issues, discussions, Discord, or social media.**

Instead, use one of these private channels:

1. **GitHub private vulnerability reporting** (preferred): on the affected repository, go to **Security → Report a vulnerability**. This creates a private advisory visible only to maintainers.
2. **Discord direct message**: contact a core team member privately on [Discord](https://discord.gg/bF2GKHgrfv) and ask for a secure channel — do not post details in public channels.

Please include as much of the following as you can:

- The affected repository, component, and version/commit
- A description of the vulnerability and its potential impact
- Step-by-step reproduction instructions or a proof of concept
- Any suggested mitigation or fix

## Scope

Of particular interest:

- **EpixChain** — consensus, EpixMint emission logic, precompiles, EVM/Cosmos state divergence, signature verification, IBC handling
- **EpixNet** — content signing/verification, peer protocol, Tor/I2P integration, sandbox escapes in the site wrapper
- **Smart contracts** — epix-tipping, epix-airdrop, VRF contracts
- **Wallet & identity** — epix-wallet, xID / xAuth

## What to expect

- We will acknowledge your report within **72 hours**.
- We will keep you informed as we validate and remediate the issue.
- We ask that you give us a reasonable window to ship a fix before any public disclosure.
- With your permission, we will credit you in the advisory once the fix is released.

## Supported versions

Only the latest release / default branch of each repository receives security fixes unless a repository states otherwise.

Thank you for helping keep Epix and its users safe.

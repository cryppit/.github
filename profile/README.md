# Cryppit

**Keyless, read-only tools for cross-chain money — that show their work.**

Cryppit traces where crypto actually is and who can move it, from public chain data alone. No keys, no custody,
no sign-in: paste an order or an address and read the answer, with every hop sourced to the chain or contract
that proves it.

## What we've shipped

| Tool | What it does | Where |
|---|---|---|
| **Where's My Swap** | Trace a NEAR Intents order hop by hop to its payout — where the money is now and who can move it. Payouts on 33 chains; flags order accounts locked by Intents' operators. | [Open it](https://wheres-my-swap.station-wheres-my-swap.workers.dev) |
| **Safe to Send** | Check an address before you send: see whether funds on that chain can be reached. Catches smart wallets that only exist on one chain across 20 chains, with every Abstract wallet archived before Abstract shuts down on 15 Dec. | [Open it](https://cryppit.github.io/safe-to-send/) · [repo](https://github.com/cryppit/safe-to-send) |
| **Where's My Withdrawal** | Paste a rollup withdrawal (Optimism, Base, Arbitrum, Robinhood Chain, Linea, ZKsync) and see which step is missing and who can finish it. | [Open it](https://cryppit.github.io/wheres-my-withdrawal/) |
| **Zcash Refund Helper** | Find a ZEC or BTC deposit stuck in the NEAR Omni bridge and print the bridge's own refund steps. Used on mainnet to return a stuck deposit to its owner. | [Open it](https://cryppit.github.io/zec-refund-helper/) · [repo](https://github.com/cryppit/zec-refund-helper) |
| **NU7 Readiness** | Which Zcash wallets, libraries, bridges and swaps are ready for NU7, from public evidence — re-checked hourly. | [The board](https://cryppit.github.io/nu7-readiness/) |
| **ZIP 320 TEX vectors** | Test vectors, a reference codec and an integrator checklist for Zcash TEX addresses. | [repo](https://github.com/cryppit/zcash-tex-vectors) |

## How we work

- **Read-only, always.** Our tools never hold a key or sign a transaction.
- **Every claim is sourced.** A verdict points to the block, transaction or contract it came from.
- **Open where it helps.** We file the upstream fixes we find while building — see [the maintainer's profile](https://github.com/Anirudh-712).

Hyderabad, India.

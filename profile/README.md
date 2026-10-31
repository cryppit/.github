# Cryppit

**Free tools that tell you where your crypto is, and what to do next.**

Money gets stuck between chains, bridges and apps, and support answers are slow. Cryppit's tools read the public
blockchain records and tell you, in plain words, where your money is, who can move it and the next step. They never
ask for your keys, never sign anything and need no account: you paste a transaction or an address and read the answer.

## Before you send

| Tool | Use it when | You paste, you get |
|---|---|---|
| **Safe to Send** · [open](https://cryppit.github.io/safe-to-send/) | You are about to send to an address on another chain. Some smart wallets (Abstract, Safe) exist on one chain only, and money sent to the same address elsewhere can be lost. | An address and the chain you will send on. You get *safe*, *caution* or *don't send*, checked on 20 chains, with the reason. |
| **Address check** · [open](https://wheres-my-swap.station-wheres-my-swap.workers.dev/address) | You want to be sure an address is right before sending. | Any address on the 21 chains NEAR Intents pays out to. You get which chain it belongs to and whether it has a typo; for Zcash, whether a transparent-only or a shielded wallet can pay it. Checked in your browser, nothing is sent anywhere. |

## Your money is stuck on the way

| Tool | Use it when | You paste, you get |
|---|---|---|
| **Where's My Swap** · [open](https://wheres-my-swap.station-wheres-my-swap.workers.dev) | You swapped through NEAR Intents (used inside many wallets and apps) and the money has not arrived. | The transaction from your wallet. You get every step of the swap, where the money is right now, who can move it, and how to get it back if it was refunded. Payouts on 33 chains. |
| **Zcash Refund Helper** · [open](https://cryppit.github.io/zec-refund-helper/) | You sent ZEC or BTC into the NEAR Omni bridge and it never arrived. | Your deposit's transaction. You get where it stands and, if it can be refunded, every step left, what each costs and the only address it can go back to (shielded when your address can take it). Used on mainnet to send a stuck 0.1 BTC home. |
| **Where's My Withdrawal** · [open](https://cryppit.github.io/wheres-my-withdrawal/) | You are moving ETH from a rollup (13 chains, including Optimism, Base, Arbitrum, Blast, Robinhood Chain, Linea and ZKsync) back to Ethereum and it seems stuck. | The withdrawal transaction. You get which step is missing (prove, wait, claim) and who can do it; often anyone can, and the money still goes only to you. |
| **Shield Receipt** · [open](https://cryppit.github.io/shield-receipt/) | You withdrew ZEC from an exchange to a shielded or unified address and want to know whether it arrived shielded. Many exchanges pay the transparent part instead. | The withdrawal's transaction and the address you gave (it never leaves the page). You get where it landed: your transparent address, where anyone can see the amount, or a shielded pool (Sapling, Orchard or Ironwood). |

## In a chat

**[@WheresMySwap_Bot](https://t.me/WheresMySwap_Bot) on Telegram** answers the same questions without opening a page:
`/check` a swap, `/refund` a stuck Bitcoin or Zcash deposit, `/address` before you send. Every answer comes with a
picture you can forward to anyone.

## For wallet and exchange support teams

**[Flight Recorder](https://wheres-my-swap.station-wheres-my-swap.workers.dev/recorder)** watches the NEAR Intents
orders your users ask about and tells your team the moment one changes: it stalls, is refunded, settles late or its
payout never lands. Each order comes with the timeline and the evidence links, so your team can answer before the user
writes in. Free during the pilot; ask at [@CryppitHQ on X](https://x.com/CryppitHQ).

## Watching a network

**[NU7 Readiness](https://cryppit.github.io/nu7-readiness/)**: which Zcash wallets, libraries, bridges and swaps are
ready for the NU7 upgrade, from public evidence, re-checked every hour.

## For developers

- **[ZIP 320 TEX vectors](https://github.com/cryppit/zcash-tex-vectors)**: test vectors, a reference codec and a
  checklist for wallets adding Zcash TEX addresses.
- Every tool's code is open: [Where's My Swap](https://github.com/cryppit/wheres-my-swap),
  [Zcash Refund Helper](https://github.com/cryppit/zec-refund-helper),
  [Where's My Withdrawal](https://github.com/cryppit/wheres-my-withdrawal),
  [Safe to Send](https://github.com/cryppit/safe-to-send),
  [NU7 Readiness](https://github.com/cryppit/nu7-readiness),
  [Shield Receipt](https://github.com/cryppit/shield-receipt).

## How we work

- **Read-only, always.** No tool holds a key, signs a transaction or asks you to connect a wallet.
- **Every answer shows its proof.** Each result links to the transaction, block or contract it was read from.
- **Check that the site runs the public code.** Where's My Swap publishes a fingerprint of every file it serves with
  each release, and a script that compares the live site with your own build
  ([how](https://github.com/cryppit/wheres-my-swap#verify-the-copy-you-run)).

Hyderabad, India.

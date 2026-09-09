# Crumbs

Cookie Chain cApp for the Superteam bounty [Create an App on Cookie Chain](https://superteam.fun/earn/listing/create-an-app-on-cookie-chain-app/) (Global, 500 + 500 USDC).

Crumbs sends native COOK with an on-chain memo, shows Nightly wallet state, and reads activity from Cookie RPC.

## Network

| | |
| --- | --- |
| RPC | https://rpc.cookiescan.io |
| Genesis | `9wDaBRDgArEUpvhHxGguNkwozsZh4UpGZB9o2EoEcBB2` (live `getGenesisHash` 2026-09-09) |
| Explorer | https://cookiescan.io |
| Bridge | https://hyperlane.cookiescan.io |
| Nightly | https://nightly.app/ |

## What it does

- Connect **Nightly** (`window.nightly.solana`) and call `changeNetwork({ genesisHash, url })`.
- Fallback to `window.solana` if Nightly is missing (bounty still requires Nightly in the demo).
- Show address and COOK balance.
- Transfer COOK + Memo program instruction.
- Confirm the signature and link the explorer.
- Dashboard: slot, epoch, RPC ping.
- Activity: last signatures for the connected address.

## Run locally

Open `index.html` in a browser (or any static server). Nightly only injects on http/https origins, not always on `file://`.

```
npx --yes serve crumbs
```

## Deploy (needed for the bounty)

1. Push this folder to a public GitHub repo.
2. Enable GitHub Pages on `crumbs/` or the repo root if you copy `index.html` there.
3. Live URL + repo URL + (optional) tx signature go into Superteam.
4. X thread: see `X_THREAD.md`. Share the thread in https://t.me/TheCookieNetChain

## Bridge

Get COOK on Solana, then bridge at https://hyperlane.cookiescan.io before sending crumbs.

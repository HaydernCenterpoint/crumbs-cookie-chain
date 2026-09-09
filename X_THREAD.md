# X thread for Cookie Chain cApp (after GitHub Pages is live)

Replace LIVE_URL and REPO_URL.

1/ Crumbs is a Cookie Chain cApp: connect Nightly, switch to rpc.cookiescan.io, send COOK with an on-chain memo, watch the signature land.

LIVE_URL

2/ Nightly is first-class. The app calls changeNetwork with Cookie genesis `9wDaBRDgArEUpvhHxGguNkwozsZh4UpGZB9o2EoEcBB2` plus the community RPC, then signAndSendTransaction.

Wallet: https://nightly.app/

3/ How to use it
- Install Nightly
- Bridge COOK: https://hyperlane.cookiescan.io
- Connect → paste a recipient → add a memo → sign
- Explorer: https://cookiescan.io

4/ Oven stats (slot/epoch/ping) and recent signatures are read live from Cookie RPC. No fake indexer.

Repo: REPO_URL
Docs: https://docs.cookiechain.wtf/getting-started
@TheCookieChain

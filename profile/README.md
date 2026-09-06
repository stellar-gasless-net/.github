Stellar Gasless Network
Gasless meta-transaction infrastructure for Soroban: a dApp sponsors a user's transaction fee via a real FeeBumpTransaction, so the user never needs to hold XLM to interact with it.

Projects
Repo	What it is	Live Demo
soroban-gasless-contracts	On-chain WASM contracts: trusted forwarder (with atomic batch execution), voucher/token paymasters, and a passkey-secured smart-account wallet with per-session spend caps.	— (see deployments/testnet.json + stellar.expert)
stellar-gasless-relayer	TypeScript backend that wraps signed inner transactions into real FeeBumpTransactions, with real Soroban RPC preflight simulation and a rotating sponsor-keypair pool.	— (backend service; see the dashboard below for its UI)
stellar-gasless-sdk	TypeScript client SDK: WebAuthn passkey signing, Freighter/xBull wallet adapters, and a GaslessClient that talks to the relayer.	— (library)
gasless-relayer-dashboard	Admin console preview — clearly marks which panels are real (live relayer status, a real end-to-end gasless transaction) versus UI mockup.	gasless-relayer-dashboard.vercel.app
Every README in this suite states plainly what's live and tested versus what's a disclosed, not-yet-built limitation.

Maintainer
@larryjay007

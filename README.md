# Nadcks TX Checker 🔍

A lightweight, client-side blockchain transaction verifier built for crypto exchange support teams. Paste any transaction hash and instantly see its real status, network, amount, sender/receiver, and confirmations — no backend, no API keys.

## 🚀 Features

- Supports **11 networks**: Bitcoin, Ethereum (ERC20), BNB Smart Chain (BEP20), Tron (TRC20), Avalanche, Litecoin, Bitcoin Cash, Dogecoin, XRP Ledger, Solana, Cardano
- Auto-detects the correct network when a coin has multiple (e.g. USDT on TRON vs BSC)
- Flags a mismatch between the coin the user claims and the coin actually found on-chain
- Shows status (success/failed/pending), confirmations, block number, fee, timestamp, and a direct explorer link
- 100% client-side — queries public RPCs/explorers (publicnode, mempool.space, TronGrid, xrplcluster, Koios, Blockchair) directly from the browser
- Dark mode support, RTL/Persian UI
- No dependencies, single HTML file

## 🛠 Tech

Vanilla JavaScript, no frameworks. Uses `BigInt` throughout for exact amount calculations (no floating-point rounding errors). Direct `eth_call`/JSON-RPC calls for EVM chains, REST APIs for the rest.

## 📦 Usage

Just open `index.html` in any browser. No build step, no install.

## ⚠️ Disclaimer

Reads only public, on-chain data. No private keys, credentials, or exchange-internal data are involved or required.

---

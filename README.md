# 🎲 Solana Lottery Bot

A decentralized lottery and raffle platform built on **Solana**, integrating directly with **Telegram** for seamless participation.  
Players can join pools using any SPL token (including memecoins) and compete for on-chain rewards with **provably fair randomness**.

---

## 🚀 Features

- **Smart-contract powered pools** — fully automated creation, joining, and payout.
- **Fair randomness** — integrated with Switchboard or similar randomness oracles.
- **Multi-token support** — compatible with memecoins, community tokens, and SPL assets.
- **Deflationary mechanism** — 3.5 % of every pool is burned, reducing token supply.
- **Referral system (coming soon)** — earn rewards when friends you invite participate.
- **Developer donations** — allow creators or whales to boost prize pools transparently.
- **Telegram integration** — play, donate, and view results without leaving the app.

---

## 💡 How It Works

1. A user creates a pool (lottery) and defines:
   - token to use  
   - entry amount  
   - number of players  
   - duration (e.g. 15 minutes)

2. Others join the pool until it’s full.  
3. When the pool closes:
   - 90 % → winner  
   - 5 % → developer fee  
   - 3.5 % → burn  
   - 1.5 % → treasury wallet (for referrals and community rewards)

4. The winner is chosen **on-chain**, verifiably and transparently.

---

## 🧱 Tech Stack

- **Solana Program Library (Rust)**
- **Anchor Framework**
- **Switchboard / Randomness Oracle**
- **Telegram Bot API (Python / Node.js)**
- **TypeScript client for Solana transactions**

---

## 🧩 Roadmap

- [x] Smart contract core  
- [x] Pool creation / joining / cancel logic  
- [x] Randomness & payout  
- [ ] Referral system  
- [ ] Frontend / dashboard  
- [ ] Public testnet launch  
- [ ] Mainnet deployment  

---

## 👨‍💻 Author

EUGENIU — Web3 Developer  
X: https://x.com/missoutl


---

## 📜 License

MIT License – feel free to use, modify, and contribute.

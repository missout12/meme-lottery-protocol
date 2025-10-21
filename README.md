# 🎲 MissOut Lottery Bot

A **decentralized lottery and raffle platform** built on **Solana**, fully integrated with **Telegram** for seamless participation.  
Players can join pools using any SPL token (including memecoins) and compete for on-chain rewards with **provably fair randomness** — all without leaving Telegram.

---

## 🚀 Features

- ⚙️ **Smart-contract powered pools** — fully automated creation, joining, locking, and payout.  
- 🎲 **Provably fair randomness** — powered by [Switchboard](https://switchboard.xyz) or similar randomness oracles.  
- 💰 **Multi-token support** — works with memecoins, community tokens, and any SPL asset.  
- 🔥 **Deflationary mechanism** — 3.5 % of every pool is burned, reducing token supply and increasing scarcity.  
- 🫂 **Referral system** *(coming soon)* — earn rewards when friends you invite participate.  
- 💎 **Developer donations** — allow creators or whales to boost prize pools transparently.  
- 📱 **Telegram integration** — create, join, donate, and view results without leaving the app.

---

## 💡 How It Works

1. A user creates a **lottery pool** and defines:
   - SPL token to use  
   - Entry amount  
   - Number of players  
   - Pool duration (e.g. 15 minutes)

2. Participants join until the pool is full.  
3. Once full, the pool **locks** and requests verifiable randomness from the oracle.  
4. The winner is selected **on-chain** and payouts are distributed automatically:

| Distribution | Percentage |
|-------------|------------|
| 🏆 Winner | 90 % |
| 👨‍💻 Developer fee | 5 % |
| 🔥 Burn | 3.5 % |
| 💰 Treasury (referrals & community) | 1.5 % |

---

## ✅ Verified Full Pool Lifecycle (On-Chain Proof)

Below is a real example of a **MissOut Lottery Pool** that completed the **entire lifecycle** on Solana Devnet — from creation and participation to randomness, winner selection, and payout.

### 📜 Pool Details

| Property | Value |
|----------|-------|
| Pool Address | [`Ci7HqRyoHeD6ytkVhW9JYVHjehKbdWx8VzGYEtEewARm`](https://explorer.solana.com/address/Ci7HqRyoHeD6ytkVhW9JYVHjehKbdWx8VzGYEtEewARm?cluster=devnet) |
| Status | ✅ Ended |
| Participants | 3 |
| Winner | `3G5v375e8Ax29zXLFL2N1UA6cnCL9HV7sZUm2YLYpYof` |
| Finalization TX | [CT1NBEjiFzzjTS2ot6urvNeLdEsqZRYr...](https://explorer.solana.com/tx/CT1NBEjiFzzjTS2ot6urvNeLdEsqZRYr?cluster=devnet) |

---

### 📊 Full Cycle Breakdown

1. **Pool Created** – smart contract initialized the pool and stored all data on-chain.  
2. **Participants Joined** – 3 users joined with 10,000 tokens each.  
3. **Pool Locked** – no further joins allowed once capacity was reached.  
4. **Randomness Requested** – randomness oracle generated a verifiable value.  
5. **Winner Selected** – randomness → winner index `1` → wallet `3G5v...` selected.  
6. **Payout Distributed** – funds distributed according to configured percentages.

---

### 🔎 Program Log (excerpt)

Instruction: EndPool
Participants count: 3
Randomness value: [6, 158, 79, 203, ...]
Normalized randomness: 7204067106267497548
Computed winner_index: 1
Selected winner: 3G5v375e8Ax29zXLFL2N1UA6cnCL9HV7sZUm2YLYpYof
Distribution: winner_amount=27000000000000, dev_amount=1500000000000, treasury_amount=1500000000000
Program invoked: Token Program -> Transfer ✅



---

## 🔗 Explore on Solana Devnet

- 🌐 **Pool Account:** [View on Solana Explorer](https://explorer.solana.com/address/Ci7HqRyoHeD6ytkVhW9JYVHjehKbdWx8VzGYEtEewARm?cluster=devnet)  
- 🧾 **Final Transaction:** [View on Solana Explorer](https://explorer.solana.com/tx/CT1NBEjiFzzjTS2ot6urvNeLdEsqZRYr?cluster=devnet)

---

## 🧱 Tech Stack

- ⚙️ **Smart Contract:** Solana Program Library (Rust) + Anchor Framework  
- 🔮 **Randomness:** Switchboard Oracle  
- 🤖 **Bot Integration:** Telegram Bot API (Node.js / Python)  
- 🪙 **Client:** TypeScript SDK for Solana transactions  
- 🗄️ **Database:** Prisma + PostgreSQL  

---

## 🗺️ Roadmap

- ✅ Smart contract core  
- ✅ Pool creation / joining / cancel logic  
- ✅ Randomness & payout  
- 🚧 Referral system *(in development)*  
- 🚧 Frontend / dashboard *(in development)*  
- 🧪 Public testnet launch  
- 🌐 Mainnet deployment  

---

## 👨‍💻 Author

**Alabasta — Web3 Developer**  
- 🐦 X: [@missoutl](https://x.com/missoutl)  
- 📢 Telegram Winners Channel: [MissOut Winners](https://t.me/your_winner_channel) *(replace with your real link)*

---

## 📜 License

**MIT License** – free to use, modify, and contribute.

---

# SunChain — Decentralized Solar Energy Network on Solana

**SunChain** is a **DePIN (Decentralized Physical Infrastructure Network)** that connects community solar hubs across Africa — starting from **South Africa** — using the **Solana blockchain** for energy data transparency, payments, and community ownership.


## Project Overview

SunChain enables communities to produce, share, and sell solar energy through decentralized smart contracts.  
Each solar hub is equipped with IoT meters that record generation and usage data directly on-chain.  
Payments and revenue distribution happen via Solana stablecoin transactions, ensuring transparency and trust.



## Core Features

**On-Chain Energy Data** — Real-time tracking of energy production and consumption.  
**Decentralized Payments** — Automatic, tamper-proof settlements via Solana smart contracts.  
**Transparent Revenue Sharing** — Local operators and investors get fair and verifiable payouts.   **DePIN Model** — Combines physical infrastructure (solar) with Web3 incentives.  
**IoT + Blockchain Integration** — Secure data flow from devices to Solana ledger.

## 🧠 Why Solana

- Ultra-fast, low-cost microtransactions for daily energy use.  
- High scalability for thousands of users per community.  
- Seamless connection to DePIN and IoT networks.

## Architecture Overview

1. **IoT Layer:** Smart meters collect solar data.  
2. **Blockchain Layer:** Data is verified and stored on Solana.  
3. **Payment Layer:** Users pay for energy via stablecoins.  
4. **Frontend Dashboard:** Real-time monitoring and analytics.

## Tech Stack

- **Blockchain:** Solana  
- **Smart Contracts:** Rust / Anchor Framework  
- **Frontend:** Next.js + TypeScript  
- **IoT Layer:** ESP32 + MQTT Broker + Solana RPC integration  
- **Database (off-chain):** Supabase / IPFS (for metadata)

## Security & Audit

SunChain uses:
- Multi-signature access control  
- Verified IoT data signatures  
- Escrow contracts for payments  
A **professional security audit** is planned before the mainnet launch to ensure safety and scalability.

## Project Category

**Category:** Infrastructure / DePIN / Clean Energy

## Deployment & Usage

This section outlines how to set up and interact with the SunChain prototype using the Solana and Anchor frameworks.  
*(Note: The following commands use placeholder examples. Replace them with actual program paths and IDs once your smart contracts are ready.)*  

### Prerequisites
Before deployment, ensure you have the following installed:  
- [Solana CLI](https://docs.solana.com/cli/install-solana-cli) (v1.18 or higher)  
- [Anchor Framework](https://book.anchor-lang.com/chapter_2/installation.html)  
- Node.js (v18 or higher)  
- Yarn or npm package manager  

### 1. Clone the Repository
```bash
git clone https://github.com/<your-username>/SunChain.git
cd SunChain
```

### 2. Configure Solana Environment
```bash
solana config set --url https://api.devnet.solana.com
solana-keygen new --outfile ~/.config/solana/id.json
```

### 3. Build and Deploy Smart Contracts
```bash
anchor build
anchor deploy
```
After deployment, take note of the **Program ID** and update it in your frontend `.env` file.

### 4. Start the Frontend
```bash
cd app
yarn install
yarn dev
```
Visit `http://localhost:3000` to access the SunChain dashboard.

### 5. Testing IoT Data Flow (Placeholder Example)
```bash
curl -X POST https://api.sunchain.energy/upload -H "Content-Type: application/json" -d '{
  "hub_id": "HUB001",
  "energy_generated": 12.5,
  "energy_consumed": 9.8
}'
```
*(This simulates IoT data being pushed to the Solana program through an API endpoint.)*

## 🚀 Roadmap

| Phase | Milestone | Timeline |
|-------|------------|-----------|
| Q4 2025 | Launch IoT-enabled pilot on Solana | ✅ |
| Q1 2026 | Expand to 5 new communities | ⏳ |
| Q2 2026 | Release SunChain Africa platform | ⏳ |

## Funding & Growth Plan

- **Current Stage:** Bootstrapped  
- **Next Steps (6–12 months):**
  - Raise seed funding for hardware expansion  
  - Complete security audit  
  - Develop mobile app & community dashboard

## Team

**Founder:** Serleemer Herrun — Web3 Builder & DePIN Innovator  
**Collaborators:** IoT Engineer, Smart Contract Dev, Community Ops Lead  

## Links

- **Platform Submission:**
- Colosseum https://arena.colosseum.org/projects/explore/sunchain-1
- **GitHub Repo:** [github.com/applengw/sunchain


Vision

> “To make clean energy as open and borderless as the internet itself — powered by Solana.”

## License

This project is open-source under the **MIT License**.  
Feel free to contribute, fork, or build on top of SunChain.

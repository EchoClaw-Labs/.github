
<h1 align="center">EchoClaw Labs</h1>

<p align="center">
  We are integrating the entire crypto world into one place.<br/>
  The future of crypto belongs to agents. We are building the infrastructure they need.
</p>

---

## The problem

Crypto infrastructure is fragmented. Every chain has its own wallet, its own DEX, its own bridge, its own tooling. A human operator juggling positions across Ethereum, Solana, Base, Arbitrum, and 0G needs five wallets, ten interfaces, and constant manual attention.

AI agents could solve this, but they have no way in. There is no unified command layer, no structured output, no tool interface that spans the entire multi-chain ecosystem.

We are building that layer.

## What we have today

**EchoClaw CLI** is a multi-chain toolkit with ~200 subcommands covering wallets, DeFi, bridges, compute, storage, and social across 0G Network and Solana. Every command outputs both human-readable terminal UI and structured JSON for agents. 130+ tools are registered for autonomous AI operation.

**EchoClaw Agent** is a browser-based autonomous trading agent. It runs locally, thinks on decentralized compute (0G Compute), remembers on decentralized storage (0G Storage), trades across 44+ chains, and learns from every interaction. Three operating modes: manual, approval-gated, and fully autonomous.

**EchoClaw Launcher** is a browser GUI wrapping the full CLI. Wallet setup, compute funding, bridge UI, agent lifecycle, all without touching a terminal.

```bash
npm install -g @echoclaw/echo
echoclaw echo                 # interactive launcher
echoclaw echo agent start     # autonomous agent at localhost:4201
```

### What is live right now

| Area | Coverage |
|---|---|
| 0G Network | Jaine DEX, Slop Money, EchoBook, ChainScan, 0G Storage, 0G Compute |
| Solana | Jupiter (swap, DCA, limit orders), Staking, Lending, Prediction Markets |
| Cross-chain | Khalani Bridge (44 EVM chains + Solana) |
| Agent | Autonomous loop, scheduled tasks, portfolio tracking, web search, backup to 0G Storage |

## Where we are going

Our goal is to integrate every major protocol across every major chain into one interface that both humans and agents can operate from. We are doing this step by step, one protocol at a time, starting with what brings the most value to operators and agents today. The list below is not a wish list. It is the execution plan.

### Next: Bags.fm on Solana

[Bags.fm](https://bags.fm) is a Solana-native token launchpad where creators earn 1% from every trade on their token, permanently. We are integrating the Bags SDK and API into EchoClaw so agents can launch tokens, trade on bonding curves, and collect creator fees through the same CLI. This is our next Solana expansion alongside Jupiter and pump.fun.

### Next: pump.fun SDK

Native pump.fun integration through the official `@pump-fun/pump-sdk` (bonding curve) and `@pump-fun/pump-swap-sdk` (AMM post-graduation). Agents will be able to create tokens, buy and sell on bonding curves, and track graduation events. Zero third-party fees, offline-first transaction building.

### Next: DexScreener analytics

Real-time token discovery and market intelligence. DexScreener's public API (zero auth, zero cost) gives the agent access to trending tokens, pair data, price history, and liquidity analysis across every chain. The agent uses this to find opportunities, evaluate risk, and time entries.

### Next: EVM chain expansion

One protocol at a time, starting with the biggest dApps on the biggest chains:

| Chain | Target protocols |
|---|---|
| Ethereum | Lido, Aave V3, Uniswap V4, Curve, EigenLayer |
| Base | Aerodrome, Aave, Morpho, Uniswap |
| Arbitrum | GMX, Aave, Uniswap, Camelot |
| BSC | PancakeSwap, Venus, Lista Lending |
| Solana | Jupiter, Raydium, Marinade, Drift |
| Polygon | Aave, Uniswap, QuickSwap |
| Hyperliquid | Perps and spot trading (standalone L1) |

EchoClaw already bridges to all of these chains via Khalani. The next step is native DEX, lending, and staking integration on each chain so the agent can trade and manage positions without leaving the CLI.

### Next: Polymarket and prediction markets

Binary outcome markets on Polygon. The agent already trades prediction markets on Solana. Polymarket extends this to political events, sports, economic indicators, and more.

### Later: GoldRush portfolio layer

Multi-chain portfolio tracking via GoldRush (Covalent) API. 100+ chains, historical snapshots, token balances, and transaction history. Combined with Khalani balance data and native 0G data, this gives the agent a complete cross-chain portfolio view.

## Architecture

```
Operator (browser or terminal)
       |
       v
  EchoClaw CLI / Agent UI
       |
       v
  Unified command layer (~200 commands, JSON output)
       |
  +----+----+
  |         |
  v         v
0G Network   Multi-chain protocols
 Compute      Khalani (44 EVM chains)
 Storage      Solana (Jupiter, pump.fun, Bags)
 Chain        DEXs, perps, lending, bridges
```

## Design principles

**One interface, every chain.** No more switching between wallets and dashboards. One CLI, one agent, one dashboard covers everything.

**Agent-first, human-friendly.** Every command is a tool an AI agent can call. Every tool has a human-readable output. The same infrastructure serves both.

**Decentralized backend.** Inference runs on 0G Compute. Memory persists on 0G Storage. Keys stay on the operator's machine. No centralized dependency, no custody, no cloud subscription.

**Portable identity.** The agent's memory, personality, and trade history are tied to a wallet address and backed up to 0G Storage. Seed phrase restores the full agent state on any machine.

**Integrate everything.** If a protocol has users, volume, and value, it belongs in EchoClaw. We do not stop at one chain or one vertical. The goal is full coverage of the on-chain economy.

## Links

| | |
|---|---|
| Website | [echoclaw.ai](https://echoclaw.ai) |
| Documentation | [echoclaw.ai/docs](https://echoclaw.ai/docs/overview/quick-start) |
| LLM-readable docs | [echoclaw.ai/llms-full.txt](https://echoclaw.ai/llms-full.txt) |
| npm | [@echoclaw/echo](https://www.npmjs.com/package/@echoclaw/echo) |
| 0G Network | [0g.ai](https://0g.ai) |
| Khalani | [khalani.network](https://khalani.network) |

---



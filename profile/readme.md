<div align="center">

# VTechcom Labs — Hydra Engineering Team

**Making Hydra practical.**

We are a Vietnam-based engineering team building the developer stack for
**Hydra**, Cardano's Layer-2 — SDKs, node infrastructure, benchmarks, and real
applications running on a live head.

[![Website](https://img.shields.io/badge/vtechcom.org-0A0A0A?style=flat-square&logo=googlechrome&logoColor=white)](https://vtechcom.org)
[![Hydra SDK Docs](https://img.shields.io/badge/docs-hydrasdk.com-2563EB?style=flat-square&logo=readthedocs&logoColor=white)](https://hydrasdk.com)
[![Cardano](https://img.shields.io/badge/Cardano-Hydra%20L2-0033AD?style=flat-square&logo=cardano&logoColor=white)](https://hydra.family)
[![Catalyst](https://img.shields.io/badge/Project%20Catalyst-Fund%2014-FF5A5F?style=flat-square)](https://projectcatalyst.io/funds/14/cardano-use-cases-concepts/hydra-hub-saas-node-distribution-system-phase-1)

</div>

---

## What we build

Four layers, one goal — take a developer from "what is a Hydra Head?" to a
production application settling on L2.

```
   Apps        Hydra One  ·  games, prediction markets, perpetual DEX
   ─────────────────────────────────────────────────────────────────
   SDK         Hydra SDK  ·  wallet, tx builders, WASM, head lifecycle
   ─────────────────────────────────────────────────────────────────
   Infra       HexCore · Hydra Hub  ·  Head-as-a-Service orchestration
   ─────────────────────────────────────────────────────────────────
   Research    benchmarks · technical reports · protocol exploration
```

---

## 🧩 SDK & Developer Tooling

| Project | What it is |
|---|---|
| **[hydra-sdk](https://github.com/Vtechcom/hydra-sdk)** ⭐ | The flagship. A Turborepo monorepo of packages — `core`, `cardano-wasm`, `hydra-bridge`, `hydra-transaction`, `evaluator` — for building Cardano wallets and Hydra-enabled apps in TypeScript. |
| **[hydra-sdk-examples](https://github.com/Vtechcom/hydra-sdk-examples)** | Runnable examples: open a head, commit funds, move UTxOs in-head, close and fan out. |
| **[hexcore-cli](https://github.com/Vtechcom/hexcore-cli)** | Terminal UI for operating Hydra nodes — interactive dashboard, head creation, multi-account selection, live status. |
| **[cardano-installer](https://github.com/Vtechcom/cardano-installer)** | Rust CLI that bootstraps a Cardano node via Docker + Mithril snapshots, so you are not waiting days to sync. |

📖 Documentation → **[hydrasdk.com](https://hydrasdk.com)**

---

## 🏗️ Infrastructure — Hydra Head as a Service

Spinning up a Hydra Head by hand means node configs, keys, peers, and a synced
Cardano node. Our infrastructure stack removes all of it.

### ⚡ HexCore v2 — now in public beta

[![npm](https://img.shields.io/npm/v/@vtechcom/hexcore/beta?style=flat-square&logo=npm&label=%40vtechcom%2Fhexcore&color=CB3837)](https://www.npmjs.com/package/@vtechcom/hexcore)
[![license](https://img.shields.io/badge/license-Apache--2.0-blue?style=flat-square)](https://www.npmjs.com/package/@vtechcom/hexcore)

A full rewrite of HexCore — control plane and web UI in one command:

```bash
npm install -g @vtechcom/hexcore@beta
hexcore
```

Requires only **Node ≥ 22** and **Docker**. No MySQL, no Redis, no RabbitMQ. The
`offline` backend runs a real multi-node Hydra Head with no chain, no credentials
and no waiting — a Blockfrost project id or a synced `cardano-node` socket is
needed only when you want heads on the real chain.

| | v1 | v2 beta |
|---|---|---|
| **Repos** | 3 separate services | 1 monorepo, 1 command |
| **Keys** | You generate and POST them in | Generated server-side on head creation |
| **Storage** | MySQL + Redis, provisioned up front | Embedded SQLite in the state dir |
| **Config** | ~30 unvalidated env vars | zod-validated, works with a single key set |
| **Setup failures** | Stack traces at random later points | `pnpm doctor` checks everything up front |
| **Failed boot** | Orphaned containers left behind | Rolls back every container it created |
| **Head state** | "Is the container up?" | Real Hydra state probed over WebSocket |

> Published under the `beta` tag while we harden it toward 2.0.0 — see the
> package CHANGELOG for what is known broken.

### The wider stack

| Project | What it is |
|---|---|
| **[hydra-hexcore](https://github.com/Vtechcom/hydra-hexcore)** | NestJS backend for managing Hydra nodes — node lifecycle, multi-party heads, transaction submission, Docker orchestration, JWT auth. |
| **[hexcore-ui](https://github.com/Vtechcom/hexcore-ui)** | Nuxt 3 web console for setting up nodes, monitoring head state, and transacting inside a head. |
| **[hydra-hexcore-design-docs](https://github.com/Vtechcom/hydra-hexcore-design-docs)** | Design document for automated deployment & management of multi-party Hydra setups. |
| **[hydra-hub-design-docs](https://github.com/Vtechcom/hydra-hub-design-docs)** | Architecture and product docs for Hydra Hub. |
| **[hydra-hub-fund14-proposal](https://github.com/Vtechcom/hydra-hub-fund14-proposal)** | Project Catalyst **Fund 14** milestone reports & completion evidence (M1–M3), including the payment-subscription contract. |

> 🔒 In active development, not yet public: `hydra-hub` (consumer portal +
> admin dashboard), `hydra-hub-backoffice`,
> `hydra-db-indexer` (head explorer & indexer), `hydra-fast-deposit-system`,
> and `deposit-batcher-validator` (on-chain deposit batching in Aiken).

---

## 🌐 Hydra One — the network and what runs on it

Hydra One is our applied layer: a live Hydra network with real applications on
top, proving that L2 is not just a whitepaper claim. Sub-second, near-free
transactions change what a Cardano app can be — so we build the apps that need
them.

| Application | What it is |
|---|---|
| **[hydra-one-docs](https://github.com/Vtechcom/hydra-one-docs)** | Integration patterns and guidelines for building on Hydra One. |
| **[hydra-network-docs](https://github.com/Vtechcom/hydra-network-docs)** | Public network documentation site. |
| **[hydra-htlc-demo](https://github.com/Vtechcom/hydra-htlc-demo)** | Full HTLC (Hash Time Locked Contract) demo with infra + client UI — presented to, and praised by, the Hydra Core Team at a Monthly Review. |
| **[aiken-htlc-contract](https://github.com/Vtechcom/aiken-htlc-contract)** | The Aiken validator behind it: hash-locked, time-locked conditional payments. |

> 🔒 Building now: **Hydra Perp** — a perpetual futures DEX on L2 (`hydra-perp`,
> `hydra-perps`) — plus the Hydra One client (`hydraone-web-client`), an on-chain
> **governance prediction market** (`hydra-gov-prediction`), and a growing arcade of
> skill-based L2 games: `hydra-graveyard`, `hydra-mines`, `hydra-fly`,
> `hydra-knight`, `hydra-gacha`, `hydra-rivercross`, `hydra-fight-dual`,
> plus poker, roulette and RPS prototypes.

---

## 🔬 Research & Benchmarks

| Project | What it is |
|---|---|
| **[hydra-benchmark](https://github.com/Vtechcom/hydra-benchmark)** | An extensible load/latency harness for a **live** `hydra-node`. Fires pre-signed txs at a target TPS, correlates each with `TxValid` and `SnapshotConfirmed`, and reports P50/P95/P99 plus three honest throughputs — offered, validated, confirmed. |
| **[hydra-sdk-technical-reports](https://github.com/Vtechcom/hydra-sdk-technical-reports)** | R&D logs and architectural decisions — polyfill incompatibilities with `@cardano-sdk`/`meshjs`, the rationale for going WASM-first, and other engineering post-mortems. |
| **[eutxo-l2-interop](https://github.com/Vtechcom/eutxo-l2-interop)** | Our working copy of the cardano-scaling EUTxO-L2 interoperability report — connecting Hydra with other L2s. |

**A result we are proud of.** Using `hydra-benchmark`, we measured what a Plutus
script transaction actually costs inside a head across three `hydra-node`
releases, against a script-free control:

| hydra-node | PlutusV3 script spend | no-script control | script penalty |
|---|---:|---:|---:|
| 2.0.0 | 85.8 TPS · 185 ms | 115.2 TPS · 137 ms | −25.5% |
| 2.2.0 | 101.8 TPS · 149 ms | 118.7 TPS · 132 ms | −14.3% |
| 2.3.0 | 106.2 TPS · 147 ms | 119.9 TPS · 131 ms | −11.4% |

The cost of being a script transaction fell by more than half — and the numbers
for [PR #2717](https://github.com/cardano-scaling/hydra/pull/2717) had never been
published anywhere, because upstream's `bench-e2e` sends plain ADA payments and
has no script to skip. Method, sign-flip permutation tests, DiD, and caveats are
all in the repo.

---

## 🧰 Tech Stack

**Languages** TypeScript · Rust · Haskell · Aiken · Gleam
**Frontend** Vue · Nuxt · Next.js · Tailwind · shadcn · Element Plus
**Backend** Node.js · NestJS · MySQL · Redis
**Cardano** Hydra Node · Ogmios · Mithril · Cardano Node · cardano-wasm
**Ops** Docker · Nix · Turborepo · Google Cloud

---

## 🎯 Where this is going

- **SDK** — the shortest path from `npm install` to a working head
- **Infrastructure** — Hydra Heads you rent, not ones you operate
- **Applications** — Hydra One as a live network with users, not a testnet
- **Research** — measurements and specs published openly, for everyone

We believe Hydra is a key component of Cardano's scalable future — fast, secure,
and trustless. The gap between that promise and shipped software is exactly the
work we do.

---

<div align="center">

**Vtechcom** · Vietnam

🌐 [vtechcom.org](https://vtechcom.org) &nbsp;·&nbsp; ✉️ [info@vtechcom.org](mailto:info@vtechcom.org) &nbsp;·&nbsp; 📖 [hydrasdk.com](https://hydrasdk.com)

*Open to collaboration with teams building on Cardano L2.*

</div>

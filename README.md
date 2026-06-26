<h1 align="center">Somil Jha</h1>

<p align="center">
  Systems builder. I write Rust, Python, and TypeScript — and I ship things that work.
</p>

<p align="center">
  <a href="mailto:somilwork77@gmail.com">somilwork77@gmail.com</a> ·
  <a href="https://linkedin.com/in/somil-jha">LinkedIn</a> ·
  <a href="https://instagram.com/somil_jha">Instagram</a>
</p>

---

## What I've shipped

### [Needle](https://github.com/somil71/NEEDLE) — Local-first code search engine
Built entirely in Rust from scratch. Hybrid BM25 + HNSW vector search, hand-rolled (no Qdrant, no Tantivy). Tree-sitter AST chunking across 8 languages, live D3 call graph with community detection, MCP server with 11 tools. Ships as a native Tauri desktop app, VS Code extension, CLI, and cloud deployment with GitHub OAuth.

`Rust` `Axum` `Tauri` `Tree-sitter` `HNSW` `BM25` `MCP`

---

### GenMol — AI Molecular Generation Platform
Full replication of *Lee et al. 2025 (arXiv:2501.06158)* — a Masked Diffusion Language Model over SMILES sequences with transformer-encoder denoiser, monotonic noise schedule, and iterative demasking inference. Includes a 3-layer hallucination guard (RDKit + perplexity + sliding window) with automatic checkpoint rollback, and a nightly self-improvement loop that retrains on high-quality production molecules.

Deployed as a microservices stack: React + Firebase Auth frontend, Node.js/Express gateway, Flask/PyTorch ML service, Supabase (PostgreSQL) data layer, Kubernetes HPA for auto-scaling.

`PyTorch` `Flask` `React` `Kubernetes` `Supabase` `RDKit` `GitHub Actions`

---

### FairPay — Decentralized Freelancer Escrow Protocol
Production-grade multi-milestone escrow on EVM (Sepolia). Funds lock at contract creation; milestones release via signatures, GitHub commit hashes, or IPFS CIDs — with automatic 48-hour default release if the client goes silent. Partial disputes let clients contest exactly the portion they disagree with. Soulbound reputation NFTs on completion; stake-based arbitration to punish bad-faith disputes.

`Solidity` `Next.js` `wagmi` `Prisma` `Neon Postgres` `BullMQ` `Docker` `Kubernetes`

---

### Job-Search Multi-Agent System
14-agent autonomous pipeline: discovers jobs across 15+ boards, scores fit against your resume, tailors the resume (A3) and validates it (A4) in a bounded feedback loop, generates a per-job apply kit, monitors your Gmail inbox for replies, classifies emails (rejection / interview / assessment / offer), schedules .ics calendar invites, tracks assessment deadlines, sends follow-ups after 3-4 days of silence, and produces weekly diagnostics reports. Claude optional; runs fully offline by default.

`Python` `FastAPI` `Playwright` `Gmail API` `SQLite` `Claude API`

---

### BSES Delhi AI Chatbot — Multilingual Electricity Service Assistant
Production-ready multi-tenant chatbot replacing a Yellow.ai subscription. A scikit-learn TF-IDF + LinearSVC classifier trained on ~36,000 labelled examples handles English, Hindi (Devanagari), and Hinglish (Latin-script) in a single model — ~1ms inference, no GPU. Three routing layers: L1 (BSES API calls), L2 (static knowledge base), L3 (Groq Llama 3.1 synthesis). Gemini Vision reads uploaded bill photos and extracts structured data. Redis caching, JWT multi-tenant sessions, per-site rate limiting. 387 tests, all passing.

`FastAPI` `scikit-learn` `Redis` `SQLite` `Groq` `Gemini` `Docker`

---

### Decision Intelligence Platform
End-to-end decision capture and drift monitoring. Slack-style chat UI where teams log decisions; a FastAPI AI microservice (GPT-4o-mini) extracts structured data and auto-generates tasks. A cron job re-evaluates decisions for drift and flags at-risk items. Circuit-breaker + retry logic throughout.

`React` `Express` `FastAPI` `MongoDB` `Redis` `Docker`

---

### FITBOARD — Shoppable Editorial Lookbook
Dark-luxury fashion platform where every outfit is a clickable product map. Admins pin individual garments on photos with exact pixel coordinates; each pin links to a tracked affiliate redirect. Infinite-scroll masonry feed, Framer Motion spring-physics pin reveals, SVG connector lines from cards to hotspots, Supabase RLS, Upstash Redis rate-limiting on click events.

`Next.js` `Supabase` `Framer Motion` `Zustand` `React Query` `TanStack`

---

### AI Consistency Auditor
Rule-based data auditing system — upload two JSON snapshots, define rules (NON_DECREASING, IMMUTABLE, NON_NULL), run an audit to detect violations with severity classification and plain-English explanations. No ML — deterministic rule engine, full audit trail, Docker deployment.

`FastAPI` `React` `MongoDB` `Docker`

---

## Stack

### Languages
![Rust](https://img.shields.io/badge/Rust-000000?style=for-the-badge&logo=rust)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Solidity](https://img.shields.io/badge/Solidity-363636?style=for-the-badge&logo=solidity&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=cplusplus&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)

### Frontend
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=next.js)
![Tailwind](https://img.shields.io/badge/Tailwind-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)

### Backend & Systems
![Axum](https://img.shields.io/badge/Axum-000000?style=for-the-badge&logo=rust)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=for-the-badge&logo=express)

### AI / ML
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)

### Infrastructure
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonaws&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)

---

## Stats

<p align="center">
  <img height="180em" src="https://github-readme-stats.vercel.app/api?username=somil71&show_icons=true&theme=tokyonight"/>
  <img height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=somil71&layout=compact&theme=tokyonight"/>
</p>

<p align="center">
  <img src="https://streak-stats.demolab.com?user=somil71&theme=tokyonight"/>
</p>

---

<p align="center">Open to client work · <a href="mailto:somilwork77@gmail.com">somilwork77@gmail.com</a></p>

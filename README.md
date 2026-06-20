<h1 align="center">Hey, I'm Sarthak 👋</h1>

<p align="center">
  Full Stack Developer · On-device AI/ML · Building things that actually ship
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/sarthak-jaiswal-9b1a17279/">LinkedIn</a> ·
  <a href="mailto:sarthakjazz8@gmail.com">Email</a>
</p>

---

## What I'm currently doing

Building the Android + ML pipeline at **[Aurviz](https://aurviz.com)** — an AI glasses startup incubated at IIT Delhi.

The pipeline chains: **on-device ASR → TFLite intent classification → slot extraction → BLE photo transfer → Gemini Vision response**

Cut end-to-end latency from **10s → under 4s**.

---

## Projects

### 🔴 [Down Detector](https://github.com/Sarthak-Jaiswal4/Down-Detector) — Uptime Monitoring Platform
Production uptime monitor modelled after Uptime Robot, built from scratch.
- HTTP/TCP checks, email alerts (downtime, recovery, SSL expiry), public status pages, maintenance windows
- 4 BullMQ workers coordinated via Redis pub/sub — result batching, retries, down-retry loop, daily SSL checks
- Per-monitor Socket.IO rooms stream live latency data to the frontend
- Turborepo monorepo: Next.js · Express · PostgreSQL · Redis · BullMQ · Prisma · Docker · CI/CD

---

### 🌾 [Sahaay AI](https://github.com/Sarthak-Jaiswal4) — AI Farming Assistant
AI assistant for farmers over WhatsApp and voice calls.
- Inngest pipeline: Twilio → weather APIs → Tavily scraper → vector DB + Neo4j knowledge graph
- GraphRAG for crop–disease–treatment reasoning
- Stack: Node.js · Python · FastAPI · Neo4j · LangChain · Twilio

---

### 🎨 [SketchBoard](https://github.com/Sarthak-Jaiswal4) — Collaborative Whiteboard
Real-time multiplayer canvas with production-grade infra.
- WebSockets + Redis pub/sub for real-time sync across clients
- Object selection, movement, undo/redo, delete recovery
- Zero-downtime CI/CD: GitHub Actions → Docker → AWS EC2 rolling updates
- Stack: Node.js · TypeScript · WebSockets · Redis · Docker · AWS EC2

---

### 🐳 [mini-docker](https://github.com/Sarthak-Jaiswal4/mini-docker) — Container Runtime in Go
Built a working container runtime from scratch to understand how Docker actually works.
- Linux namespaces, cgroups v2, OverlayFS, PivotRoot, `SYS_SETNS` for exec
- Supports image layering, process isolation, and `exec` into running containers
- Stack: Go · Linux kernel APIs

---

## At Aurviz — what I've actually built

| Component | What |
|---|---|
| Intent classifier | TFLite Keras model for fast single-intent queries; FunctionGemma 270M (LiteRT-LM, dynamic_int8) as fallback for complex multi-intent |
| Slot extraction | GLiNER vs FunctionGemma evaluation across 30-tool inventory; regex for literal slots, FunctionGemma for time-bearing + inference slots |
| Observability | Pydantic logging schema with typed latency breakdowns; BLE GATT telemetry struct in C → Kotlin ByteBuffer parser |
| BLE integration | Realtek smart glasses hardware via `GlassesHardwareBridge` (SDK isolation layer); Android as sole internet gateway |
| Latency reduction | ASR + Gemini TTFT identified as dominant bottlenecks; pipeline brought from 10s → <4s |

---

## Stack

```
Languages      C++  JavaScript  TypeScript  Python  SQL  Kotlin  Go
Frontend       React.js  Next.js  GSAP  HTML5  CSS3
Backend        Node.js  Express.js  WebSockets  Socket.IO  BullMQ  Inngest
Databases      PostgreSQL  MongoDB  Redis  Neo4j  Prisma
AI / ML        LangChain  TFLite  LiteRT-LM  Gemini API  RAG  GraphRAG  FastAPI
DevOps         Docker  AWS (EC2, S3)  GitHub Actions  CI/CD  Prometheus  Grafana
Android        Kotlin Coroutines  BLE/GATT  on-device ML
```

---

## Background

- 2nd year B.Tech IT @ **Harcourt Butler Technical University**, Kanpur
- 450+ DSA problems in C++
- Hackathons: Enigma @ RIET (cleared 2 rounds) · Brainwave 2.0 @ DTU (presented Sahaay AI)

---

<p align="center">
  If something here looks interesting, feel free to reach out — <a href="mailto:sarthakjazz8@gmail.com">sarthakjazz8@gmail.com</a>
</p>

# 🤖 Robotics OSS Radar

> **Podcast companion for open-source robotics & autonomous systems**
> Tracking the most active GitHub projects, recent development highlights, and episode opportunities.

---

## 📡 What Is This?

**Robotics OSS Radar** is a podcast companion that monitors the most recently active open-source repositories in the robotics and autonomous-vehicles ecosystem. We track recent commits, highlight development trends, and generate episode ideas — so you never miss a story worth telling.

---

## 🔍 Current Radar: Top 3 Recently Active Projects

---

### 1. 🧠 Rumi — Autonomous Scientific Research Agents

| Field | Detail |
|-------|--------|
| **Repo** | [`josemanuelm9203/rumi`](https://github.com/josemanuelm9203/rumi) |
| **Tag** | `autonomous-vehicles` |
| **Language** | Multi-platform (Windows) |
| **License** | Free / open |
| **Latest Commit** | *Update README.md* — **Sep 18, 2026** |
| **Previous Activity** | Docs overhaul (Jun 9, 2026), Initial commit (Jun 2, 2026) |

**What it does:** Rumi is a **terminal-native framework** for building autonomous scientific research agents. It runs a **10-stage pipeline** that breaks down a research topic into smaller parts, extracts entities, builds a knowledge graph, flags contradictions, and suggests new experiments. It uses **88 modular "brain" programs** to check facts and challenge assumptions — including a dedicated "Skeptic Review" module that actively challenges your conclusions.

#### 📊 Recent Commit Activity

| Date | SHA | Change | Why It Matters |
|------|-----|--------|-----------------|
| Sep 18, 2026 | `b95ad14` | README refreshed | Documentation keeps pace with feature growth — signals maturity |
| Jun 9, 2026 | `23e3723` | All modules documented; `benchmark_runner` removed | Scope refinement — moving from experimental to production-ready |
| Jun 9, 2026 | `d66c05c` | Parallel docs update | Duplicate commit suggests active iteration on documentation |
| Jun 2, 2026 | `260ca5f` | **Initial commit** | Framework launched with 10-stage pipeline |

#### 🔑 Key Architecture Highlights
- **10-Stage Pipeline:** Topic decomposition → Entity extraction → Knowledge graph construction → Contradiction mining → Hypothesis formatting → Experiment design → Skeptic review → Plan critique → Final report
- **88 independently verifiable "brain modules"** — each checks a specific fact or logical rule
- **Knowledge Mapping:** Visual graph connecting data points to reveal hidden relationships
- **Contradiction Mining:** Automatically flags claims that conflict with verified data
- **Skeptic Review:** A dedicated critic module that challenges assumptions (rare in AI tools!)
- **Local-first:** All data stays on your machine — no third-party cloud dependency

#### 🎙️ Potential Episode Topics
- *"Can AI Review Its Own Assumptions? The Skeptic Module in Autonomous Research"*
- *"From Knowledge Graphs to Experiments: The 10-Stage Pipeline of Rumi"*
- *"Agentic Science: Will Autonomous Agents Replace Literature Reviews?"*
- *"Why Local-Only Matters for Research AI (No Cloud, No Censorship)"*

---

### 2. 🚗 InterFuser-UI — Real-Time CARLA Autonomous Driving Monitor

**Repo:** [`zubairm8580/InterFuser-UI`](https://github.com/zubairm8580/InterFuser-UI)  
**Tags:** `autonomous-vehicles`, `carla-simulator`, `sensor-fusion`, `computer-vision`, `transformer`  
**License:** Apache-2.0 | **Language:** Python | **Stars:** 1

#### 📊 What It Does
A **Pygame-based real-time dashboard** for monitoring autonomous driving runs in the CARLA simulator. It fuses multi-camera feeds, LiDAR bird's-eye views, route data, and safety-rule alerts into a single screen — giving researchers a window into how a self-driving stack perceives and reacts to the world.

#### 📊 Recent Commit Activity

| Date | SHA | Change | Why It Matters |
|------|-----|--------|-----------------|
| Sep 18, 2026 | `d60a7af` | README updated (v3.3) | Documentation keeps pace with the latest release |
| Apr 3, 2026 | `3b73310` | **Full UI application + model core shipped** | The big bang commit — 41 KB UI.py, complete docs, working demo |
| Apr 2, 2026 | `d40d68b` | Application scaffold added | Rapid iteration — two commits in one day to stabilize the app |
| Mar 17, 2026 | `92be73f` | Model core contribution (justinbrianhwang) | First external contributor — signals community interest |
| Mar 17, 2026 | `7974159` | **Initial commit** | Project bootstrapped by Sunjun Hwang |

#### 🔑 Key Architecture Highlights
- **Multi-Camera View:** Front, rear, and side cameras rendered simultaneously
- **LiDAR Bird's-Eye Map:** Top-down occupancy grid from LiDAR point clouds
- **Safety Rule Alerts:** Real-time compliance checking overlaid on the feed
- **Route-Aware Control:** Visualizes planned routes + actual trajectory deviations
- **InterFuser Sensor-Fusion Overlay:** Tracks how camera + LiDAR + transformer model outputs are combined
- **Transformer-based PerceptionStack:** INTERFuser architecture uses attention mechanisms for multi-modal fusion

#### 🎙️ Potential Episode Topics
- *"Seeing Through the Eyes of a Self-Driving Car: Inside CARLA & InterFuser"*
- *"Sensor Fusion in Real-Time: How Pygame + Transformer Models Drive the View"*
- *"From Simulation to Street: What CARLA Taught Us About Autonomous Driving Safety"*
- *"Why Dashboards Matter: Making Black-Box Models Explainable"*
- *"The 41-KB UI File: What's Inside a Real-Time Driving Monitor?"*

---

### 3. ⚡ QuestDB — High-Performance Time-Series Database for Robotics Telemetry

**Repo:** [`questdb/questdb`](https://github.com/questdb/questdb)  
**Tags:** `time-series`, `iot`, `robotics`, `aerospace`, `telemetry`  
**License:** Apache-2.0 | **Language:** Java (zero-GC, C++/Rust on hot paths)  
**⭐ 17,328 stars** | 🍴 **1,648 forks** | **Daily commits — extremely active**

#### 📊 What It Does
QuestDB is an open-source, **low-latency time-series database** purpose-built for high-throughput event ingestion. It's used in **aerospace and robotics** for flight-test telemetry, fleet data, and mission replay. With up to **19 million rows/sec ingestion** and **220 million rows/sec query streaming**, it's the data backbone for the most demanding autonomous systems.

#### 📊 Recent Commit Activity (Last 5 Commits — All Within 1 Week!)

| Date | SHA | Change | Why It Matters |
|------|-----|--------|-----------------|
| Sep 18, 2026 | `4e8ea7e` | **🔥 feat(core): Query resource isolation primitives (#7585)** | Queries can no longer starve each other — critical for multi-tenant robotic deployments where one robot's telemetry shouldn't crash another's dashboard |
| Sep 17, 2026 | `fc7a28b` | **⚡ perf(sql): Breaking change — latest-by queries accelerated with partition-key filters (#7615)** | Huge win for telemetry lookups; this is the query pattern used most in time-series robotics data |
| Sep 16, 2026 | `a6f64f5` | **🐛 fix(sql): Covering index nulling bug (#7559)** | Data integrity fix — ensures indexed columns are correctly nulled, preventing silent data corruption |
| Sep 15, 2026 | `f9d4f51` | **🔧 feat(qwp): Browser negotiation + session authentication (#7531)** | QWP WebSocket protocol now supports secure connections — essential for production robot deployments |
| Sep 11, 2026 | `dbf0a87` | **✅ test(core): Stabilized log & fiber timing tests (#7593)** | CI reliability wins — means faster, more trustworthy releases |

#### 🔑 Key Architecture Highlights
- **19M rows/sec peak ingestion** — 5× faster than ClickHouse, 35× faster than TimescaleDB
- **QWP (QuestDB Wire Protocol):** Binary columnar protocol over WebSocket — unified ingest + query on one connection
- **Materialized & Live Views:** Real-time window functions for streaming telemetry (e.g., 15-second rolling averages of lidar data)
- **Tiered Storage:** Hot in-memory → native columnar → Apache Parquet on object storage
- **Zero-GC Java:** No garbage pauses during critical queries — deterministic latency for real-time systems
- **SQL extensions for time-series:** `SAMPLE BY`, `LATEST ON`, `ASOF JOIN`, `WINDOW JOIN`, `HORIZON JOIN`
- **AI coding agent integration:** Works with Claude Code, Cursor, and any MCP client
- **Open formats:** Parquet, Iceberg, Arrow — your data isn't locked in

#### 🏢 Where QuestDB Runs in Robotics
- **Aerospace:** Flight-test telemetry, mission replay
- **Fleet data:** Multi-vehicle tracking and coordination
- **Energy & infrastructure:** Turbine, reactor, and grid monitoring
- **AI coding agents:** QuestDB skills for autonomous code review

#### 🎙️ Potential Episode Topics
- *"Feeding the Beast: How 19M Rows/Second Changes Robotics Telemetry"*
- *"From Flight Test to Factory Floor: QuestDB in Aerospace & Robotics"*
- *"The Database Under Your Robot: Why Time-Series Beats General-Purpose"*
- *"Query Resource Isolation: Making Sure Your Autopilot Doesn't OOM Your Dashboard"*
- *"Breaking Changes That Break Nothing: How QuestDB Ships Performance at Scale"*
- *"QWP: The Binary Protocol That Makes Robots Speak Fluent Data"*

---

## 📊 Radar Summary

| # | Project | Domain | Stars | Commit Cadence | Vibe |
|---|---------|--------|-------|-----------------|------|
| 1 | **Rumi** | Autonomous Research Agents | New | ~2/mo | 🧠 AI-first science |
| 2 | **InterFuser-UI** | CARLA Self-Driving | 1 | Steady (Apr→Sep) | 🚗 Simulation & CV |
| 3 | **QuestDB** | Time-Series DB for Robotics | 17.3K | **Daily** (5 commits/wk) | ⚡ Infrastructure muscle |

---

## 🎙️ Episode Pipeline

| Priority | Project | Suggested Angle | Status |
|----------|---------|-------------------|--------|
| 🔴 **High** | QuestDB | The infrastructure layer — how robots store & query data at scale | In progress |
| 🟡 **Medium** | InterFuser-UI | Perception + simulation — what CARLA reveals about self-driving safety | TBD |
| 🟡 **Medium** | Rumi | Agentic science — can AI autonomously run its own research? | TBD |

---

## 📋 How to Contribute

This is a **living document**. To suggest a project or submit an episode idea:

1. Fork this repo
2. Add your candidate to the radar (follow the format above)
3. Open a PR with your suggestions
4. Or open an **Issue** with the `episode-suggestion` label

---

## 🔗 Useful Links

- [QuestDB Live Demo](https://demo.questdb.io/) — Scan 2 billion+ rows in milliseconds
- [CARLA Simulator](https://carla.org/) — Open-source autonomous driving simulator
- [QuestDB Documentation](https://questdb.com/docs/) — Full QWP & SQL guides
- [QWP vs ILP Ingestion Benchmark](https://questdb.com/blog/qwp-vs-ilp-ingestion-benchmark/) — 19M rows/sec proof
- [Streaming 500M Rows into Arrow](https://questdb.com/blog/streaming-500-million-rows-into-apache-arrow/) — 220M rows/sec query proof
- [QuestDB vs InfluxDB Comparison](https://questdb.com/blog/influxdb-vs-questdb-comparison/) — Head-to-head benchmarks

---

*Built for the open-source robotics community. Licensed under MIT.*
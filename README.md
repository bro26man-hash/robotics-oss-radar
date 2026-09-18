# 🤖 Robotics OSS Radar

> Open-Source Robotics & Autonomous Systems Radar — tracking the most active repos, recent development highlights, and podcast episode ideas.

---

## 📡 Tracked Projects

### 1. [Sinan Robo](https://github.com/sinanlabs/robo) — `sinanlabs/robo`
**Tag:** `robotics` · **Language:** Astro · **Focus:** VLA Foundation Model Index

**What it is:**
Sinan Robo (司南·机脑) is an **auditable index of open and open-weight Vision-Language-Action (VLA) robot foundation models**. It catalogues 25+ models (GR00T N1.6/N1.7, π0/π0.5, OpenVLA, Octo, RDT-1B, MolmoAct, and others) across 12 robot bodies (Unitree G1/H1, Franka FR3, ALOHA 2, and others), with every field backed by an evidence URL — licence, parameter count, target embodiment, and more.

**Recent Development Highlights (as of Sep 2026):**
- 🔴 **Real-world GPU benchmarking underway** — Active testing of 5 VLA models on both A800 80GB and RTX 5090 GPUs, with RTX 4090 vs 5090 head-to-head comparisons and per-1k-inference cost tracking being written into the data layer.
- 🟡 **"Robo 2.0" workspace redesign** — A major architectural pivot from a static index to an interactive workbench, adding: activity signals (daily GitHub/HF/ModelScope scraping with model-page activity cards & 3 leaderboard views), deployment recipes (generalized steps, environment gotchas tables, 5 published recipes, unreproducible-items list), a cost/frequency workbench, dataset tracking, Jetson edge support, and crowd-testing workflows.
- 🟢 **Hardware reference layer expanded** — Added A800 80GB with rental-price fallbacks to AutoDL domestic on-demand median pricing, giving users real-world cost context.
- 📊 **Q4 2026 target:** 40+ models, 25+ bodies, first reproducible latency measurements published.

**🎙️ Potential Episode Topics:**
- *"The VLA Model Landscape: Why We Can't Agree on What's Open"* — The licensing hell between code licences and weight licences, and why Sinan Robo refuses to rank.
- *"From Index to Workbench: Robo 2.0 and the Future of Auditable Robotics AI"* — What happens when an index becomes a living research tool.
- *"GPU Benchmarking VLA Models: A800 vs 5090 and the Real Cost of Inference"* — Hard numbers on what it actually costs to run these models.

---

### 2. [InterFuser-UI](https://github.com/zubairm8580/InterFuser-UI) — `zubairm8580/InterFuser-UI`
**Tag:** `autonomous-vehicles` · **Language:** Python · **License:** Apache-2.0 · **Stars:** 1

**What it is:**
A **real-time Pygame-based monitoring dashboard** for the InterFuser autonomous driving stack in the CARLA simulator. It consolidates front/rear/side camera feeds, a bird's-eye LiDAR map, route data, vehicle control states, safety rule alerts, and scene data into a single screen — making it easy to watch how a self-driving stack perceives and reacts to its environment.

**Recent Development Highlights (as of Sep 2026):**
- 🔴 **v3.3 released** — Latest version packaged for Windows with a dedicated download, indicating mature stabilization.
- 🟡 **Full application buildout completed** — The `interfuser_core/` module and `UI.py` (41KB) are in place, with comprehensive documentation and requirements pinned.
- 🟢 **Multi-sensor fusion visualization** — Simultaneous camera + LiDAR bird's-eye view with route-aware control tracing and safety rule overlay, which is rare for open-source CARLA tooling.
- 📦 **Windows-first deployment** — Pre-packaged ZIP distributions lower the barrier to entry for non-Linux users, which is a common pain point in the CARLA community.

**🎙️ Potential Episode Topics:**
- *"Seeing Is Believing: Why Real-Time Sensor Fusion Dashboards Matter"* — How tools like InterFuser-UI democratize self-driving stack debugging.
- *"CARLA in the Wild: From Simulation to Validation"* — The gap between simulated driving and real-world deployment, and what open-source monitoring tools reveal.
- *"InterFuser Under the Hood: Transformer-Based Sensor Fusion for Autonomous Driving"* — The architecture behind multi-camera + LiDAR fusion.

---

### 3. [Rumi](https://github.com/josemanuelm9203/rumi) — `josemanuelm9203/rumi`
**Tag:** `autonomous-vehicles` · **Focus:** Autonomous Scientific Research Agents

**What it is:**
A **terminal-native framework for building autonomous scientific research agents** that use computer models to process data, find patterns, and generate new experimental hypotheses. Rumi runs an 88-module "brain pipeline" inside your terminal, performing hypothesis generation, knowledge mapping, contradiction mining, and skeptic review — essentially an AI-powered research assistant that challenges its own assumptions.

**Recent Development Highlights (as of Sep 2026):**
- 🔴 **v3.6 released (Sept 2026)** — Latest version with improved parsing tools and faster analysis, available as a Windows .exe installer.
- 🟡 **10-stage pipeline documented** — The full hypothesis discovery workflow (topic decomposition → entity extraction → knowledge graph construction → contradiction flagging → skepticism review → experiment design) is now fully documented in the README.
- 🟢 **Contradiction Mining & Skeptic Review modules** — Unique among research agents for having a built-in "critic" module that actively challenges assumptions, reducing confirmation bias in automated research.
- ⚠️ **Active maintenance cadence** — Monthly commits with focused updates (June: documentation overhaul + module completeness, September: v3.6 release).

**🎙️ Potential Episode Topics:**
- *"Autonomous Research Agents: Can an AI Do Science Without Biasing It?"* — The promise and peril of self-correcting research pipelines.
- *"88 Brains, One Terminal: Inside Rumi's Modular Architecture"* — How micro-agents cooperate for macro-level scientific discovery.
- *"From Hypothesis to Experiment: The Autonomous Research Loop"* — What fully automated scientific discovery looks like — and when we can trust it.

---

## 🗓️ Episode Calendar (Suggested)

| Episode | Project | Angle |
|---------|---------|-------|
| #1 | Sinan Robo | The VLA licensing maze & why auditability matters |
| #2 | InterFuser-UI | Democratizing self-driving stack visualization |
| #3 | Rumi | Can an autonomous agent do unbiased science? |
| #4 | Sinan Robo (follow-up) | GPU benchmarking deep-dive: real inference costs |
| #5 | InterFuser-UI (follow-up) | From CARLA simulation to real-world validation |
| #6 | Rumi (follow-up) | The skeptic review module and AI research ethics |

---

## 📊 Activity Snapshot (as of September 18, 2026)

| Project | Stars | Language | Key Theme |
|---------|-------|----------|-------------------------------|
| Sinan Robo | — | Astro | VLA model auditability & GPU benchmarking |
| InterFuser-UI | 1 | Python | Real-time CARLA sensor fusion visualization |
| Rumi | — | — | Autonomous scientific research agents |

---

## 📋 Tracking

See the open issue **[Projects to Revisit & Upcoming Releases](https://github.com/bro26man-hash/robotics-oss-radar/issues/54)** for the running checklist of items to revisit before the next episode cycle.

---

## 🤝 Contributing

Pull requests and suggestions are welcome! To propose a new project or episode topic:
1. Open an issue describing the project and why it matters
2. Tag it with `proposal` and `episode-topic`
3. The maintainers will review and add to the radar

## 📄 License

This project is open-source under the [MIT License](LICENSE).

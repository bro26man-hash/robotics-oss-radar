# 🤖 Robotics OSS Radar

> *A living research hub tracking the most active open-source robotics & autonomous systems projects — curated for the podcast.*

---

## 📡 What Is This?

**Robotics OSS Radar** is a podcast companion project that monitors the most recently active open-source repositories in the robotics and autonomous-vehicles ecosystem. We track recent commits, highlight development trends, and generate episode ideas — so you never miss a story worth telling.

---

## 🔍 Current Radar: Top 3 Recently Active Projects

### 1. 🧠 Rumi — Autonomous Scientific Research Agents

| Field | Detail |
|-------|--------|
| **Repo** | [`josemanuelm9203/rumi`](https://github.com/josemanuelm9203/rumi) |
| **Tag** | `autonomous-vehicles` |
| **Language** | Multi-platform (Windows) |
| **Latest Commit** | *Update README.md* — Sep 18, 2026 |
| **Previous Activity** | Docs overhaul (Jun 2026), Initial commit (Jun 2026) |

**What it does:** Rumi is a terminal-native framework for building autonomous scientific research agents. It runs a **10-stage pipeline** that breaks down a research topic into smaller parts, extracts entities, builds a knowledge graph, flags contradictions, and suggests new experiments. It uses **88 modular "brain" programs** to check facts and challenge assumptions.

**Recent Development Highlights:**
- 📝 **README refresh (Sep 2026)** — Documentation updated to reflect all modules, signaling growing feature completeness.
- 📚 **Module documentation expansion (Jun 2026)** — Two parallel commits added missing module docs and removed the `benchmark_runner`, suggesting a v1.0 release is being polished.
- 🚀 **Initial launch (Jun 2026)** — First commit established the 10-stage hypothesis-discovery pipeline.

**🎙️ Potential Episode Topics:**
- "Can AI Agents Do Science? Inside Rumi's 10-Stage Research Pipeline"
- "The 88 Brain Programs: Modular AI for Autonomous Discovery"
- "From Terminal to Lab Bench: How Autonomous Research Agents Work"

---

### 2. 🚗 InterFuser-UI — Real-Time CARLA Autonomous Driving Monitor

| Field | Detail |
|-------|--------|
| **Repo** | [`zubairm8580/InterFuser-UI`](https://github.com/zubairm8580/InterFuser-UI) |
| **Tag** | `autonomous-vehicles` |
| **Language** | Python |
| **License** | Apache-2.0 |
| **Latest Commit** | *Update README.md* — Sep 18, 2026 |
| **Previous Activity** | UI application + model core (Apr 2026), Initial commit (Mar 2026) |

**What it does:** InterFuser-UI is a **Pygame-based real-time dashboard** for monitoring autonomous driving runs in the CARLA simulator. It fuses multi-camera feeds, LiDAR bird's-eye views, route data, and safety-rule alerts into a single screen — giving researchers and developers a window into how a self-driving stack perceives and reacts to the world.

**Recent Development Highlights:**
- 📝 **README update (Sep 2026)** — Documentation refreshed, likely for v3.3 release.
- 🖥️ **Full UI application shipped (Apr 2026)** — Three commits in rapid succession added the complete InterFuser application with model core, UI.py (41 KB!), and comprehensive documentation.
- 🏗️ **Initial commit (Mar 2026)** — Project bootstrapped with core architecture.

**Key Features:**
- 🎥 Multi-camera view (front, rear, side)
- 🗺️ LiDAR bird's-eye map
- ⚠️ Safety rule alerts
- 🛣️ Route-aware control visualization
- 🤖 InterFuser sensor-fusion data overlay

**🎙️ Potential Episode Topics:**
- "Seeing Through the Eyes of a Self-Driving Car: Inside CARLA & InterFuser"
- "Sensor Fusion in Real-Time: How Pygame + Transformer Models Drive the View"
- "From Simulation to Street: What CARLA Taught Us About Autonomous Driving"

---

### 3. 📍 slam-regression-ci — CI Regression Gate for SLAM & Odometry

| Field | Detail |
|-------|--------|
| **Repo** | [`pyy52/slam-regression-ci`](https://github.com/pyy52/slam-regression-ci) |
| **Tag** | `robotics` |
| **Language** | Python 3.8+ |
| **License** | MIT |
| **Latest Commit** | `feat: TUM trajectory loading, association, and ATE/RPE metrics (#6)` — Sep 18, 2026 |
| **Previous Activity** | `chore: bootstrap repository structure` — Sep 18, 2026 |

**What it does:** A **lightweight CI regression gate** specifically designed for SLAM (Simultaneous Localization and Mapping) and odometry trajectories. It compares a candidate trajectory against a committed baseline, applies configurable per-metric thresholds (ATE RMSE, RPE translation RMSE), and fails CI with both a **human-readable Markdown report** and a **machine-readable JSON report**.

**Recent Development Highlights:**
- 🎉 **First feature release (v0.1.0 in progress)** — TUM trajectory loading and association landed, plus ATE/RPE metric computation. This is the repo's first real feature commit!
- 🏗️ **Repository bootstrapped (Sep 2026)** — Full community scaffolding: `CONTRIBUTING.md`, `CODE_OF_CONDUCT.md`, `SECURITY.md`, `pyproject.toml` — professional-grade open-source setup from day one.
- 🧪 **Test infrastructure** — Both `src/` and `tests/` directories established.

**Why it matters:** SLAM is the backbone of indoor robotics, drones, and AR/VR. Without automated regression testing, a subtle algorithm change can silently degrade localization accuracy by centimeters — and this tool catches that before it ships.

**🎙️ Potential Episode Topics:**
- "Why Your SLAM Algorithm Needs CI: Ate, RPE, and the Metrics That Matter"
- "From Lab to Pipeline: Making SLAM Testable with Regression Gates"
- "The Silent Killer: How Small Numerical Drifts Break Autonomous Systems"

---

## 📊 Radar Summary

| # | Project | Domain | Stars | Last Activity | Vibe |
|---|---------|--------|-------|-----------------|------|
| 1 | **Rumi** | Autonomous Research Agents | — | Sep 18, 2026 | 🧠 AI-first science |
| 2 | **InterFuser-UI** | CARLA Self-Driving | 1 | Sep 18, 2026 | 🚗 Simulation & CV |
| 3 | **slam-regression-ci** | SLAM/ODometry Testing | — | Sep 18, 2026 | 📍 Engineering rigor |

---

## 🎙️ About the Podcast

*Robotics OSS Radar* is a podcast exploring the stories behind the open-source projects that are shaping the future of robotics and autonomous systems. Each episode dives into a real repo — its code, its contributors, its challenges — and asks: *what's next?*

**Subscribe & Follow:**
- [RSS Feed](#) 
- [Apple Podcasts](#)
- [Spotify](#)
- [YouTube](#) 
- [GitHub](#)

---

## 🤝 Contributing

Found a great repo we should track? Open an issue or submit a PR! We love suggestions.

1. Fork this repo
2. Add your candidate to `projects/`
3. Open a pull request with your rationale

---

## 📜 License

This project is open-source and available under the [MIT License](LICENSE).
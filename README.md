# 🤖 Robotics OSS Radar

> **Your weekly scan of the most active open-source repos in autonomous vehicles & robotics** — tracking commits, development highlights, and podcast-ready story angles.

---

## 🔍 Why This Repo Exists

The open-source robotics ecosystem moves fast. Every day, builders around the world are pushing code that brings us closer to fully autonomous systems. This repo is the **central scratchpad** for the *Robotics OSS Radar* podcast — cataloguing the projects worth knowing about, the commits worth discussing, and the episodes worth recording.

---

## 📡 This Week's Tracked Projects

### 1. 🧠 Rumi — Autonomous Scientific Research Agents
**Repo:** [josemanuelm9203/rumi](https://github.com/josemanuelm9203/rumi)  
**Topic:** `autonomous-vehicles`  
**Language:** Cross-platform (Windows)  
**License:** Not specified

**What it is:**  
Rumi is a terminal-native framework for building autonomous scientific research agents. It uses 88 small "brain programs" to process data, find patterns, and generate testable hypotheses. Think of it as an automated research assistant that works inline with your workflow — from hypothesis generation and knowledge mapping to contradiction mining and skeptical self-review.

**Latest Commit (Sep 18, 2026):**  
`b95ad14` — *Update README.md*  
The project is actively refreshing documentation, signaling preparation for broader adoption or an upcoming release.

**Recent Development Highlights:**
- **10-stage pipeline** now fully documented: topic decomposition → entity extraction → knowledge graph construction → pattern finding → logical trap detection → hypothesis formatting → experiment planning
- **88 modular brain programs** for multi-modal reasoning
- **Contradiction Mining** module flags inconsistencies against verified data
- **Skeptic Review** module challenges assumptions before conclusions
- **Jun 2026 docs overhaul** — Two parallel commits added all missing module docs and removed `benchmark_runner`, suggesting a v1.0 release is being polished

🎙️ **Episode Angle:** *"Can an AI Do Your Research For You? Inside the autonomous agent pipeline"* — Explore how autonomous agents are moving from simple chatbots to structured scientific workflows with deterministic, multi-stage pipelines.

---

### 2. 🚗 InterFuser-UI — Real-Time CARLA Autonomous Driving Monitor
**Repo:** [zubairm8580/InterFuser-UI](https://github.com/zubairm8580/InterFuser-UI)  
**Topic:** `autonomous-vehicles`  
**Language:** Python  
**License:** Apache-2.0 ⭐ 1 star

**What it is:**  
A Pygame-based real-time visualization dashboard for the **InterFuser** autonomous driving stack, running inside the **CARLA** simulator. It fuses camera feeds, LiDAR bird's-eye maps, route data, vehicle control states, and safety rule alerts into a single monitor view — making it ideal for debugging, demos, and understanding how multi-modal sensor fusion works in practice.

**Latest Commit (Sep 18, 2026):**  
`d60a7af` — *Update README.md*  
Documentation refresh suggests the project is stabilizing and preparing for community feedback.

**Recent Development Highlights:**
- **Multi-camera view** — front, rear, and side feeds rendered simultaneously
- **LiDAR bird's-eye view** — top-down occupancy map for obstacle detection
- **Safety rule overlay** — real-time alerts when driving behavior violates constraints
- **Route-aware control visualization** — lane changes, turns, and road-edge tracking
- **InterFuser sensor fusion data view** — watch how camera + LiDAR + radar inputs combine
- **Apr 2026 — Full UI application shipped** — Three rapid commits added the complete InterFuser application with model core, UI.py (41 KB!), and comprehensive documentation

🎙️ **Episode Angle:** *"Seeing Is Believing: Watch a self-driving car perceive the world in real-time"* — A hands-on walkthrough of sensor fusion visualization, from raw LiDAR points to a drivable bird's-eye map.

---

### 3. 🗺️ slam-regression-ci — CI Regression Gate for SLAM & Odometry
**Repo:** [pyy52/slam-regression-ci](https://github.com/pyy52/slam-regression-ci)  
**Topic:** `robotics`  
**Language:** Python 3.8+  
**License:** MIT ✨ **Under active development — v0.1.0 in progress**

**What it is:**  
A lightweight, dependency-minimal CI tool that acts as a **regression gate** for SLAM (Simultaneous Localization and Mapping) and odometry trajectories. It compares a candidate trajectory against a committed baseline, applies configurable per-metric thresholds (ATE RMSE, RPE translation RMSE), and fails CI builds with both a human-readable Markdown report and a machine-readable JSON report. Fills a critical gap: how do you catch performance regressions in iterative robotics localization code?

**Latest Commit (Sep 18, 2026):**  
`0163184` — *feat: TUM trajectory loading, association, and ATE/RPE metrics (#6)*  
Major feature drop: full TUM trajectory format support, trajectory association algorithms, and the core ATE/RPE metric computations are now implemented.

**Recent Development Highlights:**
- **TUM trajectory loading** — native support for the standard TUM dataset format
- **Trajectory association** — aligns candidate and baseline trajectories for fair comparison
- **ATE (Absolute Trajectory Error)** — RMSE computation against ground truth
- **RPE (Relative Pose Error)** — translation RMSE for local drift detection
- **Dual reporting** — Markdown for humans, JSON for CI pipelines
- **CODE_OF_CONDUCT.md & SECURITY.md** — community-first governance from day one
- **Sep 2026 — Repository bootstrapped** — Full community scaffolding: `CONTRIBUTING.md`, `CODE_OF_CONDUCT.md`, `SECURITY.md`, `pyproject.toml` — professional-grade open-source setup from day one

🎙️ **Episode Angle:** *"The Boring Thing That Saves Robotics: Why regression testing for SLAM is harder than you think"* — A deep dive into how continuous integration meets iterative robotics development.

---

## 🎙️ Podcast Episode Planner

| # | Project | Episode Title | Priority | Status |
|---|---------|----------------|----------|--------|
| 1 | Rumi | *"Can an AI Do Your Research For You?"* | 🔴 High | 📝 Idea |
| 2 | InterFuser-UI | *"Seeing Is Believing: Real-Time Sensor Fusion in CARLA"* | 🔴 High | 📝 Idea |
| 3 | slam-regression-ci | *"The Boring Thing That Saves Robotics"* | 🟡 Medium | 📝 Idea |

### Episode Flow Suggestions:
1. **Cold Open:** Show a 30-second clip of InterFuser-UI running in CARLA — LiDAR point clouds, camera feeds, safety alerts. Ask: *"What does a self-driving car see?"*
2. **Act I:** Rumi — Can autonomous agents do science? Walk through the 10-stage pipeline.
3. **Act II:** InterFuser-UI — Inside the sensor fusion stack. Live demo walkthrough.
4. **Act III:** slam-regression-ci — The unsung hero of robotics CI. Why metrics matter.
5. **Wrap-Up:** What's next? Link to the tracking issue and invite listener submissions.

---

## 📋 Contribution Guide

This is a living repo! To add a new project:

1. Fork this repository
2. Add your project summary under `projects/`
3. Include: repo link, topic tags, latest commit SHA, 3–5 bullet highlights, and a suggested episode angle
4. Open a Pull Request with the title `Add: [Project Name] to radar`

---

## 📡 Data Sources

- **GitHub Search API** — `topic:autonomous-vehicles`, `topic:robotics`
- **Commit tracking** — Latest 5 commits per repo
- **Issue tracking** — See the open issue: [*Projects to Revisit & Upcoming Releases*](https://github.com/bro26man-hash/robotics-oss-radar/issues)

---

*Built for the open-source robotics community. See something missing? Open an issue or submit a PR!*

---

**Tags:** `#robotics` `#autonomous-vehicles` `#SLAM` `#CARLA` `#open-source` `#podcast` `#CI/CD` `#sensor-fusion` `#autonomous-agents`

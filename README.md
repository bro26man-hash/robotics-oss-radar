# 🤖 Robotics OSS Radar

> Tracking the most active open-source robotics & autonomous vehicle projects — for our podcast.

## 📡 Top 3 Projects Under the Lens

---

### 1. [commaai/openpilot](https://github.com/commaai/openpilot)
**⭐ 63,675 stars | Language: Python | License: MIT | Last updated: Sept 17, 2026**

*openpilot is an operating system for robotics. Currently, it upgrades the driver assistance system on 300+ supported cars.*

**Latest Commit (Sept 17, 2026):**
- **`1328ace` — "Remove model chunking and use LFS for Chestnut releases"** (PR #38941, by Harald Schäfer)
  - Major infrastructure change: model files are no longer chunked but managed via Git LFS, streamlining the release pipeline for the upcoming **"Chestnut"** release codename.
  - Signals that commaai is preparing a significant new release with improved model distribution.

**Additional Recent Commits:**
- **`7db7735` — "rm chestnut power test"** (PR #38943) — Cleaned up a transient power test for the Chestnut device
- **`cd1490a` — "modeld: 2× faster Chestnut build"** (PR #38656) — Doubled inference build speed for Chestnut's modeld, a major performance win for on-device vision pipelines
- **`bd176cb` — "ui: remove question marks"** (PR #38938) — Cleaned up UI placeholders
- **`4d9d1bc` — "ui: not-paired bookmark alert"** (PR #38936) — Added a UX alert when a bookmarked device isn't paired

**Key Architecture:** Modeld (deep perception), Controld (longitudinal/lateral control), Params (parameter management), Logd (logging), SD (streaming), UI (comma three/four dashboard), Panda (secure CAN bus hardware). Supports 300+ cars via the comma three/four device and car harness.

**🎙️ Potential Episode Topics:**
- "openpilot at 63K stars: how a community-driven OS took on 300+ cars"
- "Chestnut is coming: what's new in openpilot's next hardware generation"
- "2× faster modeld: the engineering behind on-device vision speedups"
- "From comma three to Chestnut: hardware evolution in open-source driving"
- "LFS for models: how openpilot manages gigabyte-scale ML artifacts at scale"
- "The safety model: ISO 26262 compliance in an open-source Stack"

---

### 2. [AtsushiSakai/PythonRobotics](https://github.com/AtsushiSakai/PythonRobotics)
**⭐ 30,533 stars | Language: Python | License: MIT | Last updated: Sept 17, 2026**

*Python sample codes and textbook for robotics algorithms — the go-to educational resource for understanding autonomous motion, search, localization, mapping, and path planning, all in clean Python.*

**Latest Commit (Sept 2, 2026):**
- **`08b453a` — "build(deps): bump github/codeql-action from 4.37.4 to 4.37.9"** (PR #1423, by dependabot)
  - A dependency bump for GitHub's CodeQL security scanning action. This indicates the repo maintains security best practices even while primarily being an educational/resource project.

**Recent Development Highlights:**
- **Security hygiene maintained** — CodeQL action bump shows the maintainer cares about supply-chain security even in a textbook repo
- **Broad algorithm coverage** — from particle filters and SLAM to RRT* and A*, the repo covers the full robotics algorithms curriculum
- **Educational focus** — each algorithm includes clear explanations, visualizations, and step-by-step Python implementations
- **Active dependency management** — regular updates to keep the environment current

**Key Modules:** Localization (Kalman/particle filters, Monte Carlo), Mapping (grid, EKF, FastSLAM), SLAM (graph-based, EKF), Path Planning (A*, Dijkstra, RRT, RRT*, PRM), Trajectory Generation, Control (PID, LQR, MPC), and Sensor Fusion.

**🎙️ Potential Episode Topics:**
- "PythonRobotics: the textbook that teaches the world robotics algorithms"
- "From A* to RRT*: how Python makes robotics algorithms accessible"
- "Why educational repos matter for the open-source robotics ecosystem"
- "SLAM explained with 50 lines of Python — inside the PythonRobotics approach"
- "Particle filters and Monte Carlo methods, practically implemented"
- "How this 30K-star repo is shaping the next generation of roboticists"

---

### 3. [ApolloAuto/apollo](https://github.com/ApolloAuto/apollo)
**⭐ 26,830 stars | Language: C++ | License: Apache-2.0 | Last updated: Sept 17, 2026**

*An open autonomous driving platform — a high-performance, flexible architecture that accelerates the development, testing, and deployment of Autonomous Vehicles. From GPS waypoint following (v1.0) to curb-to-curb urban driving (v5.5+) to large-scale functional deployment (v11.0).*

**Latest Commit (Apr 16, 2026):**
- **`d53aa3d` — "docs: fix README - remove invalid build status badges"** (by xiaoxinyu)
  - Documentation cleanup: removed stale CI/CD badges that pointed to broken build pipelines. This suggests the repo's CI infrastructure may have undergone changes, and the maintainers are maintaining external credibility.

**Recent Development Highlights:**
- **Apollo 11.0 BEB+OCC perception** — new bird's-eye-view and occupancy-grid perception models for enhanced 3D scene understanding
- **Beyond Lidar driver recovery** — PR #15762 restores and hardens the lidar driver pipeline for robust sensor data ingestion
- **README cleanup & documentation hygiene** — maintaining project credibility through careful docs management
- **Apollo 11.0 focus on large-scale deployment** — comprehensive upgrades to perception, localization, planning, and development toolchains; support for ARM/Orin architecture; 4D millimeter-wave radar integration; functional safety framework reinforcement
- **Apollo Studio & Data Pipeline** — introduced in v7.0, matured through v10/11 as a one-stop online development platform

**Key Modules:** Perception (BEB+OCC), Localization (HD maps, GPS/IMU), Prediction, Planning & Control (PnC), Decider, CyberRT middleware, Dreamview Plus visualization, Package management v2.0, Apollo Studio.

**🎙️ Potential Episode Topics:**
- "Apollo 11.0: from research to production — the BEB+OCC revolution"
- "Inside Baidu's Apollo: 11 versions of open-source autonomous driving"
- "Beyond Lidar: why sensor redundancy is the key to safe AVs"
- "Apollo Studio: the one-stop dev platform for autonomous driving"
- "What's new in Apollo 11.0 — ARM support, 4D radar, and functional safety"
- "Package management and plugin architecture: how Apollo scales for production"
- "Why README badges matter: credibility and dead links in open-source"

---

## 📊 Quick Comparison

| Project | Stars | Language | Focus | Latest Activity |
|---------|-------|----------|-------|-----------------|
| openpilot | 63,675 | Python | Full-stack driver assistance OS | **Active** — Chestnut release LFS migration + 2× modeld speedup (Sept 17) |
| PythonRobotics | 30,533 | Python | Educational robotics algorithms | **Maintained** — CodeQL security bump (Sept 2) |
| Apollo | 26,830 | C++ | Full autonomous driving platform | **Moderate** — BEB+OCC perception, lidar recovery, docs cleanup (Apr 16) |

## 🎙️ About This Project

This repo is a companion to our podcast on open-source robotics and autonomous systems. We track the most active GitHub projects, analyze their latest commits, and develop episode ideas — so listeners can follow along and contribute.

## 📋 Tracking

See the open issue **[Projects to Revisit & Upcoming Releases](https://github.com/bro26man-hash/robotics-oss-radar/issues/29)** for a detailed tracking checklist of these 3 projects.

---

*Generated for the Robotics OSS Radar podcast. Stay curious, stay open-source.*

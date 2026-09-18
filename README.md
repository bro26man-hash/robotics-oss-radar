# 🤖 Robotics OSS Radar

> Tracking the most active open-source robotics & autonomous vehicle projects — for our podcast.

## 📡 Top 3 Projects Under the Lens

---

### 1. [autonomous-ai/autonomous-os](https://github.com/autonomous-ai/autonomous-os)
**⭐ 347 stars | Language: Python | License: Apache-2.0 | Last updated: Sept 17, 2026**

*Autonomous OS is the "Android" for robots — install it and your robot comes alive. It's a fully customizable operating system where every component is swappable: engine, model, voice, skills, board. Robots declare what they have in a `ROBOT.md`, and the OS mounts exactly that.*

**Recent Development Highlights:**
- **fix(hal): drain scene speaker mute and restore scene-muted peripherals on wake** (`2a11eea`, Sep 17, 2026) — by Darren; resolves audio peripheral state corruption when a scene wakes from dormancy, ensuring speakers and mics reinitialize correctly
- **FIX (hal): drain scene speaker mute and reopen scene-muted peripherals on scene off** (`8dcc596`, Sep 17, 2026) — by Darren; paired fix for the reverse transition (scene off → restore), closing the peripheral lifecycle gap
- **CHORE (hal): drop scene drain test and its handle reset** (`463c08e`, Sep 17, 2026) — by Darren; cleanup of deprecated test infrastructure for the scene drain mechanism
- **Update & merge** (`d0e158d` / `98bdf6b`, Sep 17, 2026) — by Darren & leo; integration merges for the HAL speaker/drain subsystem refactor

**Key Architecture:** Agentic reasoning engine (Hermes, Claude Code, OpenClaw, PicoClaw, Codex, OpenCode behind a unified `AgentGateway`), Skills system (markdown-driven behaviors with `[HW:…]` hardware markers), HAL (Hardware Abstraction Layer with 13 capability interfaces), Safety gate (pure-function clamps on speed, brightness, quiet hours), Go daemon `os-server` on :5000, realtime voice (Gemini Live / OpenAI Realtime), swappable boards (RPi 4/5, CM4, OrangePi 4 Pro). Supports Lamp, Reachy Mini, and Intern robots out of the box.

**🎙️ Potential Episode Topics:**
- "The Android for robots: inside Autonomous OS"
- "Skills as markdown: howgable AI behaviors replace code"
- "Safety gates without ML: pure-function guarantees for robot hardware"
- "Six agentic runtimes, one gateway: swapping brains mid-conversation"
- "From Lamp to Reachy Mini: bring-your-own-robot in four markdown files"
- "HAL Friday: the hardware abstraction layer that makes robots swappable"

---

### 2. [aerostack2/aerostack2](https://github.com/aerostack2/aerostack2)
**⭐ 385 stars | Language: C++ | License: BSD-3-Clause | Last updated: Sept 16, 2026**

*Aerostack2 is a ROS 2 framework for building autonomous multi-aerial-robot systems — designed for modularity, Sim2Real deployment, and swarming orientation. Currently developed and tested on ROS 2 Humble (Ubuntu 22.04).*

**Recent Development Highlights:**
- **[as2_motion_controller] Add the geometric controller plugin** (`19c3973`, Sep 16, 2026, PR #1001) — by Rafael Perez-Segui; brand-new geometric controller for aerial platforms, enabling more precise trajectory tracking with provable stability guarantees
- **[as2_motion_controller] Plugin parameter contract and hover as a frozen reference** (`f049960`, Sep 16, 2026, PR #1000) — by Rafael Perez-Segui; formalizes the parameter interface for all motion controller plugins and establishes hover as a stable reference point — a foundational API contract
- **[as2_motion_controller] Yaw reference, PID library name and debug topics** (`05fa631`, Sep 16, 2026, PR #999) — by Rafael Perez-Segui; adds yaw-reference handling, standardizes PID library naming, and introduces debug topics for real-time tuning visualization
- **[as2_core] Fix getting latest transform with fixed frames** (`439ee79`, Sep 16, 2026, PR #996) — by Rafael Perez-Segui; resolves a TF2 bug where fixed-frame transforms returned stale data — critical for localization accuracy
- **fix: upgrade pixi-build-ros / pin ros2 distro mutex** (`82d85ab`, Sep 7, 2026, PR #997) — by Alvaro Gaona; CI infrastructure upgrade for reliable ROS 2 builds

**Key Architecture:** ROS 2 native (Humble), modular package ecosystem (as2_core, as2_motion_controller, as2_behavior_tree, as2_state_estimator, as2_hardware_drivers, as2_simulation_assets), behavior-tree-driven autonomy, swarming support, Sim2Real deployment pipeline, Python API bindings, Docker images on DockerHub, academic paper (arXiv:2303.18237).

**🎙️ Potential Episode Topics:**
- "Aerostack2: the ROS 2 framework for drone swarming"
- "Geometric controllers for drones: PR #1001 explained"
- "From hover to trajectory tracking: the motion controller architecture"
- "TF2 bugs that can crash your drone: the fixed-frame transform story"
- "Sim2Real: how Aerostack2 bridges simulation and the real world"
- "Behavior trees for aerial robots: modular autonomy without the spaghetti"

---

### 3. [argoverse/av2-api](https://github.com/argoverse/av2-api)
**⭐ 416 stars | Language: Python | License: MIT | Last updated: Sept 15, 2026**

*Argoverse 2 is the next-generation dataset and API for self-driving perception and forecasting — supporting 3D Object Detection, 4D Occupancy Forecasting, End-to-End Forecasting, Motion Forecasting, and Scenario Mining, plus the Trust-but-Verify Map Change Detection dataset.*

**Recent Development Highlights:**
- **Bump version to v0.3.6** (`b7321d1`, Feb 19, 2026, PR #334) — by Benjamin Wilson; latest stable release with all dataset APIs, scenario mining metrics, and evaluation tooling
- **Update Scenario Mining Evaluation** (`f0b2889`, Feb 19, 2026, PR #333) — by Cainan Davidson; refined scenario mining evaluation pipeline with improved metrics and benchmarking
- **Fix CI failures + package incompatibilities** (`529886a`, Feb 13, 2026, PR #331) — by Benjamin Wilson; critical CI repair resolving dependency conflicts and build breaks
- **Update scenario mining classification metrics from F1 to balanced accuracy** (`6b22766`, Jun 11, 2025, PR #315) — by Cainan Davidson; metric methodology shift — balanced accuracy better captures class imbalance in autonomous driving scenarios
- **Bump version** (`c06ecb7`, May 19, 2025, PR #314) — by Benjamin Wilson; maintenance release

**Key Architecture:** Python API with Rust extensions (Cargo.toml), Scene-level data access, 3D Object Detection, 3D Scene Flow, 4D Occupancy Forecasting, End-to-End Forecasting, Motion Forecasting, Scenario Mining, Map Change Detection (Trust-but-Verify), PyPI-distributed (`av2` package), NeurIPS Datasets & Benchmarks 2021 paper.

**🎙️ Potential Episode Topics:**
- "Argoverse 2: the dataset behind the future of self-driving perception"
- "From F1 to balanced accuracy: why metric choice matters in AV benchmarking"
- "Scenario mining: finding the edge cases that crash self-driving cars"
- "4D Occupancy Forecasting: predicting the future of every pixel in the scene"
- "Rust + Python: the hybrid architecture behind the av2 API"
- "Trust, but Verify: detecting when HD maps go stale in production AVs"

---

## 📊 Quick Comparison

| Project | Stars | Language | Focus | Latest Activity |
|---------|-------|----------|-------|-----------------|
| Autonomous OS | 347 | Python | Open-source robot OS with agentic AI & swappable skills | HAL speaker/drain lifecycle fixes, peripheral state management |
| Aerostack2 | 385 | C++ | ROS 2 framework for autonomous multi-aerial robots | Geometric controller plugin (#1001), parameter contracts, TF2 fix |
| Argoverse 2 API | 416 | Python | Self-driving perception & forecasting datasets | v0.3.6 release, scenario mining eval, CI fixes |

---

## 📋 Tracking Checklist

See the open issue **[Projects to Revisit & Upcoming Releases](https://github.com/bro26man-hash/robotics-oss-radar/issues/31)** for a detailed tracking checklist of these 3 projects.

## 🎙️ About This Project

This repo is a companion to our podcast on open-source robotics and autonomous systems. We track the most active GitHub projects, analyze their latest commits, and develop episode ideas — so listeners can follow along and contribute.

---

*Generated for the Robotics OSS Radar podcast. Stay curious, stay open-source.*
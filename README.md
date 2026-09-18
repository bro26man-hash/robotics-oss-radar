# 🤖 Robotics OSS Radar

> **Open-source robotics & autonomous systems radar** — tracking the most actively maintained open-source projects in robotics and autonomous driving. Curated for the *Robotics OSS Radar* podcast.

This is a living catalog of the most active, well-established open-source projects at the intersection of robotics and autonomous vehicles. Each entry includes recent commit highlights, key technical themes, and suggested podcast episode topics.

---

## 📡 Tracked Projects

### 1. 🚗 CARLA Simulator — `carla-simulator/carla`

| | |
|---|---|
| **Stars** | ⭐ 14,405 |
| **Language** | C++ / Python |
| **License** | MIT |
| **Last commit** | Sep 2, 2026 |
| **Repo** | [github.com/carla-simulator/carla](https://github.com/carla-simulator/carla) |

**What it is:** CARLA is an open-source simulator for autonomous driving research, developed from the ground up to support development, training, and validation of ADAS and autonomous driving stacks. It provides open digital assets (urban layouts, buildings, vehicles) and flexible sensor suite configuration.

**Recent development highlights:**

| Commit | What's Happening |
|---|---|
| `1360bb9` — Deploy UE5 nightly to Cloudflare R2 | **Infrastructure upgrade** — CARLA's Unreal Engine 5 nightlies are now served via Cloudflare R2, dramatically improving global download reliability and speed. |
| `dd3a9d7` — feat(sensor): add V2X sensor family (CAM, path-loss, CustomV2X, V2I) | **New sensor suite** — added a full **Vehicle-to-Everything (V2X)** sensor family, enabling communication-aware simulations. Huge for connected/autonomous vehicle research. |
| `39c4fda` — guard against null traffic light in WalkerManager | **Robustness fix** — WalkerManager no longer crashes when traffic light entities are missing in scenarios. |
| `0a5ce0d` — Fix lidar smoke helper signature | **Bug fix** — resolves lidar point-cloud visualization issue in debug sessions. |
| `6279162` — add CARLA_MAPS_TO_COOK to select packaged maps | **Build system improvement** — developers can now selectively cook packaged maps via CMake option, reducing build times for minimal installations. |

**🎙️ Potential Podcast Episode Topics:**
- *"V2X in Simulation: Why CARLA's New Sensor Family Changes Everything"* — How Vehicle-to-Everything simulation enables research into connected autonomy.
- *"From UE4 to UE5: The CARLA Graphics Overhaul"* — What migrating to Unreal Engine 5 means for photorealistic autonomous driving simulation.
- *"Cloudflare R2 vs. S3: How CARLA Scaled Global Downloads"* — Infrastructure choices for open-source projects with large binary assets.
- *"Sim-to-Real: Can CARLA's V2X Predictions Transfer to the Real World?"* — The simulation-to-reality gap, and whether V2X adds new capabilities or new uncertainties.

---

### 2. 🧭 Autoware — `autowarefoundation/autoware`

| | |
|---|---|
| **Stars** | ⭐ 12,067 |
| **Language** | C++ / Python (ROS 2) |
| **License** | Apache-2.0 |
| **Last commit** | Sep 16, 2026 |
| **Repo** | [github.com/autowarefoundation/autoware](https://github.com/autowarefoundation/autoware) |

**What it is:** Autoware is the world's leading open-source autonomous driving framework. It provides a comprehensive, production-ready software stack designed to accelerate commercial deployment of autonomous vehicles across diverse platforms and use cases. Built on ROS 2.

**Recent development highlights:**

| Commit | What's Happening |
|---|---|
| `a45f9ba` — managed_transform_buffer 0.3.0 updated | **Core library bump** — improved timestamp handling and buffer management, critical for multi-sensor fusion pipelines. |
| `79446c0` — CARLA 0.10 Town10HD_Opt map added to demo artifacts | **Simulation expansion** — the grand opt-in map for large-scale urban simulation is now available in Autoware's demo setup. |
| `87f7b60` — fix(docker): build simple planning simulator with core | **CI fix** — the simulation subpackage now compiles correctly inside the Docker image, removing a major CI bottleneck. |
| `3354a27` — pin CasADi to 3.7.2 for Humble ARM64 | **Edge-computing enablement** — resolves a build-breaking dependency conflict on ARM64 Ubuntu, opening the door for deeper learning on edge hardware. |
| `c0a32e8` — ci(health-check): trim PR matrix to amd64 main legs | **CI maturity** — streamlining CI to reduce flake and noise, signalling a maturing release pipeline. |

**🎙️ Potential Podcast Episode Topics:**
- *"Autoware: The OS for Autonomous Vehicles — Can It Scale to Production?"*
- *"ROS 2 in the Real World: What Autoware's CI Changes Tell Us About Maturity"*
- *"Simulation Meets Reality: CARLA + Autoware Integration Workflows"*
- *"Arm64 Autonomous: Running Autoware on Edge Hardware"*

---

### 3. 🦾 Isaac Lab — `isaac-sim/IsaacLab`

| | |
|---|---|
| **Stars** | ⭐ 8,157 |
| **Language** | Python |
| **License** | BSD-3-Clause |
| **Last commit** | Sep 17, 2026 |
| **Repo** | [github.com/isaac-sim/IsaacLab](https://github.com/isaac-sim/IsaacLab) |

**What it is:** Isaac Lab is a GPU-accelerated, open-source framework designed to unify and simplify robotics research workflows — reinforcement learning, imitation learning, and motion planning. Built on NVIDIA Isaac Sim, it combines fast physics and sensor simulation for effective sim-to-real transfer.

**Recent development highlights:**

| Commit | What's Happening |
|---|---|
| `93d7bef` — Docs consolidation & tutorial repair | **Documentation overhaul** — asset and Docker guides merged into a single coherent page; tutorial examples fixed for 3.0. |
| `6941d59` — Fix Isaac Lab 3.0.0 RC1 package installation | **Release blocker removed** — hotfix ensuring the stable release candidate installs cleanly across Linux and Windows. |
| `e836331` — Fix operational-space feedback & task-frame consistency | **Critical bugfix** — ensures accurate feedback loops for multi-DOF manipulators and humanoid robots. |
| `0921d32` — Standalone demos complete health check after startup | **Race condition fix** — demo scripts now wait for full simulation initialization before running, eliminating flaky CI. |
| `24f61d9` — Update nightly image pull-request automation | **DevEx improvement** — automated build pipeline for nightly Docker images gets refinements for faster breaking-change feedback. |

**🎙️ Potential Podcast Episode Topics:**
- *"Isaac Lab 3.0: What's New in the Biggest Robotics Sim Release Yet"*
- *"GPU-Accelerated Robot Learning: Inside NVIDIA's Isaac Lab"*
- *"Sim-to-Real Transfer: From Isaac Lab to the Real World"*
- *"The Rise of GPU-Native Robotics Frameworks — Is This the Paradigm Shift?"*

---

## 📋 Episode Planning Checklist

| # | Project | Episode Idea | Status |
|---|---|---|---|
| 1 | CARLA | "V2X in Simulation: Why CARLA's New Sensor Family Changes Everything" | 🔴 Not started |
| 2 | CARLA | "From UE4 to UE5: The CARLA Graphics Overhaul" | 🔴 Not started |
| 3 | Autoware | "Autoware: The OS for Autonomous Vehicles — Can It Scale to Production?" | 🔴 Not started |
| 4 | Autoware | "ROS 2 in the Real World: What Autoware's CI Changes Tell Us" | 🔴 Not started |
| 5 | Isaac Lab | "Isaac Lab 3.0: What's New in the Biggest Robotics Sim Release Yet" | 🔴 Not started |
| 6 | Isaac Lab | "GPU-Accelerated Robot Learning: Inside NVIDIA's Isaac Lab" | 🔴 Not started |

---

## 🔗 Quick Links

- [CARLA Simulator](https://github.com/carla-simulator/carla)
- [Autoware](https://github.com/autowarefoundation/autoware)
- [Isaac Lab](https://github.com/isaac-sim/IsaacLab)

## 📌 How This Repo Works

This repo is a **living tracker** for the *Robotics OSS Radar* podcast. We:

1. **Monitor** the most active open-source robotics & autonomous-vehicle repos on GitHub.
2. **Log** recent commits and development highlights.
3. **Brainstorm** podcast episode topics tied to real code changes.
4. **Track** upcoming releases and milestones to revisit.

Contributions are welcome! Open an issue to suggest a new project or episode idea.

---

*Built for makers, by makers. 🛠️*
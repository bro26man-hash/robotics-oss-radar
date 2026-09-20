# 🤖 Robotics OSS Radar

> Open-source robotics & autonomous systems — tracking the most active projects, recent commits, and podcast episode ideas.

This repo is a living companion for the **Robotics OSS Radar** podcast. We monitor the hottest open-source projects in robotics and autonomous systems, summarize their latest development highlights, and brainstorm episode topics for each.

---

## 📡 Currently Tracked Projects

---

### 1. [isaac-sim/IsaacLab](https://github.com/isaac-sim/IsaacLab)

| | |
|---|---|
| ⭐ Stars | 8,170 |
| 🛠 Language | Python |
| 📜 License | BSD-3-Clause |
| 📝 Description | Unified framework for robot learning with multi-physics / renderer support |

**Latest Commits (as of Sep 20, 2026):**
- `[Tests] Speed up contributed environment CI (#7905)` — Optimizing CI pipelines for contributed environments
- `Bump PyTorch to 2.12 (#7674)` — Upgrading to the latest PyTorch for better performance & compatibility
- `Deprecate IO descriptors (#7042)` — Cleaning up legacy IO descriptor APIs
- `Handle near-singular operational-space control (#7903)` — Robustness fix for singular configurations in manipulator control
- `Name one removal release across all deprecation notices (#7840)` — Coordinating deprecation cycle across the codebase

**🔍 What's Being Worked On:**
IsaacLab is in the middle of a **major 3.0 release cycle** targeting Isaac Sim 6.1. The team is actively cleaning up deprecated APIs, upgrading core dependencies (PyTorch 2.12), and hardening the simulation engine — particularly around near-singular operational-space control for manipulators. CI performance optimizations show they're scaling for broader community contributions. The deprecation notices signal a well-planned API transition ahead.

**🎙️ Potential Episode Topics:**
- "IsaacLab 3.0: What's Changing in NVIDIA's Robot-Learning Framework"
- "PyTorch 2.12 & GPU-Accelerated Robotics — Why It Matters for Sim-to-Real"
- "Deprecation Cycles & API Stability: How NVIDIA Manages a 8K-Star Open-Source Project"
- "From Orbit to IsaacLab — The Evolution of NVIDIA's Robotics Simulation Stack"

---

### 2. [commaai/openpilot](https://github.com/commaai/openpilot)

| | |
|---|---|
| ⭐ Stars | 63,682 |
| 🛠 Language | Python |
| 📜 License | MIT |
| 📝 Description | openpilot is an operating system for robotics. Currently, it upgrades the driver assistance system on 300+ supported cars. |

**Latest Commits (as of Sep 19, 2026):**
- `cabana: generate dbc files during builds (#38974)` — Automating DBC file generation in the Cabana tuning toolchain
- `cabana: refine signal heatmap grid (#38964)` — Improving the signal visualization heatmap for CAN bus analysis
- `cabana: preserve activity with a brighter baseline (#38971)` — UI/UX enhancement for the Cabana interactive signal explorer
- `cabana: revert quiet signal brightness clamp (#38970)` — Addressing a UX regression in dark-mode signal display
- `cabana: brighten quiet signals in dark mode (#38969)` — Improving readability of low-amplitude CAN signals

**🔍 What's Being Worked On:**
The **Cabana** signal analysis and tuning tool is seeing heavy active development. Recent commits focus on automating DBC (Database CAN) file generation, refining signal heatmap visualizations, and iterating on the UI/UX experience — especially dark-mode readability for low-amplitude signals. This suggests comma.ai is doubling down on making low-level CAN signal inspection and vehicle tuning more accessible to the community.

**🎙️ Potential Episode Topics:**
- "Inside openpilot's Cabana Tool — How Community Members Tune CAN Signals"
- "From 300+ Cars to One OS: The openpilot Approach to Mass-Scale ADAS"
- "MIT vs. Apache: How Licensing Shapes the openpilot Ecosystem"
- "The Hidden World of CAN Bus Signals — What openpilot Sees That You Don't"

---

### 3. [carla-simulator/carla](https://github.com/carla-simulator/carla)

| | |
|---|---|
| ⭐ Stars | 14,410 |
| 🛠 Language | C++ |
| 📜 License | MIT |
| 📝 Description | Open-source simulator for autonomous driving research. |

**Latest Commits (as of Sep 2, 2026):**
- `Deploy UE5 nightly to Cloudflare R2 (#9859)` — Streamlining asset distribution via Cloudflare R2 storage
- `Fix lidar smoke helper signature (#9791)` — Bug fix in the LiDAR sensor smoke visualization helper
- `fix(nav): guard against null traffic light in WalkerManager (#9758)` — Robustness fix for pedestrian navigation
- `feat(sensor): add V2X sensor family — CAM service, path-loss, CustomV2X, V2I (#9757)` — Major new vehicle-to-everything sensor suite
- `feat(cmake): add CARLA_MAPS_TO_COOK to select packaged maps (#9800)` — Build-system improvement for map selection

**🔍 What's Being Worked On:**
CARLA is undergoing a major transition to **Unreal Engine 5.5 (the `ue5-dev` branch)**. The biggest recent addition is a **V2X (Vehicle-to-Everything) sensor family** — CAM service, path-loss modeling, CustomV2X, and V2I — which is a huge leap for simulating connected/autonomous vehicle communication. They're also deploying UE5 nightlies via Cloudflare R2 for faster global distribution, hardening WalkManager against null references, and improving the CMake build system for map selection.

**🎙️ Potential Episode Topics:**
- "CARLA's Leap to Unreal Engine 5.5 — What Sim Researchers Need to Know"
- "V2X Simulation Is Here: Inside CARLA's New Vehicle-to-Everything Sensor Suite"
- "Cloudflare R2 & the Future of Open-Source Simulator Distribution"
- "From Simulation to Reality: How CARLA Bridges the Sim-to-Real Gap"

---

## 🎙️ About This Podcast

**Robotics OSS Radar** is a podcast exploring the open-source projects powering the future of robotics and autonomous systems. Each episode dives into a tracked project — its architecture, its community, its latest breakthroughs, and what it means for the future of autonomous technology.

---

## 📋 Roadmap

See the open issue **[Projects to Revisit & Upcoming Releases](https://github.com/bro26man-hash/robotics-oss-radar/issues)** for a checklist of projects to track and potential episode plans.

---

## 🤝 Contributing

Pull requests and suggestions are welcome! To suggest a project:
1. Open an issue with the repo URL and a brief description of why it's interesting
2. Tag it with `project-suggestion`

---

## 📡 Sources

All project data is pulled from GitHub in real-time. Stars, commits, and metadata reflect the most recent snapshot.

---
*Built for the open-source robotics community. MIT Licensed.*

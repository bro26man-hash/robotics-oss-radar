# 🤖 Robotics OSS Radar

> Tracking the most active open-source robotics & autonomous vehicle projects — for our podcast.

## 📡 Top 3 Projects Under the Lens

---

### 1. [microsoft/AirSim](https://github.com/microsoft/AirSim)
**⭐ 18,490 stars | Language: C++ | License: MIT | Last updated: Sept 15, 2026**

*Open-source simulator for autonomous vehicles built on Unreal Engine / Unity, from Microsoft AI & Research. Supports drones, cars, and more — with software-in-the-loop (PX4 & ArduPilot) and hardware-in-the-loop capabilities.*

**Recent Development Highlights:**
- **PR #9836 — Pin GitHub Actions to full-length commit SHAs** (`1ca93f6`, Sept 15, 2026) — improved CI reproducibility and security by pinning all GitHub Actions to full commit SHAs
- **PR #9835 — Updated README** (`d109f0d`, June 28, 2026) — documentation refresh by maintainer Shital Shah
- **Stats & maintenance commits** (`0b2db65`, March 15, 2026) — ongoing repo hygiene
- Key recent features: ROS2 wrapper, Cinematographic Camera, API to list all assets, movetoGPS API, Optical flow camera, simSetKinematics API, light control & dynamic texture updates

**🎙️ Potential Episode Topics:**
- "Inside AirSim: how Microsoft's high-fidelity simulator is training the next generation of autonomous drones and cars"
- "ROS2 integration in AirSim — what's new and why it matters for the robotics community"
- "From simulation to reality: transfer learning workflows with AirSim's Python/C++ APIs"
- "The evolution of AirSim: sports cars, drones, and thefy investment challenge of maintaining a research simulator"

---

### 2. [carla-simulator/carla](https://github.com/carla-simulator/carla)
**⭐ 14,404 stars | Language: C++ | License: MIT | Last updated: Sept 2, 2026**

*Open-source simulator for autonomous driving research. Developed from the ground up to support development, training, and validation of autonomous driving systems with open digital assets (urban layouts, buildings, vehicles).*

**Recent Development Highlights:**
- **PR #9859 — Deploy UE5 nightly to Cloudflare R2** (`1360bb9`, Sept 2, 2026) — streamlined nightly asset distribution via Cloudflare R2 for faster global downloads
- **PR #9791 — Fix lidar smoke helper signature** (`0a5ce0d`, July 14, 2026) — sensor bugfix for lidar visualization
- **PR #9758 — Guard against null traffic light in WalkerManager** (`39c4fda`, July 14, 2026) — robustness fix for pedestrian simulation
- **PR #9757 — Add V2X sensor family** (`dd3a9d7`, July 13, 2026) — major new sensor suite: CAM service, path-loss, CustomV2X, V2I — enabling vehicle-to-everything communication simulation
- **PR #9800 — CARLA_MAPS_TO_COOK CMake option** (`6279162`, July 10, 2026) — packaging improvement for map selection
- Currently in active UE5.5 development branch with parallel UE4.26 support

**🎙️ Potential Episode Topics:**
- "CARLA's V2X sensor: why vehicle-to-everything simulation is the next big thing for AV testing"
- "From UE4 to UE5: the CARLA render engine migration and what it means for photorealistic training data"
- "How CARLA's open digital assets are democratizing autonomous driving research"
- "Inside the CARLA leaderboard: benchmarking the world's best autonomous driving stacks"

---

### 3. [rerun-io/rerun](https://github.com/rerun-io/rerun)
**⭐ 11,462 stars | Language: Rust | License: Apache-2.0 / MIT | Last updated: Sept 17, 2026**

*The data layer for physical AI — log, query, visualize, and stream to training on shared columnar storage built for multimodal data. SDKs in Python, Rust, and C++.*

**Recent Development Highlights:**
- **Release 0.38.1** (`5c524e9`, Sept 17, 2026) — latest stable release with bug fixes and improvements
- **LeRobot task text support** (`f57020d`, Sept 17, 2026) — `re_lerobot` now supports LeRobot task text written as `LargeUtf8`, expanding compatibility with the popular robotics dataset format
- **Dataset read retry logic** (`3f1659b`, Sept 17, 2026) — improved resilience by retrying dataset reads until the requested revision is promoted
- **Alpha release pipeline fixes** (`bef4e0b`, Sept 17, 2026) — CI/CD improvements for release hygiene
- **Agent skills package** — ships coding agent skills for AI-assisted Rerun development

**🎙️ Potential Episode Topics:**
- "Rerun: the columnar data layer that's replacing ad-hoc logging in robotics pipelines"
- "From Rviz to Rerun: why the robotics visualization stack is being rewritten in Rust"
- "LeRobot + Rerun: how open-source robot掀 data formats are converging"
- "Streaming multimodal data directly to training — the end of export jobs?"

---

## 📊 Quick Comparison

| Project | Stars | Language | Focus | Latest Activity |
|---------|-------|----------|-------|-----------------|
| AirSim | 18.5K | C++ | Autonomous Vehicle Simulation | CI/commits maintenance |
| CARLA | 14.4K | C++ | Autonomous Driving Simulator | V2X sensors, UE5 builds |
| Rerun | 11.5K | Rust | Robotics Data Visualization | Active releases, LeRobot support |

---

## 🎙️ About This Project

This repo is a companion to our podcast on open-source robotics and autonomous systems. We track the most active GitHub projects, analyze their latest commits, and develop episode ideas — so listeners can follow along and contribute.

---

*Generated for the Robotics OSS Radar podcast. Stay curious, stay open-source.*
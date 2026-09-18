# 🤖 Robotics OSS Radar

> **Open-Source Robotics & Autonomous Systems — Podcast Radar**
> Tracking the most actively developed open-source projects, their latest commits, and potential episode topics for the *Robotics OSS Radar* podcast.

---

## 🎙️ About This Project

This repo is the companion hub for the **Robotics OSS Radar** podcast — a show dedicated to the people, projects, and behind-the-scenes engineering driving open-source robotics and autonomous systems forward. Between episodes, we use this repo to **monitor, summarize, and spotlight** the repos that matter most.

---

## 📡 Tracked Projects

### 1. [commaai/openpilot](https://github.com/commaai/openpilot)
| | |
|---|---|
| ⭐ Stars | **63,679** |
| 🛠 Language | Python |
| 📜 License | MIT |
| 🔗 Repo | [github.com/commaai/openpilot](https://github.com/commaai/openpilot) |

**What it is:** An open-source operating system for robotics that upgrades the driver assistance system on **300+ supported cars**. It's the most-starred active robotics project on GitHub and a flagship example of real-world autonomous driving deployed at scale.

**Recent Development Highlights (as of Sept 18, 2026):**

| Commit | What's Happening |
|---|---|
| `d06711b` — *ui: prime menu (#38860)* | Full redesign of the Prime UI menu — improving driver-facing UX and usability |
| `c6d13eb` — *Cinque v3 (#38932)* | New vehicle hardware generation support (Cinque v3), expanding the 300+ car compatibility list |
| `9a95fdc` — *cabana: fix stale message size warnings (#38961)* | Bug fix in Cabana (the data replay tool) — improving diagnostic reliability |
| `c8d56a1` — *cabana: filter multiplexed signals in binary grid (#38960)* | Enhanced signal processing in the data analysis pipeline |
| `df7e0e5` — *Use upstream tinygrad disk tensors for model loading (#38956)* | Performance optimization — leveraging upstream tinygrad improvements for faster model loading |

**🎙️ Potential Episode Topics:**
- *"Inside openpilot: How 300+ Cars Run Open-Source Autonomous Driving"* — The architecture, safety model (ISO 26262), and how the panda security chip works
- *"From DIY to Deployment: The comma.ai Hardware Pipeline"* — comma four, comma three, and the new Cinque hardware generations
- *"Tinygrad & the Edge: Running Deep Models on Car Hardware"* — The model-loading optimization story and what it means for on-device inference
- *"Cabana & Data-Driven Development: Replaying the Real World"* — How comma.ai uses route replay and signal analysis to debug and improve models

---

### 2. [ApolloAuto/apollo](https://github.com/ApolloAuto/apollo)
| | |
|---|---|
| ⭐ Stars | **26,829** |
| 🛠 Language | C++ |
| 📜 License | Apache-2.0 |
| 🔗 Repo | [github.com/ApolloAuto/apollo](https://github.com/ApolloAuto/apollo) |

**What it is:** Baidu's **open autonomous driving platform** — a full-stack, end-to-end software framework for developing, testing, and deploying autonomous vehicles. From geo-fenced waypoint following (v1.0) to curb-to-curb urban driving (v5.5+) to large-scale functional deployment (v11.0), Apollo has been the leading open-source AV platform since 2017.

**Recent Development Highlights (as of Feb 27, 2026):**

| Commit | What's Happening |
|---|---|
| `539f546` — *feat: add Apollo 11.0 bev+occ* | 🚀 **Major release:** Apollo 11.0 introduces **BEV (Bird's Eye View) + OCC (Occupancy)** perception — a paradigm shift from camera/LiDAR-based 3D detection to top-down representation, aligning with the industry trend pioneered by Tesla and Waymo |
| `40c8a01` — *Merge PR #15762: recover_seyond_lidar_driver* | New **Seyond LiDAR driver** integration — expanding hardware support for next-generation LiDAR sensors |
| `6680288` / `995b75a` — *Seyond LiDAR driver config & docs* | Full documentation and configuration support for the new lidar sensor |
| `d53aa3d` — *docs: fix README - remove invalid build status badges* | Maintenance cleanup — keeping docs current |

**🎙️ Potential Episode Topics:**
- *"BEV & OCC: The Paradigm Shift in Autonomous Perception"* — Why Bird's Eye View + Occupancy networks are replacing traditional 3D object detection, and what Apollo 11.0 means for the field
- *"From Apollo 1.0 to 11.0: 9 Years of Open-Source AV"* — The full evolution story, from GPS waypoint following to large-scale functional deployment
- *"CyberRT: The Middleware That Powers a Platoon of Robotaxis"* — Deep dive into Apollo's real-time communication framework
- *"Sensors & the Software Stack: Integrating Next-Gen LiDAR"* — What it takes to add a new sensor to a production-grade AV platform

---

### 3. [microsoft/AirSim](https://github.com/microsoft/AirSim)
| | |
|---|---|
| ⭐ Stars | **18,492** |
| 🛠 Language | C++ |
| 📜 License | MIT |
| 🔗 Repo | [github.com/microsoft/AirSim](https://github.com/microsoft/AirSim) |

**What it is:** Microsoft Research's **open-source, high-fidelity simulator** for autonomous vehicles — built on Unreal Engine (with an experimental Unity release). It supports drones, cars, and more, with software-in-the-loop (PX4/ArduPilot) and hardware-in-the-loop simulation. It's the go-to platform for AI research in deep learning, computer vision, and reinforcement learning for autonomous systems.

**Recent Development Highlights (as of Sept 15, 2026):**

| Commit | What's Happening |
|---|---|
| `1ca93f6` — *Merge PR #9836: Pin GitHub Actions to full-length commit SHAs* | 🔒 **CI/CD hardening:** Pinning GitHub Actions to full-length commit SHAs — a security best practice that prevents supply-chain attacks via compromised upstream actions |
| `44f3f43` — *Pin GitHub Actions to full-length commit SHAs* | Same security improvement — demonstrates Microsoft's commitment to open-source security hygiene |
| `d109f0d` — *Updated README (June 28, 2026)* | Documentation refresh — keeping the project accessible to new researchers |
| Recent added features (from README "What's New") | ROS2 wrapper, Cinematographic Camera, Optical Flow Camera, moveToGPS API, multiple drone support in Unity, simSetKinematics API, dynamic texture/object control, light spawning & control |

**🎙️ Potential Episode Topics:**
- *"Sim-to-Real: How AirSim Bridges Simulation and the Physical World"* — The challenges of transfer learning and why simulation is the secret weapon behind modern autonomy
- *"Reinforcement Learning in Unreal: Training Drones That Fly"* — A practical walkthrough of using AirSim for RL experiments
- *"Why Security Hygiene Matters in Open Source (Even for Simulators)"* — The GitHub Actions pinning story and what it teaches about supply-chain security
- *"ROS2 Meets AirSim: The Integration That Changes Everything"* — How the new ROS2 wrapper opens up AirSim to the broader robotics ecosystem
- *"From Academic Paper to Industry Standard: The AirSim Story"* — The journey from a 2017 FSR paper to one of the most-cited robotics simulators

---

## 📋 Roadmap & Episode Planner

See the open issue **[Projects to Revisit & Upcoming Releases](https://github.com/bro26man-hash/robotics-oss-radar/issues)** for a living checklist of each project's milestones to track, upcoming releases to watch, and interview angles to explore.

---

## 🔧 How to Use This Repo

- **Browse the README above** for at-a-glance project summaries and episode ideas
- **Open issues** to suggest new projects, propose episode topics, or flag major upstream releases
- **PRs welcome** for additional project entries, commit analysis, or content improvements
- **RSS/Atom feeds** from each project's GitHub can be piped into the podcast production workflow

---

## 🎙️ Listen & Subscribe

*Robotics OSS Radar* — exploring the code, the people, and the machines that are making autonomous systems real.

| Platform | Link |
|---|---|
| 🌐 Website | _Coming soon_ |
| 📡 RSS | _Coming soon_ |
| 🐦 Twitter/X | @RoboticsOSSRadar |

---

*Built for the open-source robotics community. MIT License.*

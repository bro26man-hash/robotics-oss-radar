# 🤖 Robotics OSS Radar

> **Podcast companion for open-source robotics & autonomous systems**
> Tracking the most active GitHub projects, recent development highlights, and episode opportunities.

---

## 📡 What Is This?

**Robotics OSS Radar** is a podcast companion that monitors the most recently active open-source repositories in the robotics and autonomous-vehicles ecosystem. We track recent commits, highlight development trends, and generate episode ideas — so you never miss a story worth telling.

---

## 🔍 Current Radar: Top 3 Recently Active Projects

---

### 1. 🚗 commaai/openpilot — Open-Source Driver Assistance & Autonomous Driving

| Field | Detail |
|-------|--------|
| **Repo** | [`commaai/openpilot`](https://github.com/commaai/openpilot) |
| **Tag** | `robotics` |
| **Language** | Python, C++ |
| **⭐ Stars** | ~63,682 |
| **License** | GPLv3 |
| **Latest Commit** | `cabana: improve theme contrast` — **Sep 19, 2026** |

**What it does:** openpilot is an **open-source operating system for robotics**, currently focused on upgrading the driver assistance system on 300+ supported cars. It replaces stock ADAS with a vision-based, neural-network-driven system that handles acceleration, braking, and lane-keeping — all running on consumer hardware.

#### 📊 Recent Commit Activity

| Date | SHA | Change | Why It Matters |
|------|-----|--------|-----------------|
| Sep 19, 2026 | `2eee697` | **cabana: improve theme contrast (#38965)** | UI polish — improving the driver-facing interface for better readability and safety |
| Sep 19, 2026 | `5ae0da0` | **DM: Super Leicht Model (#38942)** | Core ML upgrade — a new lightweight model for the driver monitoring system, likely faster inference & lower power draw on edge devices |
| Sep 18, 2026 | `a395610` | **ui: allow delay of scroller start (#38958)** | UX refinement — smoother scrolling in the UI, reducing visual glitches during critical driving moments |

#### 🔑 Key Architecture Highlights
- **Vision-based perception:** Camera-only pipeline (no LiDAR/radar reliance) using neural networks for path planning
- **300+ car support:** Broad vehicle compatibility with community-contributed car interfaces
- **Edge-optimized ML:** Models tuned for on-device inference (NVIDIA Tegra, Qualcomm Snapdragon)
- **Driver Monitoring (DM):** Real-time drowsiness & distraction detection using the new "Super Leicht" model
- **Open & community-driven:** 1,000+ contributors; car interfaces contributed by owners
- **CI/CD at scale:** Daily merges, rapid iteration on both UI and core models

#### 🎙️ Potential Episode Topics
- *"How openpilot Teaches Your Car to Drive Themselves — 300+ Cars and Counting"*
- *"Super Leicht: The Lightweight Model Revolutionizing On-Device Driver Monitoring"*
- *"Vision-Only vs. Sensor Fusion: Why openpilot Chose Cameras"*
- *"From Hobbyist to 63K Stars: The Community Behind openpilot"*
- *"Driving on Edge: How openpilot Runs Neural Networks on Phone Chips"*

---

### 2. 🏗️ ApolloAuto/apollo — The Open Autonomous Driving Platform

| Field | Detail |
|-------|--------|
| **Repo** | [`ApolloAuto/apollo`](https://github.com/ApolloAuto/apollo) |
| **Tag** | `autonomous-vehicles` |
| **Language** | C++, Python |
| **⭐ Stars** | ~26,829 |
| **License** | Apache-2.0 |
| **Latest Commit** | `docs: fix README - remove invalid build status badges` — **Apr 16, 2026** |

**What it does:** Apollo is Baidu's **full-stack open autonomous driving platform**. It provides everything from hardware abstraction to perception, planning, and control — designed for developers building self-driving cars at scale. It's one of the most mature open-source AV stacks in production use.

#### 📊 Recent Commit Activity

| Date | SHA | Change | Why It Matters |
|------|-----|--------|-----------------|
| Apr 16, 2026 | `d53aa3d` | **docs: fix README — remove invalid build status badges** | Maintenance pass — cleaning up stale CI badges; signals a shift toward release-focused workflow |
| Feb 28, 2026 | `40c8a01` | **Merge PR #15762 — recover_seyond_lidar_driver** | LiDAR driver recovery — restoring support for Beyondlidar sensors, expanding hardware compatibility |
| Feb 27, 2026 | `539f546` | **feat: add Apollo 11.0 bev+occ** | Major release feature — Bird's-Eye View + Occupancy network for 3D scene understanding, a key step toward L4 autonomy |

#### 🔑 Key Architecture Highlights
- **Full-stack AV stack:** Perception → Prediction → Planning → Control, all open-source
- **BEV + OCC (v11.0):** Bird's-Eye View representation with 3D occupancy grids — the industry's leading approach for 3D scene reconstruction
- **Hardware-agnostic:** Supports multiple lidar, camera, and compute configurations
- **Simulation & data pipeline:** Integrated tools for data labeling, simulation, and testing
- **Industry-backed:** Used by Baidu's Robotaxi fleet (Apollo Go) — real production-grade code

#### 🎙️ Potential Episode Topics
- *"Apollo 11.0: What BEV + OCC Means for the Future of Autonomous Driving"*
- *"From Baidu's Robotaxi to Your Garage: The Apollo Open-Stack Story"*
- *"LiDAR Drivers & Sensor Recovery: The Unseen Complexity of AV Hardware"*
- *"Full-Stack vs. Stack-of-Stacks: Why Apollo Ships Everything"*
- *"The 26,000-Star AV Platform Nobody Talks About"*

---

### 3. 🎮 microsoft/AirSim — Open-Source Autonomous Vehicle Simulator

| Field | Detail |
|-------|--------|
| **Repo** | [`microsoft/AirSim`](https://github.com/microsoft/AirSim) |
| **Tag** | `autonomous-vehicles` |
| **Language** | C++, Python, Unreal Engine |
| **⭐ Stars** | ~18,499 |
| **License** | MIT |
| **Latest Commit** | `Merge PR #9836 — pin actions to full-length SHAs` — **Sep 15, 2026** |

**What it does:** AirSim is an **open-source simulator for autonomous vehicles** built on Unreal Engine and Unity, from Microsoft AI & Research. It provides photorealistic environments, realistic sensor simulations (cameras, LiDAR, IMU, GPS), and APIs for Python/C++ — making it the go-to platform for training and testing autonomous systems in simulation before deploying to the real world.

#### 📊 Recent Commit Activity

| Date | SHA | Change | Why It Matters |
|------|-----|--------|-----------------|
| Sep 15, 2026 | `1ca93f6` | **Merge PR #9836 — pin actions to full-length SHAs** | Security hardening — pinning GitHub Actions to full-length commit SHAs prevents dependency confusion attacks; critical for a project used in research & production |
| Aug 12, 2026 | `44f3f43` | **Pin GitHub Actions to full-length commit SHAs** | Follow-up security hardening — comprehensive supply-chain protection |
| Jun 28, 2026 | `d109f0d` | **Updated README** | Documentation refresh — likely adding new features or setup improvements |

#### 🔑 Key Architecture Highlights
- **Unreal Engine-powered:** Photorealistic rendering for realistic visual perception testing
- **Multi-sensor simulation:** Cameras, LiDAR, IMU, GPS, depth — all synchronized and configurable
- **Python & C++ APIs:** Easy integration with ML pipelines (PyTorch, TensorFlow ROS)
- **Pre-built environments:** Cities, racetracks, indoor spaces — ready to deploy
- **Multi-vehicle support:** Simulate fleets of robots/vehicles simultaneously
- **ROS integration:** Works seamlessly with the Robot Operating System
- **Actively maintained by Microsoft Research:** Still receiving security & feature updates after 5+ years

#### 🎙️ Potential Episode Topics
- *"Training Self-Driving Cars in a Video Game: Inside Microsoft's AirSim"*
- *"Why Simulation Is the Secret Weapon of Autonomous Systems"*
- *"From Unreal Engine to ROS: How AirSim Bridges Simulation & Reality"*
- *"Security in Open-Source Robotics: Microsoft's AirSim Supply-Chain Hardening"*
- *"18,000 Stars and Still Counting — The Simulator That Built a Generation of AV Researchers"*

---

## 📊 Radar Summary

| # | Project | Domain | Stars | Commit Cadence | Vibe |
|---|---------|--------|-------|-----------------|------|
| 1 | **openpilot** | Driver Assistance / AV | ~63.7K | **Daily** (3 commits in 2 days) | 🚗 Community & edge ML |
| 2 | **Apollo** | Full-Stack AV Platform | ~26.8K | Steady (monthly maintains) | 🏗️ Industry-grade & full-stack |
| 3 | **AirSim** | Autonomous Simulator | ~18.5K | Monthly (security & docs) | 🎮 Simulation & research |

---

## 🎙️ Episode Pipeline

| Priority | Project | Suggested Angle | Status |
|----------|---------|-------------------|--------|
| 🔴 **High** | openpilot | Community-driven ADAS — how 63K stars and 300 cars are changing driving | In progress |
| 🟡 **Medium** | Apollo | Full-stack AV from Baidu — BEV + OCC and the road to L4 | TBD |
| 🟡 **Medium** | AirSim | The simulator that makes robots before they hit the road | TBD |

---

## 📋 How to Contribute

This is a **living document**. To suggest a project or submit an episode idea:

1. Fork this repo
2. Add your candidate to the radar (follow the format above)
3. Open a PR with your suggestions
4. Or open an **Issue** with the `episode-suggestion` label

---

## 🔗 Useful Links

- [openpilot](https://github.com/commaai/openpilot) — Open-source driver assistance
- [Apollo (Baidu)](https://github.com/ApolloAuto/apollo) — Full-stack autonomous driving
- [AirSim (Microsoft)](https://github.com/microsoft/AirSim) — Autonomous vehicle simulator
- [CARLA Simulator](https://carla.org/) — Another great open-source AV simulator

---

*Built for the open-source robotics community. Licensed under MIT.*

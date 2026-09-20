# 🤖 Robotics OSS Radar

> *Spotlight on the most active open-source robotics & autonomous-vehicle projects — weekly commits, highlights, and episode ideas for the OSS Robotics podcast.*

---

## 📡 Tracked Projects

We monitor the top repos in the `robotics` and `autonomous-vehicles` topics, focusing on recent development activity and what's worth covering on the podcast.

---

### 1. 🚗 [ApolloAuto/apollo](https://github.com/ApolloAuto/apollo)

| | |
|---|---|
| **Stars** | 26,829 ⭐ |
| **Language** | C++ |
| **Topic** | Autonomous Driving |
| **Last Updated** | April 2026 |

**What it is:** Apollo is Baidu's open-source autonomous driving platform. It provides a complete stack — perception, planning, control, and simulation — for building self-driving systems.

**Recent Development Highlights:**

| Date | Commit | Highlights |
|------|--------|------------|
| Apr 2026 | `d53aa3d` | README cleanup — removed invalid build status badges (maintenance pass) |
| Feb 2026 | `40c8a01` | Recovered Seyond lidar driver — restores 3D lidar support for Apollo's perception pipeline |
| Feb 2026 | `539f546` | **Apollo 11.0 BEV + OCC** — major feature: Bird's-Eye-View perception with Occupancy-based Convexification for 3D scene understanding |

**🎙️ Potential Episode Topics:**
- *"BEV Perception in Practice — What Apollo 11.0's OCC Means for 3D Scene Understanding"*
- *"From LiDAR to L3: How Open-Source Stacks Are Accelerating the Shift to Autonomous Driving"*
- *"The Lidar Driver Comeback — Why Sensor Abstraction Matters in AV Pipelines"*

---

### 2. 🛞 [commaai/openpilot](https://github.com/commaai/openpilot)

| | |
|---|---|
| **Stars** | 63,682 ⭐ |
| **Language** | Python |
| **Topic** | Robotics / Driver Assistance |
| **Last Updated** | September 2026 (today!) |

**What it is:** openpilot is an open-source operating system for robotics. Its flagship product upgrades the driver-assistance system on 300+ supported cars — essentially making semi-autonomous driving accessible to everyone.

**Recent Development Highlights:**

| Date | Commit | Highlights |
|------|--------|------------|
| Sep 2026 | `1b1b60b` | **Cabana: DBC file generation during builds** — auto-generates DRD (Data Reference Description) files so car-specific CAN signal definitions are always up to date |
| Sep 2026 | `95ed021` | **Cabana: Signal heatmap grid refinement** — improved visualization of CAN signal activity for debugging and reverse-engineering new vehicles |
| Sep 2026 | `ea0afb6` | **Cabana: Brighter baseline activity preservation** — UI tweaks to keep signal activity visible even when the screen dims |

**🎙️ Potential Episode Topics:**
- *"Reverse-Engineering 300+ Cars — How openpilot's Cabana Tool Cracks the CAN Bus"*
- *"From Golden Project to OS: The comma.ai Philosophy on Building Robotics Software"*
- *"Can You Trust Open-Source ADAS? A Deep Dive into openpilot's Safety Model"*

---

### 3. 🌐 [microsoft/AirSim](https://github.com/microsoft/AirSim)

| | |
|---|---|
| **Stars** | 18,499 ⭐ |
| **Language** | C++ |
| **Topic** | Autonomous Vehicles / Simulation |
| **Last Updated** | September 2026 |

**What it is:** AirSim is Microsoft's open-source simulator for autonomous vehicles, built on Unreal Engine and Unity. It provides high-fidelity physics, computer vision, and lidar simulation for training and testing autonomous systems in virtual environments.

**Recent Development Highlights:**

| Date | Commit | Highlights |
|------|--------|------------|
| Sep 2026 | `1ca93f6` | Merged PR #9836 — pinned GitHub Actions to full-length commit SHAs (security hardening) |
| Aug 2026 | `44f3f43` | **Pin GitHub Actions to full-length SHAs** — prevents supply-chain attacks by avoiding mutable tag references |
| Jun 2026 | `d109f0d` | README update — refreshed documentation and setup instructions |

**🎙️ Potential Episode Topics:**
- *"Sim-to-Real in 2026 — How AirSim Is Bridging the Gap Between Virtual and Physical Robots"*
- *"Supply-Chain Security in Open-Source Simulation — Why Pinning Actions Matters"*
- *"Training Self-Driving Cars in Unreal Engine — The Tech Behind AirSim"*

---

## 📋 Upcoming Episode Pipeline

| Episode | Project | Status |
|---------|---------|--------|
| 1 | Apollo BEV + OCC deep-dive | 📝 Idea |
| 2 | Cabana & CAN reverse-engineering | 📝 Idea |
| 3 | Sim-to-real with AirSim | 📝 Idea |
| 4 | Open-source ADAS safety comparison (openpilot vs Apollo) | 🔜 Planned |
| 5 | LiDAR ecosystems in open-source AVs | 🔜 Planned |

---

## 🔗 Quick Links

- [Apollo Docs](https://pilot.apollo.ai/)
- [openpilot Docs](https://docs.comma.ai/)
- [AirSim Docs](https://microsoft.github.io/AirSim/)

---

*This radar is updated weekly. Star the repo to follow along!*
# 🤖 Robotics OSS Radar

> Open-source robotics & autonomous systems — tracking the most active repos, recent commits, and podcast episode ideas.

A living research hub curating the top open-source projects in robotics and autonomous driving, with development highlights and episode topics for the **Robotics OSS Radar** podcast.

---

## 🔍 Featured Projects

### 1. [commaai/openpilot](https://github.com/commaai/openpilot)
**Stars:** 63,682 · **Language:** Python · **License:** MIT

An open-source operating system for robotics that upgrades the driver assistance system on **300+ supported cars**. openpilot is the brain behind comma.ai's consumer-grade ADAS lineup (comma three, comma four, chestnut).

#### 📌 Recent Development Highlights (Sept 2026)
| Commit | What's Happening |
|---|---|
| `cabana: improve theme contrast` (#38965) | UI/UX polish — improving the visual theme contrast in the Cabana debugging interface |
| `DM: Super Leicht Model` (#38942) | New deep learning model variant — "Super Leicht" (German for "super light") suggests a lighter-weight perception/model architecture |
| `ui: allow delay of scroller start` (#38958) | UI feature allowing delayed scroller activation — likely for safer in-car display behavior |

#### 🎙️ Potential Episode Topics
- **"The Consumer-Grade Autonomy Playbook"** — How comma.ai built a 300+ car support ecosystem with an open-source stack
- **"Model Size vs. Safety"** — What the "Super Leicht" model tells us about the industry push toward efficient on-device inference
- **"UI/UX for Safety-Critical Systems"** — Why the scroller delay and theme contrast changes matter in a driving context
- **"From Research to Road: The ISO26262 Journey"** — openpilot's safety engineering practices

---

### 2. [ApolloAuto/apollo](https://github.com/ApolloAuto/apollo)
**Stars:** 26,829 · **Language:** C++ · **License:** Apache-2.0

Baidu's high-performance, flexible architecture for accelerating the development, testing, and deployment of autonomous vehicles. Apollo has evolved from waypoint following (v1.0) to full urban autonomous driving (v11.0) across multiple iterations.

#### 📌 Recent Development Highlights (2026)
| Commit | What's Happening |
|---|---|
| `feat: add Apollo 11.0 bev+occ` | **Major:** Apollo 11.0 introduces **BEV (Bird's Eye View) + OCC (Occupancy)** perception models — a significant architectural shift toward modern 3D scene understanding |
| `recover_seyond_lidar_driver` | Recovery fix for the Seyond LiDAR driver — hardware integration maintenance |
| `docs: fix README - remove invalid build status badges` | Documentation cleanup |

#### 🎙️ Potential Episode Topics
- **"From 1.0 to 11.0: Apollo's 10-Year Autonomy Journey"** — How Baidu's platform evolved from GPS waypoint following to BEV+OCC urban driving
- **"BEV + OCC: The New Perception Paradigm"** — What Bird's Eye View and Occupancy networks mean for the future of AV perception
- **"Open Source AV Platforms: Apollo vs. The World"** — Comparing Apollo with other stacks (and why open-source matters for industry adoption)
- **"The Hardware Story: LiDAR, Orin, and 4D Radar"** — Apollo 9.0's ARM/Orin support and 4D millimeter-wave radar integration

---

### 3. [microsoft/AirSim](https://github.com/microsoft/AirSim)
**Stars:** 18,499 · **Language:** C++ · **License:** MIT

Microsoft's open-source, cross-platform simulator for autonomous vehicles — built on Unreal Engine (with an experimental Unity release). AirSim supports drones, cars, and more, with software-in-the-loop (PX4, ArduPilot) and hardware-in-the-loop simulation. A staple of academic AI research for autonomous systems.

#### 📌 Recent Development Highlights (2026)
| Commit | What's Happening |
|---|---|
| `Pin GitHub Actions to full-length commit SHAs` (#9836) | **Security hardening** — pinning CI actions to full SHAs for supply-chain security |
| `updated README` | Documentation refresh |
| *Ongoing:* ROS2 wrapper, Cinematographic Camera, Optical Flow Camera, `movetoGPS` API, multi-drone Unity support | New features landed in recent PRs — see [README](https://github.com/microsoft/AirSim) for full list |

#### 🎙️ Potential Episode Topics
- **"Simulate This: Why AirSim Still Matters in the Age of Generative Simulators"** — The enduring value of Unreal Engine-based physical simulation
- **"From Simulation to Reality: Transfer Learning with AirSim"** — How researchers use AirSim for sim-to-real transfer with PX4/ArduPilot
- **"The Security Side of Open-Source CI"** — What pinning GitHub Actions to full SHAs means for supply-chain security in OSS robotics
- **"Multi-Drone, Multi-Engine: AirSim's Expanding Scope"** — Unity support, ROS2 integration, and the cinematographic camera for research-grade data collection

---

## 📊 Quick Comparison

| Dimension | openpilot | Apollo | AirSim |
|---|---|---|---|
| **Focus** | Consumer ADAS / FoV | Full-stack AV platform | Simulation & AI research |
| **Language** | Python | C++ | C++ |
| **Stars** | 63.7K | 26.8K | 18.5K |
| **License** | MIT | Apache-2.0 | MIT |
| **Hardware** | comma four device | By-wire vehicles + RTX GPU | ANY — drones, cars, PX4 |
| **Maturity** | Production (300+ cars) | 11 years, v11.0 | Research-grade |
| **Active?** | 🔥 Daily commits | 🟡 Monthly commits | 🟢 Recent updates |

---

## 🎙️ About the Podcast

**Robotics OSS Radar** is a podcast exploring the open-source projects that are quietly (and not so quietly) reshaping robotics and autonomous systems. Each episode dives into a project's codebase, community, and roadmap — because the future of autonomy is being built in the open.

---

## 📋 Tracking

See the **[Projects to Revisit & Upcoming Releases](https://github.com/bro26man-hash/robotics-oss-radar/issues)** issue for a checklist of featured projects to revisit and upcoming releases to track.

---

*Created for the Robotics OSS Radar podcast companion. Star this repo if you find it useful!*

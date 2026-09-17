# 🤖 Robotics OSS Radar

> Tracking the most active open-source robotics & autonomous vehicle projects — for our podcast.

## 📡 Top 3 Projects Under the Lens

---

### 1. [carla-simulator/carla](https://github.com/carla-simulator/carla)
**⭐ 14,404 stars | Language: C++ | License: MIT | Last updated: Sept 2026**

*Open-source simulator for autonomous driving research — developed from the ground up to support development, training, and validation of autonomous driving systems.*

**Recent Development Highlights:**
- **UE5 nightly deployed to Cloudflare R2** (`1360bb9`, Sept 2, 2026) — the Unreal Engine 5.5 version of CARLA is now readily accessible via cloud storage, lowering the barrier to entry for researchers
- **Lidar smoke helper signature fix** (`0a5ce0d`, July 14, 2026) — bug fix improving sensor simulation accuracy
- **Null traffic light guard in WalkerManager** (`39c4fda`, July 14, 2026) — critical safety fix preventing crashes when traffic light data is missing in scenarios
- Currently on the `ue5-dev` branch (Unreal Engine 5.5), with the `ue4-dev` branch (UE 4.26) maintained in parallel

**🎙️ Potential Episode Topics:**
- "CARLA goes UE5: how the latest simulator upgrade changes autonomous driving research"
- "Why sensor fidelity matters: inside CARLA's lidar and traffic light fixes"
- "Open-source simulators vs. proprietary tools — can CARLA compete with Waymo/Cruise's internal stacks?"
- "Building a self-driving car from scratch using CARLA's Python API"

---

### 2. [cyberbotics/webots](https://github.com/cyberbotics/webots)
**⭐ 4,634 stars | Language: C++ | License: Apache-2.0 | Last updated: Sept 2026**

*Webots provides a complete development environment to model, program, and simulate robots, vehicles, and mechanical systems — beginner-friendly and used in academia & industry worldwide.*

**Recent Development Highlights:**
- **Controller pose cache removal fix** (`d2ba706`, Sept 16, 2026) — recent bug fix ensuring accurate robot pose tracking during controller updates
- **Released version sync** (`777eee4`, Sept 12, 2026) — maintainer Olivier Michel synced the released branch, keeping stable builds aligned
- **Active CI/CD across all platforms** — nightly tests running on Linux, Windows, and macOS for both `master` and `develop` branches
- Originally designed at EPFL (1996), open-sourced in 2018, now commercially supported by Cyberbotics

**🎙️ Potential Episode Topics:**
- "From EPFL lab to industry: the 30-year journey of Webots"
- "How robot simulators bridge the gap between academia and real-world deployment"
- "Webots vs. Gazebo vs. Isaac Sim — choosing the right simulator for your robot project"
- "The business model behind open-source robotics software"

---

### 3. [leofan90/Awesome-World-Models](https://github.com/leofan90/Awesome-World-Models)
**⭐ 2,017 stars | Language: Python | License: BSD-3-Clause | Last updated: Sept 2026**

*A curated, continuously updated list of papers on World Models for General Video Generation, Embodied AI, and Autonomous Driving — the go-to knowledge hub for the hottest research frontier in robotics.*

**Recent Development Highlights:**
- **Automated arXiv paper ingestion** (`3e788af`, Sept 16, 2026) — the repo's automation pipeline just added 128+ new arXiv candidates, keeping the list current with the latest research
- **Reviewed world model papers added** (`5d81eb5`, Sept 16, 2026) — human-reviewed additions ensure quality alongside the automated pipeline
- **Rapidly growing corpus** — the list now covers foundational World Model papers through cutting-edge 2026 publications, including NVIDIA Cosmos, GAIA-2, SimWorld, and dozens of new models
- Key subsections: Foundation Models, Embodied AI, VLA, Autonomous Driving, Datasets & Benchmarks

**🎙️ Potential Episode Topics:**
- "World Models 101: why LeCun says they're the future of AI — and what they mean for robotics"
- "From NVIDIA Cosmos to GAIA-2: a tour of the open-source world model ecosystem"
- "Can world models replace simulation? The CARLA vs. learned-simulator debate"
- "Embodied AI's hidden dependency: how world model paper lists are shaping research directions"
- "The benchmark explosion: evaluating what world models can actually do"

---

## 📊 Quick Comparison

| Project | Stars | Language | Focus | Latest Activity |
|---------|-------|----------|-------|-----------------|
| CARLA | 14.4K | C++ | Autonomous Driving Simulator | UE5 migration, sensor fixes |
| Webots | 4.6K | C++ | Robot Simulation Platform | Bug fixes, release syncs |
| Awesome-World-Models | 2.0K | Python | Research Paper Curation | Daily arXiv auto-ingestion |

---

## 📋 Tracking Checklist

See the open issue **[Projects to Revisit & Upcoming Releases](https://github.com/bro26man-hash/robotics-oss-radar/issues/22)** for a detailed tracking checklist of these 3 projects.

## 🎙️ About This Project

This repo is a companion to our podcast on open-source robotics and autonomous systems. We track the most active GitHub projects, analyze their latest commits, and develop episode ideas — so listeners can follow along and contribute.

---

*Generated for the Robotics OSS Radar podcast. Stay curious, stay open-source.*
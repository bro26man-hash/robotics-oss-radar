# 🤖 Robotics OSS Radar

> Open-source robotics & autonomous systems — tracking the most active projects, recent commits, and podcast episode ideas.

This repo is a living companion for the **Robotics OSS Radar** podcast. We monitor the hottest open-source projects in robotics and autonomous systems, summarize their latest development highlights, and brainstorm episode topics for each.

---

## 📡 Currently Tracked Projects

### 1. [ApolloAuto/apollo](https://github.com/ApolloAuto/apollo)
| | |
|---|---|
| ⭐ Stars | 26,829 |
| 🛠 Language | C++ |
| 📜 License | Apache-2.0 |
| 📝 Description | An open autonomous driving platform |

**Latest Commits (as of Apr 16, 2026):**
- `docs: fix README - remove invalid build status badges` — Maintenance / documentation cleanup
- `Merge pull request #15762: recover_seyond_lidar_driver` — Recovering and merging a LiDAR driver integration
- `feat: add Apollo 11.0 bev+occ` — Introducing Bird's Eye View (BEV) and Occupancy (OCC) models for Apollo 11.0

**🔍 What's Being Worked On:**
Apollo 11.0 is on the horizon, bringing **BEV (Bird's Eye View) and OCC (Occupancy) perception models** — a major leap in 3D scene understanding for autonomous vehicles. There's also active work on recovering the SoliX/LiDAR driver, indicating ongoing hardware integration efforts. The platform continues to evolve toward large-scale functional autonomous vehicle deployment.

**🎙️ Potential Episode Topics:**
- "Apollo 11.0: BEV + OCC — How Baidu Is Pushing the Envelope on AV Perception"
- "From Apollo 1.0 to 11.0 — 10 Years of Open-Source Autonomous Driving"
- "LiDAR Driver Recovery & Hardware Integration Challenges in Open AV Stacks"

---

### 2. [carla-simulator/carla](https://github.com/carla-simulator/carla)
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

**🔍 What's Being Worked On:**
CARLA is undergoing a major transition to **Unreal Engine 5.5 (the `ue5-dev` branch)**. Recent work includes deploying UE5 nightlies via Cloudflare R2 for faster global distribution, fixing LiDAR sensor bugs, and hardening the WalkerManager against null traffic light references. The community is actively maintaining the UE4.26 branch while propulsion shifts to UE5.

**🎙️ Potential Episode Topics:**
- "CARLA's Leap to Unreal Engine 5.5 — What Sim Researchers Need to Know"
- "Cloudflare R2 & the Future of Open-Source Simulator Distribution"
- "From Simulation to Reality: How CARLA Bridges the Sim-to-Real Gap"

---

### 3. [AtsushiSakai/PythonRobotics](https://github.com/AtsushiSakai/PythonRobotics)
| | |
|---|---|
| ⭐ Stars | 30,544 |
| 🛠 Language | Python |
| 📜 License | MIT |
| 📝 Description | Python sample codes and textbook for robotics algorithms. |

**Latest Commits (as of Sep 2, 2026):**
- `build(deps): bump github/codeql-action from 4.37.4 to 4.37.9 (#1423)` — Security scanning dependency update
- `build(deps): bump ruff from 0.16.1 to 0.16.5 in /requirements (#1424)` — Linter toolchain upgrade
- `build(deps): bump scipy from 1.17.1 to 1.18.1 in /requirements (#1425)` — Scientific computing dependency bump

**🔍 What's Being Worked On:**
Recent activity is focused on **dependency maintenance and security** — CodeQL security scanning, ruff linter, and scipy upgrades. While the core algorithm library remains stable and educational, the project is keeping its toolchain modern and secure. This is a great example of how OSS educational projects maintain long-term health through automated dependency management.

**🎙️ Potential Episode Topics:**
- "PythonRobotics: The Textbook That Teaches a Generation of Roboticists"
- "Dependency Management as a Feature — Lessons from PythonRobotics"
- "From Kalman Filters to RRT*: Core Algorithms Every Robotics Engineer Should Know"

---

## 🎙️ About This Podcast

**Robotics OSS Radar** is a podcast exploring the open-source projects powering the future of robotics and autonomous systems. Each episode dives into a tracked project — its architecture, its community, its latest breakthroughs, and what it means for the future of autonomous technology.

---

## 📋 Roadmap

See the open issue **[Projects to Revisit & Upcoming Releases](https://github.com/bro26man-hash/robotics-oss-radar/issues/76)** for a checklist of projects to track and potential episode plans.

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
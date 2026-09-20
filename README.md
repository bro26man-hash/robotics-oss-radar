# 🤖 Robotics OSS Radar

> Open-source robotics & autonomous systems — tracking the most active projects, recent commits, and podcast episode ideas.

This repo is a living companion for the **Robotics OSS Radar** podcast. We monitor the hottest open-source projects in robotics and autonomous systems, summarize their latest development highlights, and brainstorm episode topics for each.

---

## 📡 Currently Tracked Projects

### 1. [commaai/openpilot](https://github.com/commaai/openpilot)
| | |
|---|---|
| ⭐ Stars | 63,682 |
| 🛠 Language | Python |
| 📜 License | MIT |
| 📝 Description | openpilot is an operating system for robotics. Currently, it upgrades the driver assistance system on 300+ supported cars. |

**Latest Commits (as of Sep 19, 2026):**
- `cabana: generate dbc files during builds` — Automating DBC file generation in the Cabana tuning toolchain
- `cabana: refine signal heatmap grid` — Improving the signal visualization heatmap for CAN bus analysis
- `cabana: preserve activity with a brighter baseline` — UI/UX enhancement for the Cabana interactive signal explorer

**🔍 What's Being Worked On:**
The **Cabana** signal analysis and tuning tool is seeing heavy active development. Recent commits focus on automating DBC (Database CAN) file generation, refining signal heatmap visualizations, and improving the UI/UX experience. This suggests comma.ai is doubling down on making low-level CAN signal inspection and vehicle tuning more accessible to the community.

**🎙️ Potential Episode Topics:**
- "Inside openpilot's Cabana Tool — How Community Members Tune CAN Signals"
- "From 300+ Cars to One OS: The openpilot Approach to Mass-Scale ADAS"
- "MIT vs. Apache: How Licensing Shapes the openpilot Ecosystem"

---

### 2. [ApolloAuto/apollo](https://github.com/ApolloAuto/apollo)
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
- "Apollo 11.0: BEV + OCC: How Baidu Is Pushing the Envelope on AV Perception"
- "From Apollo 1.0 to 11.0 — 10 Years of Open-Source Autonomous Driving"
- "LiDAR Driver Recovery & Hardware Integration Challenges in Open AV Stacks"

---

### 3. [carla-simulator/carla](https://github.com/carla-simulator/carla)
| | |
|---|---|
| ⭐ Stars | 14,410 |
| 🛠 Language | C++ |
| 📜 License | MIT |
| 📝 Description | Open-source simulator for autonomous driving research. |

**Latest Commits (as of Sep 2, 2026):**
- `Deploy UE5 nightly to Cloudflare R2` — Streamlining asset distribution via Cloudflare R2 storage
- `Fix lidar smoke helper signature` — Bug fix in the LiDAR sensor smoke visualization helper
- `fix(nav): guard against null traffic light in WalkerManager` — Robustness fix for pedestrian navigation

**🔍 What's Being Worked On:**
CARLA is undergoing a major transition to **Unreal Engine 5.5 (the `ue5-dev` branch)**. Recent work includes deploying UE5 nightlies via Cloudflare R2 for faster global distribution, fixing LiDAR sensor bugs, and hardening the WalkerManager against null traffic light references. The community is actively maintaining the UE4.26 branch while propulsion shifts to UE5.

**🎙️ Potential Episode Topics:**
- "CARLA's Leap to Unreal Engine 5.5 — What Sim Researchers Need to Know"
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

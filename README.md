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
| 📝 Description | openpilot is an operating system for robotics. Currently, it upgrades the driver assistance system on 300+ supported cars. |

**Latest Commits (as of Sep 19, 2026):**
- `1b1b60b` — cabana: generate dbc files during builds (#38974) — Automating DBC file generation in the Cabana tuning toolchain
- `95ed021` — cabana: refine signal heatmap grid (#38964) — Improving the signal visualization heatmap for CAN bus analysis
- `ea0afb6` — cabana: preserve activity with a brighter baseline (#38971) — UI/UX enhancement for the Cabana interactive signal explorer
- `680aa6f` — cabana: revert quiet signal brightness clamp (#38970) — Polish on signal brightness controls
- `d375e7f` — cabana: brighten quiet signals in dark mode (#38969) — Accessibility improvement for dark-mode signal inspection

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
| 📝 Description | An open autonomous driving platform |

**Latest Commits (as of Apr 16, 2026):**
- `d53aa3d` — docs: fix README - remove invalid build status badges — Maintenance / documentation cleanup
- `40c8a01` — Merge PR #15762: recover_seyond_lidar_driver — Recovering and merging a LiDAR driver integration
- `539f546` — feat: add Apollo 11.0 bev+occ — Introducing Bird's Eye View (BEV) and Occupancy (OCC) models for Apollo 11.0
- `6680288` — [doc]: update seyond lidar driver conf — Documentation for new LiDAR hardware support
- `995b75a` — [doc]: update seyond lidar driver readme — README updates for LiDAR integration docs

**🔍 What's Being Worked On:**
Apollo 11.0 is on the horizon, bringing **BEV (Bird's Eye View) and OCC (Occupancy) perception models** — a major leap in 3D scene understanding for autonomous vehicles. There's also active work on recovering the SoliX/LiDAR driver, indicating ongoing hardware integration efforts. The platform continues to evolve toward large-scale functional autonomous vehicle deployment.

**🎙️ Potential Episode Topics:**
- "Apollo 11.0: BEV + OCC — How Baidu Is Pushing the Envelope on AV Perception"
- "From Apollo 1.0 to 11.0 — 10 Years of Open-Source Autonomous Driving"
- "LiDAR Driver Recovery & Hardware Integration Challenges in Open AV Stacks"

---

### 3. [AtsushiSakai/PythonRobotics](https://github.com/AtsushiSakai/PythonRobotics)
| | |
|---|---|
| ⭐ Stars | 30,544 |
| 🛠 Language | Python |
| 📝 Description | Python sample codes and textbook for robotics algorithms. |

**Latest Commits (as of Sep 2, 2026):**
- `08b453a` — build(deps): bump github/codeql-action from 4.37.4 to 4.37.9 (#1423) — Security scanning dependency update
- `8c3f761` — build(deps): bump ruff from 0.16.1 to 0.16.5 in /requirements (#1424) — Linter version bump
- `069e0fb` — build(deps): bump scipy from 1.17.1 to 1.18.1 in /requirements (#1425) — Scientific computing dependency update
- `1fe4fb9` — build(deps): bump github/codeql-action from 4 to 4.37.4 (#1405) — Earlier security scanning update
- `99716a0` — build(deps): bump ruff from 0.15.16 to 0.16.1 in /requirements (#1406) — Earlier linter update

**🔍 What's Being Worked On:**
PythonRobotics is in **maintenance mode** — recent activity is almost entirely automated dependency bumps (dependabot) for codeql-action, ruff, and scipy. No new robotics algorithm content has been added recently. This is a well-established educational resource that's stable but not actively evolving new features. The dependabot activity does signal that the project is still being maintained and kept secure.

**🎙️ Potential Episode Topics:**
- "Why the Best Robotics Textbook is Also a Codebase — PythonRobotics Deep Dive"
- "From Textbook to Tutorial: How PythonRobotics Teaches 50+ Robotics Algorithms"
- "Maintenance Mode vs. Active Development: What Happens to OSS Edu Projects After They 'Arrive'?"

---

## 🎙️ About This Podcast

**Robotics OSS Radar** is a podcast exploring the open-source projects powering the future of robotics and autonomous systems. Each episode dives into a tracked project — its architecture, its community, its latest breakthroughs, and what it means for the future of autonomous technology.

---

## 📋 Roadmap

See the open issue **[Projects to Revisit & Upcoming Releases](https://github.com/bro26man-hash/robotics-oss-radar/issues/73)** for a checklist of projects to track and potential episode plans.

---

## 🤝 Contributing

Pull requests and suggestions are welcome! To suggest a project:
1. Open an issue with the repo URL and a brief description of why it's interesting
2. Tag it with `project-suggestion`

---

## 📡 Sources

All project data is pulled from GitHub in real-time. Stars, commits, and metadata reflect the most recent snapshot.

---

*Built for the open-source robotics community.*

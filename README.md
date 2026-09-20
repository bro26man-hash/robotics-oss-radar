# 🤖 Robotics OSS Radar

> Tracking the most active open-source robotics & autonomous-systems projects — with development highlights and podcast episode ideas.

---

## 📡 Top 3 Projects Under the Lens

Selected from the most recently active repos tagged `robotics` or `autonomous-vehicles` on GitHub (as of Sep 2026).

---

### 1. [commaai/openpilot](https://github.com/commaai/openpilot)
**Tag:** `robotics` · **Language:** Python · **Stars:** 63,694★

**What it is:** openpilot is an operating system for robotics — currently it upgrades the driver assistance system on 300+ supported cars. It's the most-starred open-source driving project in our radar and a cornerstone of the OE (open piloting) movement.

**Recent development highlights:**
- 🗓️ **Sep 20, 2026** — `cabana: resize heatmap and prevent signal clipping` (3b2a75a, @TreyMoen): Critical visualization fix — the signal heatmap now resizes properly and prevents signal clipping, ensuring that large CAN signal values don't get truncated in the UI.
- 🗓️ **Sep 19, 2026** — `cabana: generate dbc files during builds` (1b1b60b, @TreyMoen): Automates DBC file generation in the cabana debugging tool — critical for parsing CAN bus signals across 300+ supported vehicle variants without manual effort.
- 🗓️ **Sep 19, 2026** — `cabana: refine signal heatmap grid` (95ed021, @TreyMoen): Visualization upgrade for the signal heatmap, helping developers quickly identify which CAN signals are active and which are noisy.

🎙️ **Potential episode topics:**
- *"Open Piloting at Scale"* — How openpilot went from a weekend project to 300+ car support and what that means for the future of ADAS.
- *"The cabana Debugging Lifeline"* — Inside openpilot's tools that let developers and users see exactly what the car is thinking on the CAN bus.
- *"DBC Files & the CAN Bus Maze"* — Why automated signal parsing matters when you support hundreds of different car models.

---

### 2. [ApolloAuto/apollo](https://github.com/ApolloAuto/apollo)
**Tag:** `autonomous-vehicles` · **Language:** C++ · **Stars:** 26,830★

**What it is:** Apollo is Baidu's open autonomous driving platform — a full-stack solution covering perception, planning, control, and HD map infrastructure. It's one of the most mature open-source AV platforms, used by numerous research groups and companies worldwide.

**Recent development highlights:**
- 🗓️ **Apr 16, 2026** — `docs: fix README - remove invalid build status badges` (d53aa3d, @xiaoxinyu): Maintenance cleanup — removed stale CI badges from the README that were pointing to deleted or renamed branches, keeping documentation accurate.
- 🗓️ **Feb 28, 2026** — `Merge PR #15762: recover_seyond_lidar_driver` (40c8a01, @yuxin): Hardware support recovery — re-enabled a lidar driver for the beyond-series lidar units, expanding Apollo's sensor compatibility list.
- 🗓️ **Feb 27, 2026** — `feat: add Apollo 11.0 bev+occ` (539f546, @yuxin): Major feature release — Apollo 11.0 introduces Bird's-Eye-View (BEV) perception and Occupancy (OCC) modules, bringing modern 3D scene understanding to the platform.

🎙️ **Potential episode topics:**
- *"Apollo 11.0: BEV + Occupancy in an Open AV Stack"* — What does adding modern BEV perception and occupancy grids mean for an open-source platform that's been around for years?
- *"From Baidu Research to Industry Standard"* — How Apollo became the reference implementation for autonomous driving in China and beyond.
- *"Lidar Driver Recovery & Hardware Ecosystem"* — Why maintaining sensor driver support matters and the politics of hardware compatibility in open-source AV.

---

### 3. [AtsushiSakai/PythonRobotics](https://github.com/AtsushiSakai/PythonRobotics)
**Tag:** `robotics` · **Language:** Python · **Stars:** 30,555★

**What it is:** PythonRobotics is a textbook-style collection of Python sample codes covering core robotics algorithms — from kinematics and path planning to SLAM and computer vision. It's the go-to resource for students and researchers learning robotics fundamentals.

**Recent development highlights:**
- 🗓️ **Sep 2, 2026** — `build(deps): bump github/codeql-action from 4.37.4 to 4.37.9` (08b453a, @dependabot): Security hygiene — updated GitHub's code scanning action to the latest version for improved vulnerability detection across the codebase.
- 🗓️ **Sep 2, 2026** — `build(deps): bump ruff from 0.16.1 to 0.16.5` (8c3f761, @dependabot): Linting modernization — updated the Ruff linter for improved performance and new rules.
- 🗓️ **Sep 2, 2026** — `build(deps): bump scipy from 1.17.1 to 1.18.1` (069e0fb, @dependabot): Scientific computing upgrade — updated SciPy to the latest release, bringing performance improvements and new algorithms for the numerical routines used throughout the textbook.

🎙️ **Potential episode topics:**
- *"Why the Most Important Robotics Repo Has Almost No Commits"* — What does it mean when a 30k-star educational project is mostly dependency bumps? The quiet art of maintaining a textbook.
- *"PythonRobotics as a Gateway Drug to Robotics Engineering"* — How this textbook-style repo feeds the pipeline of future robotics engineers.
- *"From Textbook to Production: Can Educational Code Scale?"* — The tension between clean, pedagogical code and the messy reality of production robotics systems.

---

## 🎙️ About This Radar

This repo is the companion data source for the **Robotics OSS Radar** podcast — a show exploring the open-source projects shaping the future of autonomous systems and robotics. Each episode dives deep into one project, interviewing maintainers, walking through the code, and discussing what's coming next.

**Suggested episode cadence:**
| Week | Project | Theme |
|------|---------|-------|
| 1 | openpilot | Open Piloting at Scale & the CAN Bus Debugging Lifeline |
| 2 | Apollo | Apollo 11.0: BEV + Occupancy in an Open AV Stack |
| 3 | PythonRobotics | Why the Most Important Robotics Repo Has Almost No Commits |

---

## 🔧 How to Contribute

- Found a stale project? Open an issue with the repo URL and what you expected to see.
- Want your project featured? Submit a link and a 2-line description.
- Episode ideas? The issue tracker is the place.

---

## 📊 Radar Dashboard

| Project | Last Commit | Activity | Stars | Language |
|---------|-------------|----------|-------|----------|
| openpilot | Sep 20, 2026 | 🟢 Active (cabana heatmap fix + DBC automation) | 63,694★ | Python |
| Apollo | Apr 16, 2026 | 🟡 Moderate (README cleanup + Apollo 11.0 BEV+OCC) | 26,830★ | C++ |
| PythonRobotics | Sep 2, 2026 | 🟡 Maintenance (dependency bumps) | 30,555★ | Python |

---

*Built with 💡 and a lot of open-source love.*
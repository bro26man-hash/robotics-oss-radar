# 🤖 Robotics OSS Radar

> Tracking the most active open-source robotics & autonomous-systems projects — with development highlights and podcast episode ideas.

---

## 📡 Projects Under the Lens

### 1. [commaai/openpilot](https://github.com/commaai/openpilot)
**Tag:** `robotics` · **Language:** Python · **Stars:** 63,682★ · **Last commit:** Sep 19, 2026

**What it is:** openpilot is an operating system for robotics — currently it upgrades the driver assistance system on 300+ supported cars. It's the most-starred open-source project in our radar and a cornerstone of the OE (open piloting) movement.

**Recent development highlights:**
- 🗓️ **Sep 19, 2026** — `cabana: generate dbc files during builds` (1b1b60b, @TreyMoen): Automated DBC file generation in the cabana debugging tool — no more manual DBC builds, streamlining the CAN signal reverse-engineering workflow.
- 🗓️ **Sep 19, 2026** — `cabana: refine signal heatmap grid` (95ed021, @TreyMoen): Improved signal heatmap visualization for easier identification of relevant CAN signals during hardware bring-up.
- 🗓️ **Sep 19, 2026** — `cabana: preserve activity with a brighter baseline` (ea0afb6, @TreyMoen): UI contrast improvement for the cabana interface — critical for outdoor/garage visibility.

🎙️ **Potential episode topics:**
- *"Open Piloting at Scale"* — How openpilot went from a weekend project to 300+ car support and what that means for the future of ADAS.
- *"The Cabana Workbench"* — Inside openpilot's debugging tools that let developers and users see exactly what the car is thinking via CAN signals.
- *"DBCgen & the Reverse-Engineering Pipeline"* — How automated DBC generation is changing the game for third-party hardware integration.

---

### 2. [microsoft/AirSim](https://github.com/microsoft/AirSim)
**Tag:** `autonomous-vehicles` · **Language:** C++ · **Stars:** 18,499★ · **Last commit:** Sep 15, 2026

**What it is:** AirSim is an open-source simulator for autonomous vehicles built on Unreal Engine / Unity, from Microsoft AI & Research. It provides high-fidelity photorealistic environments, sensor simulation (camera, LiDAR, IMU), and API access for path planning, computer vision, and reinforcement learning research.

**Recent development highlights:**
- 🗓️ **Sep 15, 2026** — `Merge PR #9836: pin-actions` (1ca93f6, @ChrisGuagliano): Security hardening — pinned all GitHub Actions to full-length commit SHAs, eliminating supply-chain attack vectors from short-sha references.
- 🗓️ **Aug 12, 2026** — `Pin GitHub Actions to full-length commit SHAs` (44f3f43, @DanFiedler): Continued CI security posture improvement.
- 🗓️ **Jun 28, 2026** — `updated README` (d109f0d, @ShitalShah): Documentation refresh — improving onboarding experience for new researchers and contributors.

🎙️ **Potential episode topics:**
- *"Sim-to-Real: Why AirSim Still Matters"* — How high-fidelity simulation bridges the gap between synthetic training data and real-world autonomous driving.
- *"Security in Open-Source AV Tooling"* — The GitHub Actions pinning story: a case study in supply-chain security for simulation frameworks.
- *"Rebuilding AirSim for 2026"* — What it takes to maintain a years-old research simulator in the era of Ely Forge and neural renderers.

---

### 3. [AtsushiSakai/PythonRobotics](https://github.com/AtsushiSakai/PythonRobotics)
**Tag:** `robotics` · **Language:** Python · **Stars:** 30,544★ · **Last commit:** Sep 2, 2026

**What it is:** Python sample codes and textbook for robotics algorithms — covering localization, mapping, path planning, control, and more. It's the go-to educational resource for anyone learning robotics programming in Python.

**Recent development highlights:**
- 🗓️ **Sep 2, 2026** — `build(deps): bump github/codeql-action from 4.37.4 to 4.37.9` (08b453a, @dependabot): Security tooling kept current — the CodeQL action update ensures static analysis catches vulnerabilities as the codebase evolves.
- 🗓️ **Sep 2, 2026** — `build(deps): bump ruff from 0.16.1 to 0.16.5` (8c3f761, @dependabot): Linting toolchain updated — ruff 0.16.x brings new rules and performance improvements for the project's code quality pipeline.
- 🗓️ **Sep 2, 2026** — `build(deps): bump scipy from 1.17.1 to 1.18.1` (069e0fb, @dependabot): Core scientific dependency bumped — scipy 1.18.x includes performance optimizations for the numerical routines that underpin many robotics algorithms in the repo.

🎙️ **Potential episode topics:**
- *"Teaching Robots to Think in Python"* — How PythonRobotics makes algorithms like Kalman filters, RRT*, and PID control accessible to the next generation of roboticists.
- *"The Dependency Drain"* — What happens when your educational repo depends on the scientific Python ecosystem: a story about keeping up with numpy, scipy, and tooling churn.
- *"Code as Curriculum"* — Why reading working code is sometimes better than reading textbooks — and how PythonRobotics proves it.

---

## 🎙️ About This Radar

This repo is the companion data source for the **Robotics OSS Radar** podcast — a show exploring the open-source projects shaping the future of autonomous systems and robotics. Each episode dives deep into one project, interviewing maintainers, walking through the code, and discussing what's coming next.

**Suggested episode cadence:**
| Week | Project | Theme |
|------|---------|-------|
| 1 | openpilot | Open Piloting at Scale + Cabana Deep-Dive |
| 2 | AirSim | Sim-to-Real + Supply-Chain Security |
| 3 | PythonRobotics | Teaching Robots to Think in Python |

---

## 🔧 How to Contribute

- Found a stale project? Open an issue with the repo URL and what you expected to see.
- Want your project featured? Submit a link and a 2-line description.
- Episode ideas? The issue tracker is the place.

---

## 📊 Radar Dashboard

| Project | Last Commit | Activity | Stars | Language |
|---------|-------------|----------|-------|----------|
| openpilot | Sep 19, 2026 | 🟢 Very Active (cabana DBCgen + heatmap + UI) | 63,682★ | Python |
| AirSim | Sep 15, 2026 | 🟢 Active (GitHub Actions security hardening) | 18,499★ | C++ |
| PythonRobotics | Sep 2, 2026 | 🟢 Active (dependency bumps + security tooling) | 30,544★ | Python |

---

*Built with 💡 and a lot of open-source love.*
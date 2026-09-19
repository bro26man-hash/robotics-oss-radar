# 🤖 Robotics OSS Radar

> Tracking the most active open-source robotics & autonomous-systems projects — with development highlights and podcast episode ideas.

---

## 📡 Projects Under the Lens

### 1. [commaai/openpilot](https://github.com/commaai/openpilot)
**Tag:** `robotics` · **Language:** Python · **Stars:** 63,682★

**What it is:** openpilot is an operating system for robotics — currently it upgrades the driver assistance system on 300+ supported cars. It's the most-starred open-source project in our radar and a cornerstone of the OE (open piloting) movement.

**Recent development highlights:**
- 🗓️ **Sep 19, 2026** — `cabana: improve theme contrast` (2eee697, @TreyMoen): UI polish for the cabana debugging interface, improving readability in bright sunlight conditions.
- 🗓️ **Sep 19, 2026** — `DM: Super Leicht Model` (5ae0da0, @ZwX1616): A new "Super Leicht" (super light) model for the Decision Maker (DM), promising faster inference and lower compute overhead — critical for cost-sensitive hardware.
- 🗓️ **Sep 18, 2026** — `ui: allow delay of scroller start` (a395610, @stef): UX improvement to prevent UI scroll jitter on startup.

🎙️ **Potential episode topics:**
- *"Open Piloting at Scale"* — How openpilot went from a weekend project to 300+ car support and what that means for the future of ADAS.
- *"The Super Leicht Model"* — What does it mean to make autonomy "lighter"? Exploring model compression techniques for edge devices.
- *"Cabana & the Debugging Lifeline"* — Inside openpilot's tools that let developers and users see exactly what the car is thinking.

---

### 2. [ApolloAuto/apollo](https://github.com/ApolloAuto/apollo)
**Tag:** `autonomous-vehicles` · **Language:** C++ · **Stars:** 26,829★

**What it is:** Apollo is Baidu's open autonomous driving platform — a full-stack solution covering perception, planning, control, and HD map infrastructure. It's one of the earliest and most comprehensive open-source AV stacks.

**Recent development highlights:**
- 🗓️ **Apr 16, 2026** — `docs: fix README - remove invalid build status badges` (d53aa3d, @xiaoxinyu): Maintenance cleanup — removing stale CI badges, signaling a shift in their CI/CD pipeline.
- 🗓️ **Feb 28, 2026** — `Merge PR #15762: recover_seyond_lidar_driver` (40c8a01, @yuxin): Recovery of the "Seyond" lidar driver — bringing back support for a specific lidar hardware platform, indicating ongoing hardware ecosystem expansion.
- 🗓️ **Feb 27, 2026** — `feat: add Apollo 11.0 bev+occ` (539f546, @yuxin): Major feature drop — Apollo 11.0 introduces Bird's-Eye-View (BEV) and Occupancy (OCC) perception, aligning with the industry's shift from camera-only to multi-modal 3D perception.

🎙️ **Potential episode topics:**
- *"BEV + OCC: The Perception Revolution"* — Why Bird's-Eye-View and Occupancy networks are replacing traditional 3D object detectors, and how Apollo 11.0 implements them.
- *"From Apollo to Autonomy: 10 Years of Open AV"* — A retrospective on Baidu's Apollo platform and its influence on the open-source AV ecosystem.
- *"Lidar Driver Archaeology"* — Why maintaining hardware drivers matters and what happens when they break — a story of recovery and ecosystem fragility.

---

### 3. [AtsushiSakai/PythonRobotics](https://github.com/AtsushiSakai/PythonRobotics)
**Tag:** `robotics` · **Language:** Python · **Stars:** 30,544★

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
| 1 | openpilot | Open Piloting at Scale |
| 2 | Apollo | BEV + OCC: The Perception Revolution |
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
| openpilot | Sep 19, 2026 | 🟢 Active (UI polish + new DM model) | 63,682★ | Python |
| Apollo | Apr 16, 2026 | 🟡 Maintenance (docs cleanup + Apollo 11.0 BEV/OCC) | 26,829★ | C++ |
| PythonRobotics | Sep 2, 2026 | 🟢 Active (dependency bumps + security tooling) | 30,544★ | Python |

---

*Built with 💡 and a lot of open-source love.*

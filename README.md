# 🤖 Robotics OSS Radar

> **A podcast about open-source robotics and autonomous systems.**  
> This repo tracks the most actively developed open-source projects in robotics and autonomous vehicles, summarizes recent development highlights, and proposes podcast episode topics.

---

## 📡 Tracked Projects

We focus on repos that are:
- **Actively maintained** — committed to within the last few weeks
- **Community-driven** — significant stars, forks, and contributor activity
- **Impactful** — shaping the future of robotics, autonomy, or embodied AI

---

### 1. 🚗 [commaai/openpilot](https://github.com/commaai/openpilot)

| | |
|---|---|
| **Stars** | 63,672 ⭐ |
| **License** | MIT |
| **Language** | Python |
| **Last Activity** | September 17, 2026 |

**What it is:**  
openpilot is an open-source, operating-system-level driver assistance system. It upgrades the ADAS in 300+ supported cars, providing real-world autonomous driving capabilities on consumer hardware.

**Recent Development Highlights:**
- **AGNOS 19.8 release** — the latest operating system update for comma hardware, bringing improved driving models and safety features (commit `cab5343`, Sep 17)
- **UI/UX improvements** — removal of legacy question-mark placeholders and a new "not paired" bookmark alert for the comma four device (commits `bd176cb` & `4d9d1bc`, Sep 17)
- **Continuous safety testing** — ISO 26262-compliant safety model enforced in hardware (panda), with software-in-the-loop tests on every commit

**🔎 Potential Episode Topics:**
- "How openpilot turned your car into a self-driving vehicle — the engineering behind 300+ car support"
- "From comma one to comma four: the hardware journey of openpilot"
- "ISO 26262 and functional safety in open-source autonomous driving"
- "The comma.ai community: how crowdsourced data trains real driving models"

---

### 2. 🦾 [AtsushiSakai/PythonRobotics](https://github.com/AtsushiSakai/PythonRobotics)

| | |
|---|---|
| **Stars** | 30,531 ⭐ |
| **License** | MIT |
| **Language** | Python |
| **Last Activity** | September 2, 2026 |

**What it is:**  
A comprehensive Python textbook and code collection for robotics algorithms — covering localization, mapping, SLAM, path planning, path tracking, arm navigation, aerial navigation, and bipedal locomotion.

**Recent Development Highlights:**
- **Dependency upgrades** — Bumped GitHub CodeQL action (4.37.4 → 4.37.9), ruff (0.16.1 → 0.16.5), and SciPy (1.17.1 → 1.18.1) for security and stability (Sep 2)
- **Maintained educational quality** — the textbook documentation at [atsushisakai.github.io/PythonRobotics](https://atsushisakai.github.io/PythonRobotics/) remains actively hosted and linked
- **Broad algorithm coverage** — from EKF/PF/Histogram filters to RRT*, MPC, Frenet-frame trajectory generation, and drone/rocket landing

**🔎 Potential Episode Topics:**
- "Learning robotics from scratch with Python: the PythonRobotics textbook approach"
- "RRT* vs MPC vs Stanley: which path-planning algorithm should you use?"
- "From self-driving cars to quadrotors: the surprising breadth of PythonRobotics"
- "Why Python (not C++) dominates robotics education and prototyping"

---

### 3. 🌍 [Genesis-Embodied-AI/genesis-world](https://github.com/Genesis-Embodied-AI/genesis-world)

| | |
|---|---|
| **Stars** | 29,958 ⭐ |
| **License** | Apache-2.0 |
| **Language** | Python |
| **Last Activity** | September 16, 2026 |

**What it is:**  
A unified simulation platform for physical AI and embodied AI learning. Genesis World combines a multi-physics engine (Rigid, FEM, MPM, SPH, PBD), a photo-realistic renderer (Nyx), and a cross-platform compiler (Quadrants) behind a clean Python API. Previously known as **Genesis**.

**Recent Development Highlights:**
- **Bug fix for damped joints** — resolved energy injection when constraint solve exits with force residual, improving simulation accuracy (commit `c27875e`, Sep 16)
- **Kinematic tree refactor** — made the kinematic tree (not the entity) the unit for every rigid solver pass, enabling better modularity and performance (commit `453510e`, Sep 16)
- **CI for dependent repos** — production CI now runs for downstream projects, strengthening the ecosystem (commit `a4daa11`, Sep 15)
- **Multi-physics coupling** — new demos for cloth-on-rigid, sand wheels, SPH+MPM, and FEM+rigid interactions
- **Nyx renderer advances** — Gaussian splatting, multi-camera multi-environment setups, PBR materials, and object picking

**🔎 Potential Episode Topics:**
- "Genesis World: one simulator to rule them all — rigid, fluid, cloth, and more"
- "From Taichi to Quadrants: the open-source compiler revolution in robotics simulation"
- "Why physics simulation is the secret weapon for training real robots"
- "Nyx and Gaussian splatting: photorealistic rendering for robot perception research"

---

## 🎙️ Podcast Structure Ideas

| Segment | Description |
|---------|-------------|
| **Project Spotlight** | Deep dive into one tracked repo per episode |
| **Commit Commentary** | Walk through the latest real commits and explain what they mean |
| **Epicaster** | Find the intersection of these projects (e.g., simulation + driving) |

---

## 📋 Tracking Checklist

See the issue **[Projects to Revisit & Upcoming Releases](https://github.com/bro26man-hash/robotics-oss-radar/issues)** for the full tracking checklist with milestones and next-steps.

---

## 🤝 Contributing

- Suggest a project: open an issue
- Propose an episode: open a discussion
- Submit a PR: fix typos, add projects, or improve summaries

---

## 📜 License

This repo is released under the [MIT License](LICENSE). All tracked projects retain their own respective licenses.

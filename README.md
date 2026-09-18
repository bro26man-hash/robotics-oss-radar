# 🤖 Robotics OSS Radar

> **Open-Source Robotics & Autonomous Systems Podcast** — Tracking the projects, people, and trends shaping the future of self-driving tech, drones, and autonomous robots.

---

## 🎙️ About This Project

This repo is the companion hub for the **Robotics OSS Radar** podcast. We surface the most active, impactful, and intriguing open-source robotics projects on GitHub — and break down what's happening under the hood for builders, researchers, and enthusiasts.

---

## 📡 Featured Projects This Episode

### 1. 🚗 [Microsoft AirSim](https://github.com/microsoft/AirSim)
| | |
|---|---|
| **Stars** | ⭐ 18,492 |
| **Language** | C++ |
| **License** | MIT |
| **Last Active** | September 2026 |

**What it is:** A photo- and physics-realistic simulator for drones, cars, and more, built on Unreal Engine (with an experimental Unity release). Developed by Microsoft AI & Research, it supports software-in-the-loop (PX4, ArduPilot) and hardware-in-the-loop simulation, plus a platform-independent API for deep learning, computer vision, and reinforcement learning research.

**Recent Development Highlights:**
- **ROS2 wrapper** now available — bridging AirSim to the ROS2 ecosystem for seamless integration with autonomous stacks
- **Cinematographic Camera** PR — new camera modes for high-fidelity data capture, perfect for training perception models
- **`movetoGPS` API** and **`simSetKinematics` API** — expanded programmatic control for precise experiment reproducibility
- **Optical flow camera** support — enabling motion-estimation research directly in simulation
- **Multiple drone support in Unity** — scaling multi-agent experiments
- **Dynamic object texture control** and **light spawning/destruction API** — richer scene authoring

**🎙️ Potential Episode Topics:**
- *"Sim-to-Real: How AirSim Is Bridging the Gap Between Virtual and Physical Autonomy"*
- *"Why ROS2 Integration Changes Everything for Autonomous Vehicle Pipelines"*
- *"Training Perception Models with Cinematographic Cameras — A Deep Dive"*

---

### 2. 🐍 [PythonRobotics](https://github.com/AtsushiSakai/PythonRobotics)
| | |
|---|---|
| **Stars** | ⭐ 30,536 |
| **Language** | Python |
| **License** | MIT |
| **Last Active** | September 2026 |

**What it is:** The definitive Python textbook and code collection for robotics algorithms. Covers the full autonomy stack — localization, mapping, SLAM, path planning, path tracking, aerial navigation, and even bipedal locomotion — all in readable, minimal-dependency Python.

**Recent Development Highlights:**
- **Active dependabot maintenance** — regular bumps to CodeQL, ruff, scipy, and other core tooling keeping the project modern and secure
- **Python 3.13 support** — latest language features benefiting type hints and performance
- **New algorithms added:** Particle Swarm Optimization (PSO) for path planning, Nonlinear MPC with C-GMRES, LQR-RRT*, and Frenet-frame optimal trajectory generation
- **Enhanced testing infrastructure** — pytest with parallel execution and mypy type-checking across the entire codebase
- **Official documentation site** at [atsushisakai.github.io/PythonRobotics](https://atsushisakai.github.io/PythonRobotics/) with full mathematical derivations

**🎙️ Potential Episode Topics:**
- *"From Textbook to Production: How PythonRobotics Became the World's Most-Starred Robotics Repo"*
- *"SLAM for Everyone — Making Probabilistic Robotics Accessible with Python"*
- *"MPC vs. LQR: Practical Trajectory Optimization for Autonomous Vehicles"*

---

### 3. 🏗️ [LGSVL Simulator (SVL Simulator)](https://github.com/lgsvl/simulator)
| | |
|---|---|
| **Stars** | ⭐ 2,456 |
| **Language** | C# (Unity HDRP) |
| **License** | Custom (non-commercial) |
| **Last Active** | January 2022 (Sunsetted) |

**What it is:** An HDRP Unity-based multi-robot simulator for autonomous vehicle developers, originally built by LG Electronics America R&D Lab. Featured out-of-the-box integrations with **Autoware.auto** and **Baidu Apollo**, HD map generation, and high-fidelity sensor simulations (LiDAR, camera, GPS, CANBUS).

**⚠️ Important Note:** LG announced the **sunsetting of SVL Simulator** as of January 1, 2022. No further source code changes, bug fixes, or asset updates are planned. The code remains open-source on GitHub, and the community is free to fork and build upon it — with over **500 forks** already created.

**Recent Development Highlights (Historic):**
- **2D perception sensor ego-detection fix** — improving object recognition accuracy
- **GPS and CANBUS sensor type name corrections** — better standardization for Apollo integration
- **Developer Mode asset caching fix** — performance improvements for custom scene builds
- **F1Tenth NPC light layer trigger size fix** — more realistic pedestrian and traffic scenarios

**🎙️ Potential Episode Topics:**
- *"When Big Tech Walks Away: The Rise and Sunset of SVL Simulator"*
- *"Community Forks & Open-Source Lifelines — Can the Community Keep SVL Alive?"*
- *"Simulator Wars: AirSim vs. SVL vs. CARLA — A Head-to-Head Comparison"*

---

## 🗓️ Episode Planning Calendar

| Episode | Project | Status |
|---------|---------|--------|
| 1 | AirSim — Sim-to-Real & ROS2 | 📝 In Research |
| 2 | PythonRobotics — The Algorithms Behind Autonomy | 📝 In Research |
| 3 | SVL Simulator Sunset — What Happens When OSS Loses Its Champion | 📝 In Research |
| 4 | Viewer Request / Community Deep-Dive | 🔜 Up Next |

---

## 🤝 How to Contribute

We welcome contributions! Here's how you can help:

1. **Suggest projects** — Open an issue with a repo you think we should cover
2. **Share your build** — Record a demo using one of our featured projects and tag us
3. **Submit episode ideas** — Pitch a topic or guest
4. **Fix errors** — PRs for corrections in our show notes are always welcome

---

## ⭐ Starring

| Rank | Project | Stars |
|------|---------|-------|
| 🥇 | PythonRobotics | 30,536 |
| 🥈 | AirSim | 18,492 |
| 🥉 | SVL Simulator | 2,456 |

---

*"The future of autonomous systems is being built in the open. Let's cover it all."* 🤖🚀
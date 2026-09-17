# 🤖 Robotics OSS Radar

> Tracking the most active open-source robotics & autonomous vehicle projects — for our podcast.

## 📡 Top 3 Projects Under the Lens

---

### 1. [AtsushiSakai/PythonRobotics](https://github.com/AtsushiSakai/PythonRobotics)
**⭐ 30,533 stars | Language: Python | License: MIT | Last updated: Sept 17, 2026**

*Python sample codes and textbook for robotics algorithms. A comprehensive, educational code collection covering localization, mapping, SLAM, path planning, path tracking, arm navigation, aerial navigation, and bipedal locomotion — designed to be easy to read with minimum dependencies.*

**Recent Development Highlights:**
- **SciPy 1.18.1 dependency bump** (`069e0fb`, Sept 2, 2026) — staying current with the latest scientific Python ecosystem
- **Ruff 0.16.5 linter upgrade** (`8c3f761`, Sept 2, 2026) — improved code quality checks across the codebase
- **CodeQL 4.37.9 security scanning update** (`08b453a`, Sept 2, 2026) — continuous security posture improvement
- **Python 3.13 support** — latest Python version fully supported with active CI on Linux, macOS, and Windows
- **Ongoing documentation maintenance** — textbook at [atsushisakis.github.io/PythonRobotics](https://atsushisakai.github.io/PythonRobotics/) with animation GIFs hosted separately

**Key Modules:** EKF/PF/Histogram Filter localization, ICP & FastSLAM, Dijkstra/A*/D*/RRT*/LQR-RRT* planning, Stanley/MPC/LQR path tracking, arm navigation, drone 3D trajectory following, rocket-powered landing, bipedal inverted pendulum planner.

**🎙️ Potential Episode Topics:**
- "PythonRobotics: the textbook that teaches a generation of roboticists"
- "RRT* vs LQR-RRT*: choosing the right path planner for your robot"
- "From EKF to particle filters: how robots localize themselves"
- "Model Predictive Control in Python: a hands-on walkthrough"
- "Why minimum dependencies matter: the PythonRobotics philosophy"
- "SLAM from ICP to FastSLAM 1.0"

---

### 2. [microsoft/AirSim](https://github.com/microsoft/AirSim)
**⭐ 18,490 stars | Language: C++ | License: MIT | Last updated: Sept 17, 2026**

*Open-source simulator for autonomous vehicles built on Unreal Engine (with experimental Unity release). Supports drones, cars, PX4/ArduPilot flight controllers, software-in-loop and hardware-in-loop simulation. Developed by Microsoft AI & Research as a platform for deep learning, computer vision, and RL experiments.*

**Recent Development Highlights:**
- **GitHub Actions pinning to full-length SHAs** (`44f3f43`, Aug 12, 2026) — improved build reproducibility and supply-chain security
- **ROS2 wrapper** (PR #3976) — native ROS 2 integration expanding the simulator's reach in the robotics community
- **Cinematographic Camera** (PR #3949) — advanced camera API for high-fidelity visual data capture
- **Optical flow camera** (PR #3938) — new sensor modality for optical flow-based navigation experiments
- **simSetKinematics API** (PR #4066) — direct kinematic state control for more precise simulation experiments
- **Multiple drones in Unity** (PR #3128) — experimental Unity release now supports multi-drone scenarios
- **movetoGPS API** (PR #3746) — GPS-based positioning for realistic outdoor simulation workflows

**Key Features:** Unreal/Unity-based high-fidelity rendering, PX4 & ArduPilot SIT/HITL, Python/C++/C#/Java APIs, weather effects, Computer Vision mode, data logging for deep learning training, reinforced learning tutorials.

**🎙️ Potential Episode Topics:**
- "Inside AirSim: how Microsoft builds a virtual world for autonomous vehicles"
- "ROS 2 meets Unreal Engine: the new AirSim ROS2 wrapper explained"
- "Hardware-in-loop with PX4: from simulation to real flight"
- "Computer Vision mode: when you don't need physics, you need pixels"
- "Reinforcement learning in AirSim: training drones to fly"
- "Supply chain security in open-source robotics simulators"

---

### 3. [zhm-real/MotionPlanning](https://github.com/zhm-real/MotionPlanning)
**⭐ 2,743 stars | Language: Python | License: Not specified | Last updated: Sept 17, 2026**

*Motion planning algorithms commonly used on autonomous vehicles (path planning + path tracking). Implements Hybrid A*, Frenet Optimal Trajectory, H-OBCA (incomplete), and controllers including Pure Pursuit, Rear-Wheel Feedback, Stanley, LQR, and Linear MPC — with both simple car and car-pulling-trailers models.*

**Recent Development Highlights:**
- **README workflow format fix** (`7a6b43d`, Nov 18, 2020) — last documented code contribution; currently maintained as a reference/educational resource
- **Curated paper references** — links to key papers from Stanford, CMU, UC Berkeley, and ApolloAuto for every algorithm
- **Reeds-Shepp curves integration** — dependency on the companion [ReedsSheppCurves](https://github.com/zhm-real/ReedsSheppCurves) repo for curvature-continuous path generation
- **cvxpy optimization stack** — uses CVXPY for convex optimization in MPC and LQR controllers
- **Car-pulling-trailers model** — unique among educational repos, includes a bicycle+trailer vehicle model for more realistic planning scenarios

**Key Algorithms:** Hybrid A* (with continuation), Frenet Optimal Trajectory (dynamic street scenarios), H-OBCA (hierarchical optimization-based collision avoidance, incomplete), Pure Pursuit, Rear-Wheel Feedback, Stanley/Front-Wheel Feedback, LQR + PID, Linear MPC.

**🎙️ Potential Episode Topics:**
- "Hybrid A* vs Frenet: two philosophies for autonomous vehicle path planning"
- "What is H-OBCA? Hierarchical optimization for collision avoidance"
- "From Stanley to LQR: the evolution of path-tracking controllers"
- "Why the car-pulling-trailers model matters for realistic motion planning"
- "cvxpy and convex optimization: the hidden math behind MPC"
- "Educational open-source repos: the long-tail of robotics algorithm reference implementations"

---

## 📊 Quick Comparison

| Project | Stars | Language | Focus | Activity Status |
|---------|-------|----------|-------|-----------------|
| PythonRobotics | 30,533 | Python | Robotics algorithms textbook & code | Active (CI, deps, Python 3.13) |
| AirSim | 18,490 | C++ | Autonomous vehicle simulator (UE/Unity) | Active (PRs, ROS2, new APIs) |
| MotionPlanning | 2,743 | Python | Motion planning & path tracking | Reference (last code 2020, curated) |

---

## 📋 Tracking Checklist

See the open issue **[Projects to Revisit & Upcoming Releases](https://github.com/bro26man-hash/robotics-oss-radar/issues/28)** for a detailed tracking checklist of these 3 projects.

## 🎙️ About This Project

This repo is a companion to our podcast on open-source robotics and autonomous systems. We track the most active GitHub projects, analyze their latest commits, and develop episode ideas — so listeners can follow along and contribute.

---

*Generated for the Robotics OSS Radar podcast. Stay curious, stay open-source.*
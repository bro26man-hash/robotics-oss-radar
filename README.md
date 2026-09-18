# 🤖 Robotics OSS Radar

> Tracking the most active open-source robotics & autonomous vehicle projects — for our podcast.

## 📡 Top 3 Projects Under the Lens

---

### 1. [commaai/openpilot](https://github.com/commaai/openpilot)
**⭐ 63,675 stars | Language: Python | License: MIT | Last updated: Sept 17, 2026**

*openpilot is an operating system for robotics. Currently, it upgrades the driver assistance system in 300+ supported cars — turning every commodity sensor setup into an advanced driver-assistance system (ADAS).*

**Recent Development Highlights:**
- **Model chunking removed & LFS adopted for Chestnut releases** (`1328ace`, Sep 17, 2026, PR #38941) — by Harald Schäfer; streamlines model storage and release management using Git LFS, making CI faster and more reliable
- **Chestnut power test removed** (`7db7735`, Sep 17, 2026, PR #38943) — by Daniel Koepping; cleanup of deprecated power testing infrastructure for the new Chestnut hardware generation
- **modeld: 2× faster Chestnut build** (`cd1490a`, Sep 17, 2026, PR #38656) — by Adeeb Shihadeh; major performance optimization cutting model compilation time in half for the upcoming Chestnut release

**Key Architecture:** modeld (deep learning model runner), managerc (process manager), controls (actuator & state management), ui (React Native dashboard), boardd (CAN bus interface), panda (hardware security & CAN bridge), Chestnut hardware support, RAML-based release pipeline.

**🎙️ Potential Episode Topics:**
- "63K stars and 300+ cars: inside commaai's openpilot"
- "Chestnut is coming: 2× faster builds and LFS-based releases"
- "Why modeld matters: how openpilot runs neural nets on the edge"
- "panda and boardd: the hardware backbone of open-source ADAS"
- "From comma one to commodity hardware: the openpilot hardware saga"
- "UI polish as a feature: how small UX fixes move open-source forward"

---

### 2. [carla-simulator/carla](https://github.com/carla-simulator/carla)
**⭐ 14,405 stars | Language: C++ | License: MIT | Last updated: Sept 2, 2026**

*CARLA is an open-source simulator for autonomous driving research, developed from the ground up to support development, training, and validation of autonomous driving systems. It provides open digital assets (urban layouts, buildings, vehicles) and flexible sensor suites and environmental conditions. Currently on the `ue5-dev` branch for Unreal Engine 5.5.*

**Recent Development Highlights:**
- **Deploy UE5 nightly to Cloudflare R2** (`1360bb9`, Sep 2, 2026, PR #9859) — by germanros1987; automated nightly builds of the Unreal Engine 5.5 version are now deployed to Cloudflare R2, making the latest simulator builds easily accessible to the community worldwide
- **Fix lidar smoke helper signature** (`0a5ce0d`, Jul 14, 2026, PR #9791) — by Yin Li; bug fix for the LiDAR sensor smoke visualization helper, improving rendering accuracy for sensor simulation debug sessions
- **Fix nav: guard against null traffic light in WalkerManager** (`39c4fda`, Jul 14, 2026, PR #9758) — by Jesus Armando Anaya; null-safety guard in pedestrian navigation preventing crashes when traffic lights are missing in scenarios

**Key Architecture:** Unreal Engine 5.5 rendering pipeline, Python API for scenario scripting, ROS2 bridge for integration, sensor suites (LiDAR, camera, radar), WalkerManager for pedestrian simulation, traffic light and sign modeling, urban environment assets, Cloudflare R2 distribution for nightly builds.

**🎙️ Potential Episode Topics:**
- "CARLA: the open-source simulator powering autonomous driving research"
- "UE5 nightly builds: how CARLA ships cutting-edge graphics to the community"
- "LiDAR simulation in CARLA: how realistic is it?"
- "WalkerManager and traffic logic: simulating urban mobility"
- "CARLA + ROS2: bridging simulation and real-world stacks"
- "From CoRL'17 to UE5: the 9-year evolution of CARLA"
- "Cloudflare R2 vs. S3: infrastructure choices for repos with big binaries"

---

### 3. [isaac-sim/IsaacLab](https://github.com/isaac-sim/IsaacLab)
**⭐ 8,157 stars | Language: Python | License: BSD-3-Clause | Last updated: Sept 17, 2026**

*Isaac Lab is a GPU-accelerated, open-source framework designed to unify and simplify robotics research workflows — reinforcement learning, imitation learning, and motion planning. Built on NVIDIA Isaac Sim (currently v6.1), it combines fast physics and sensor simulation for sim-to-real transfer in robotics.*

**Recent Development Highlights:**
- **Docs: Consolidate asset and Docker guides and repair tutorial examples** (`93d7bef`, Sep 17, 2026, PR #7819) — by hujc; major documentation overhaul consolidating scattered asset guides and Docker setup into one place, plus fixing broken tutorial examples that were blocking new contributors
- **Fix Isaac Lab 3.0 RC1 package installation** (`6941d59`, Sep 17, 2026, PR #7874) — by Sheikh Dawood; critical fix for the 3.0 RC1 release package installation, unblocking users from trying the latest version
- **Fix operational-space feedback and task-frame consistency** (`e836331`, Sep 17, 2026, PR #7868) — by ooctipus; physics correctness fix for operational-space control feedback and task-frame consistency, essential for accurate robot control in simulation

**Key Architecture:** GPU-accelerated physics (PhysX, RTX), 16+ robot models (manipulators, quadrupeds, humanoids), 30+ ready-to-train RL environments, sensor simulation (RGB/depth/segmentation cameras, IMU, contact sensors, ray casters), supports RSL RL, SKRL, RL Games, Stable Baselines, multi-agent RL, cloud-distributed training, Isaac Sim 6.1 dependency.

**🎙️ Potential Episode Topics:**
- "Isaac Lab 3.0: NVIDIA's GPU-accelerated robot learning framework"
- "From Orbit to Isaac Lab: the evolution of a robotics simulator"
- "Sim-to-real transfer: how Isaac Lab bridges simulation and the real world"
- "Operational-space control: the physics math behind realistic robot movement"
- "30 environments, 16 robots: the scale of Isaac Lab"
- "Documentation as a feature: why Isaac Lab's doc overhaul matters"
- "Isaac Lab 3.0 RC1: what's new and what's broken"

---

## 📊 Quick Comparison

| Project | Stars | Language | Focus | Latest Activity |
|---------|-------|----------|-------|-----------------|
| openpilot | 63,675 | Python | Open-source ADAS OS for 300+ cars | Chestnut build optimization, LFS migration, UI fixes |
| CARLA | 14,405 | C++ | Open-source autonomous driving simulator (UE5.5) | UE5 nightly deployment, LiDAR fix, WalkerManager null-guard |
| Isaac Lab | 8,157 | Python | GPU-accelerated robot learning framework (Isaac Sim 6.1) | Docs overhaul, 3.0 RC1 install fix, operational-space control fix |

---

## 📋 Tracking Checklist

See the open issue **[Projects to Revisit & Upcoming Releases](https://github.com/bro26man-hash/robotics-oss-radar/issues/36)** for a detailed tracking checklist of these 3 projects.

## 🎙️ About This Project

This repo is a companion to our podcast on open-source robotics and autonomous systems. We track the most active GitHub projects, analyze their latest commits, and develop episode ideas — so listeners can follow along and contribute.

---

*Generated for the Robotics OSS Radar podcast. Stay curious, stay open-source.*
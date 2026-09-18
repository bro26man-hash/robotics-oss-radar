# 🤖 Robotics OSS Radar

> Tracking the most active open-source robotics & autonomous vehicle projects — for our podcast.

## 📡 Top 3 Projects Under the Lens

These three repos were selected as the most recently active, highest-impact open-source projects in the `autonomous-vehicles` and `robotics` topic spaces on GitHub (as of September 2026). Each is pushing real, substantive code changes weekly.

---

### 1. [commaai/openpilot](https://github.com/commaai/openpilot)
**⭐ 63,675 stars | Language: Python | License: MIT | Last updated: Sept 17, 2026**

*openpilot is an operating system for robotics. Currently, it upgrades the driver assistance system on 300+ supported cars.*

**Recent Development Highlights (latest commits — Sept 17, 2026):**
- **Remove model chunking / use LFS for Chestnut releases** (`1328ace`, PR #38941) — Harald Schäfer migrated model storage to Git LFS for the new Chestnut hardware platform, streamlining release artifacts
- **rm chestnut power test** (`7db7735`, PR #38943) — Daniel Koepping cleaned up a transient power test for the Chestnut device
- **modeld: 2× faster Chestnut build** (`cd1490a`, PR #38656) — Adeeb Shihadeh doubled the inference build speed for Chestnut's modeld, a major performance win for on-device vision pipelines
- **ui: remove question marks** (`bd176cb`, PR #38938) — Shane Smiskol cleaned up UI placeholders
- **ui: not-paired bookmark alert** (`4d9d1bc`, PR #38936) — stef added a UX alert when a bookmarked device isn't paired

**Key Architecture:** Modeld (deep perception), Controld (longitudinal/lateral control), Params (parameter management), Logd (logging), SD (streaming), UI (comma three/ four dashboard), Panda (secure CAN bus hardware). Supports 300+ cars via the comma three/four device and car harness.

**🎙️ Potential Episode Topics:**
- "openpilot at 63K stars: how a community-driven OS took on 300+ cars"
- "Chestnut is coming: what's new in openpilot's next hardware generation"
- "2× faster modeld: the engineering behind on-device vision speedups"
- "From comma three to Chestnut: hardware evolution in open-source driving"
- "LFS for models: how openpilot manages gigabyte-scale ML artifacts at scale"
- "The safety model: ISO 26262 compliance in an open-source Stack"

---

### 2. [carla-simulator/carla](https://github.com/carla-simulator/carla)
**⭐ 14,405 stars | Language: C++ | License: MIT | Last updated: Sept 17, 2026**

*Open-source simulator for autonomous driving research — developed from the ground up to support development, training, and validation of autonomous driving systems. Now running on Unreal Engine 5.5 with open digital assets, flexible sensor suites, and environmental conditions.*

**Recent Development Highlights (latest commits):**
- **Deploy UE5 nightly to Cloudflare R2** (`1360bb9`, Sep 2, 2026, PR #9859) — germanros1987 automated nightly builds to Cloudflare R2, making the bleeding-edge UE5 builds instantly downloadable for researchers worldwide
- **Fix lidar smoke helper signature** (`0a5ce0d`, Jul 14, 2026, PR #9791) — Yin Li corrected the lidar sensor helper signature, improving the accuracy of LiDAR point-cloud generation in the simulator
- **WalkerManager null traffic light guard** (`39c4fda`, Jul 14, 2026, PR #9758) — Jesus Armando Anaya added a defensive null-check in WalkerManager's traffic-light handling, preventing crashes when scenarios lack traffic lights
- **V2X sensor family** (`dd3a9d7`, Jul 13, 2026, PR #9757) — added CAM service, path-loss, CustomV2X, and V2I sensors — a major step toward connected-and-autonomous vehicle simulation
- **CARLA_MAPS_TO_COOK CMake option** (`6279162`, Jul 10, 2026, PR #9800) — Jesus Armando Anaya added a build-time toggle to select packaged maps, streamlining builds for different use cases

**Key Features:** UE5.5 high-fidelity rendering, open digital assets (urban layouts, buildings, vehicles), Python API, full sensor suite (camera, LiDAR, radar, IMU, V2X), WalkerManager for NPC traffic, ROS2 bridge, Driving Benchmarks, Scenario Runner, Cloudflare-hosted nightlies. Parallel UE5.5 and UE4.26 branches.

**🎙️ Potential Episode Topics:**
- "CARLA goes UE5.5: what's new in the latest simulation engine"
- "Why nightly builds matter: how CARLA democratizes access to cutting-edge simulation"
- "Lidar simulation done right: the smoke helper fix and sensor fidelity"
- "WalkerManager and safe navigation: defensive coding in autonomous simulators"
- "V2X is here: CARLA's new Vehicle-to-Everything sensor family"
- "ROS 2 meets CARLA: bridging simulation and real-world robotics stacks"
- "From CoRL'17 to now: the evolution of CARLA as an open research platform"

---

### 3. [isaac-sim/IsaacLab](https://github.com/isaac-sim/IsaacLab)
**⭐ 8,157 stars | Language: Python | License: BSD-3-Clause | Last updated: Sept 17, 2026**

*Isaac Lab is a GPU-accelerated, open-source framework designed to unify and simplify robotics research workflows — reinforcement learning, imitation learning, and motion planning. Built on NVIDIA Isaac Sim, it combines fast physics and sensor simulation for sim-to-real transfer.*

**Recent Development Highlights (latest commits — Sept 17, 2026):**
- **Docs: Consolidate asset & Docker guides, repair tutorial examples** (`93d7bef`, PR #7819) — hujc reorganized documentation, merging asset and Docker guides and fixing broken tutorial examples — a major usability improvement
- **Fix Isaac Lab 3.0 RC1 package installation** (`6941d59`, PR #7874) — Sheikh Dawood resolved installation issues for the 3.0 RC1 release, unblocking users from trying the latest features
- **Fix operational-space feedback & task-frame consistency** (`e836331`, PR #7868) — ooctipus fixed a fundamental bug in operational-space feedback control, ensuring correct task-frame behavior for manipulation tasks
- **Standalone demos: complete health check after startup** (`0921d32`, PR #7869) — ooctipus made standalone demos wait for the health check to complete, preventing race conditions on startup
- **Update nightly image PR automation** (`24f61d9`, PR #7867) — Kelly Guo refreshed the CI automation for nightly Docker images

**Key Features:** 16+ robot models (manipulators, quadrupeds, humanoids), 30+ ready-to-train environments, RSLgym/SKRL/RL Games/Stable Baselines integration, RTX-based sensors (RGB/depth/segmentation), IMU, contact sensors, ray casters, GPU-accelerated physics, cloud-distributed training, Isaac Sim 6.1 dependency.

**🎙️ Potential Episode Topics:**
- "Isaac Lab 3.0: the GPU-accelerated future of robot learning"
- "Sim-to-real transfer: how Isaac Lab bridges simulation and the real world"
- "Operational-space control: the math behind robot manipulation (and why it matters)"
- "30 environments, 16 robots: a tour of Isaac Lab's benchmark-ready setups"
- "Nightly builds and CI: how NVIDIA ships Isaac Lab at scale"
- "Isaac Lab vs. CARLA: two simulators, two approaches to autonomous systems research"
- "From Orbit to Isaac Lab: the evolution of NVIDIA's robotics simulation stack"

---

## 📊 Quick Comparison

| Project | Stars | Language | Focus | Latest Activity |
|---------|-------|----------|-------|-----------------|
| openpilot | 63,675 | Python | Open-source driving OS for 300+ cars | Chestnut HW prep, 2× modeld speedup, LFS migration |
| CARLA | 14,405 | C++ | Autonomous driving simulator (UE5.5) | V2X sensors, nightly builds, nav safety fixes |
| Isaac Lab | 8,157 | Python | GPU-accelerated robot learning framework | Isaac Sim 6.1, operational-space fix, docs overhaul |

---

## 📋 Tracking Checklist

See the open issue **[Projects to Revisit & Upcoming Releases](https://github.com/bro26man-hash/robotics-oss-radar/issues/29)** for a detailed tracking checklist of these 3 projects.

## 🎙️ About This Project

This repo is a companion to our podcast on open-source robotics and autonomous systems. We track the most active GitHub projects, analyze their latest commits, and develop episode ideas — so listeners can follow along and contribute.

---

*Generated for the Robotics OSS Radar podcast. Stay curious, stay open-source.*
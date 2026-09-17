# 🤖 Robotics OSS Radar

> Tracking the most active open-source robotics & autonomous vehicle projects — for our podcast.

## 📡 Top 3 Projects Under the Lens

---

### 1. [carla-simulator/carla](https://github.com/carla-simulator/carla)
**⭐ 14,405 stars | Language: C++ | License: MIT | Last updated: Sept 2026**

*Open-source simulator for autonomous driving research — developed from the ground up to support development, training, and validation of autonomous driving systems.*

**Recent Development Highlights:**
- **UE5 nightly deployed to Cloudflare R2** (`1360bb9`, Sept 2, 2026) — the Unreal Engine 5.5 version of CARLA is now readily accessible via cloud storage, lowering the barrier to entry for researchers
- **Lidar smoke helper signature fix** (`0a5ce0d`, July 14, 2026) — bug fix improving sensor simulation accuracy
- **Null traffic light guard in WalkerManager** (`39c4fda`, July 14, 2026) — critical safety fix preventing crashes when traffic light data is missing in scenarios
- **V2X sensor family added** (`dd3a9d7`, July 13, 2026) — new Vehicle-to-Everything sensor family (CAM service, path-loss, CustomV2X, V2I) enabling connected-autonomy research
- **CARLA_MAPS_TO_COOK CMake option** (`6279162`, July 10, 2026) — lets developers select packaged maps at build time, streamlining custom scenario setups
- Currently on the `ue5-dev` branch (Unreal Engine 5.5), with the `ue4-dev` branch (UE 4.26) maintained in parallel

**🎙️ Potential Episode Topics:**
- "CARLA goes UE5: how the latest simulator upgrade changes autonomous driving research"
- "Why sensor fidelity matters: inside CARLA's lidar and traffic light fixes"
- "V2X in simulation: why connected-autonomy research needs CARLA's new sensor family"
- "Open-source simulators vs. proprietary tools — can CARLA compete with Waymo/Cruise's internal stacks?"
- "Building a self-driving car from scratch using CARLA's Python API"

---

### 2. [autowarefoundation/autoware](https://github.com/autowarefoundation/autoware)
**⭐ 12,067 stars | Language: C++ / Docker | License: Apache-2.0 | Last updated: Sept 2026**

*Autoware — the world's leading open-source software project for autonomous driving. A full-stack AV stack enabling everything from sensing and perception to planning and control.*

**Recent Development Highlights:**
- **Managed transform buffer v0.3.0** (`a45f9ba`, Sept 16, 2026) — dependency update improving coordinate-frame transformation handling, critical for multi-sensor fusion
- **CARLA 0.10 Town10HD_Opt map added to demo artifacts** (`79446c0`, Sept 9, 2026) — high-definition map integration for more realistic simulation demos
- **Simple planning simulator build fix with core** (`87f7b60`, Sept 8, 2026) — CI/Docker fix ensuring the planning simulator builds correctly alongside core components
- **CasADi pinned to 3.7.2 for Humble ARM64** (`3354a27`, Sept 7, 2026) — dependency pin fix for ARM64 builds, improving accessibility for embedded/edge developers
- **CI health-check matrix trimmed** (`c0a32e8`, Sept 7, 2026) — build optimization reducing CI runtime by focusing on amd64 main legs

**🎙️ Potential Episode Topics:**
- "Inside Autoware: the full-stack open-source AV stack that's powering real-world deployments"
- "Why transform buffers matter: the hidden complexity of multi-sensor fusion"
- "From simulation to street: how Autoware bridges CARLA and real-world HD maps"
- "ARM64 and edge: can open-source AV stacks run on embedded hardware?"
- "The Autoware Foundation ecosystem — how managed repositories scale open-source AV development"

---

### 3. [ros-navigation/navigation2](https://github.com/ros-navigation/navigation2)
**⭐ 4,715 stars | Language: C++ | License: Apache-2.0 | Last updated: Sept 2026**

*ROS 2 Navigation Framework and System — the standard for autonomous mobile robot navigation in the ROS 2 ecosystem, used from research labs to warehouse robots.*

**Recent Development Highlights:**
- **Assisted Teleop lateral projection sign fix + unit tests** (`76b2d4d`, Sept 17, 2026) — critical bug fix ensuring correct lateral movement in teleop mode, plus new test coverage
- **MPPI cost clearing between optimization iterations** (`e9e77d6`, Sept 17, 2026) — fix preventing cost accumulation across iterations, improving path-planning stability
- **Missing fstream include fix in Nav2 panel** (`c8a2812`, Sept 17, 2026) — build fix for the GUI panel component
- **MPPI noise distribution refresh on reset** (`f1f8070`, Sept 16, 2026) — ensures stochastic planner resets properly between planning runs
- **Steep footprint edge cell fix** (`0e572ba`, Sept 16, 2026) — grid map fix preventing navigation failures on sharp obstacle edges

**🎙️ Potential Episode Topics:**
- "MPPI deep-dive: how Model Predictive Path Integral control is changing robot navigation"
- "The unsung heroes: bug fixes that prevent real-world robot crashes"
- "ROS 2 Navigation2 vs. custom stacks — why the standard matters"
- "From teleop to autonomy: the full stack of mobile robot development"
- "Testing the untestable: how unit tests are improving navigation reliability"

---

## 📊 Quick Comparison

| Project | Stars | Language | Focus | Latest Activity |
|---------|-------|----------|-------|-----------------|
| CARLA | 14.4K | C++ | Autonomous Driving Simulator | UE5 migration, V2X sensors, safety fixes |
| Autoware | 12.1K | C++/Docker | Full-Stack AV Software | Dependency updates, HD map integration, CI optimization |
| Nav2 | 4.7K | C++ | ROS 2 Robot Navigation | MPPI improvements, teleop fixes, grid map bug fixes |

---

## 📋 Tracking Checklist

See the open issue **[Projects to Revisit & Upcoming Releases](https://github.com/bro26man-hash/robotics-oss-radar/issues/22)** for a detailed tracking checklist of these 3 projects.

## 🎙️ About This Project

This repo is a companion to our podcast on open-source robotics and autonomous systems. We track the most active GitHub projects, analyze their latest commits, and develop episode ideas — so listeners can follow along and contribute.

---

*Generated for the Robotics OSS Radar podcast. Stay curious, stay open-source.*
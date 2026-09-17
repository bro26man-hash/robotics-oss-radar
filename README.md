# 🤖 Robotics OSS Radar

> Tracking the most active open-source robotics & autonomous vehicle projects — for our podcast.

## 📡 Top 3 Projects Under the Lens

---

### 1. [carla-simulator/carla](https://github.com/carla-simulator/carla)
**⭐ 14,405 stars | Language: C++ | License: MIT | Last updated: Sept 2026**

*Open-source simulator for autonomous driving research — developed from the ground up to support development, training, and validation of autonomous driving systems.*

**Recent Development Highlights:**
- **Deploy UE5 nightly to Cloudflare R2** (`1360bb9`, Sept 2, 2026) — the Unreal Engine 5.5 version of CARLA is now readily accessible via cloud storage, lowering the barrier to entry for researchers
- **Fix lidar smoke helper signature** (`0a5ce0d`, July 14, 2026) — bug fix improving sensor simulation accuracy for lidar data
- **Guard against null traffic light in WalkerManager** (`39c4fda`, July 14, 2026) — critical safety fix preventing crashes when traffic light data is missing in scenarios
- **V2X sensor family added** — new Vehicle-to-Everything sensor family (CAM service, path-loss, CustomV2X, V2I) enabling connected-autonomy research
- **CARLA_MAPS_TO_COOK CMake option** — lets developers select packaged maps at build time, streamlining custom scenario setups
- Currently on the `ue5-dev` branch (Unreal Engine 5.5), with the `ue4-dev` branch (UE 4.26) maintained in parallel

**🎙️ Potential Episode Topics:**
- "CARLA goes UE5: how the latest simulator upgrade changes autonomous driving research"
- "Why sensor fidelity matters: inside CARLA's lidar and traffic light fixes"
- "V2X in simulation: why connected-autonomy research needs CARLA's new sensor family"
- "Open-source simulators vs. proprietary tools — can CARLA compete with Waymo/Cruise's internal stacks?"
- "Building a self-driving car from scratch using CARLA's Python API"

---

### 2. [cyberbotics/webots](https://github.com/cyberbotics/webots)
**⭐ 4,635 stars | Language: C++ | License: Apache-2.0 | Last updated: Sept 2026**

*Webots — a fast, easy-to-use, open-source robot simulator with a complete physics engine, sensors models, and a wide range of robots. Used in research, education, and industry.*

**Recent Development Highlights:**
- **Fix controller pose cache removal** (`d2ba706`, Sept 16, 2026) — bug fix ensuring correct controller pose rendering, critical for accurate simulation feedback
- **Sync released branch** (`777eee4`, Sept 12, 2026) — major release sync, keeping the stable branch aligned with latest features and bug fixes
- **Merge master into released branch** (`a6f0361`, Sept 12, 2026) — ongoing stabilization ensuring the released version incorporates all critical updates
- Active release branch management — Webots maintains a disciplined branching strategy with regular syncs between master and released branches

**🎙️ Potential Episode Topics:**
- "Why Webots is the simulator you're not using (but should be)"
- "Inside Webots: how a commercial-grade physics engine powers open-source robotics research"
- "From classroom to research lab: Webots' dual identity in education and cutting-edge robotics"
- "The branching strategy that keeps Webots stable: released vs. master branches explained"
- "Webots vs. Gazebo vs. Isaac Sim — the great robot simulator showdown"

---

### 3. [ros-navigation/navigation2](https://github.com/ros-navigation/navigation2)
**⭐ 4,715 stars | Language: C++ | License: Apache-2.0 | Last updated: Sept 2026**

*ROS 2 Navigation Framework and System — the standard for autonomous mobile robot navigation in the ROS 2 ecosystem, used from research labs to warehouse robots.*

**Recent Development Highlights:**
- **Fix Assisted Teleop lateral projection sign + unit tests** (`76b2d4d`, Sept 17, 2026) — critical bug fix ensuring correct lateral movement in teleop mode, plus new test coverage preventing regressions
- **Clear MPPI costs between optimization iterations** (`e9e77d6`, Sept 17, 2026) — fix preventing cost accumulation across iterations, improving path-planning stability and repeatability
- **Fix missing fstream include in Nav2 panel** (`c8a2812`, Sept 17, 2026) — build fix for the GUI panel component
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
| Webots | 4.6K | C++ | Robot Simulation | Controller pose fixes, release branch sync |
| Nav2 | 4.7K | C++ | ROS 2 Robot Navigation | MPPI improvements, teleop fixes, grid map bug fixes |

---

## 📋 Tracking Checklist

See the open issue **[Projects to Revisit & Upcoming Releases](https://github.com/bro26man-hash/robotics-oss-radar/issues/22)** for a detailed tracking checklist of these 3 projects.

## 🎙️ About This Project

This repo is a companion to our podcast on open-source robotics and autonomous systems. We track the most active GitHub projects, analyze their latest commits, and develop episode ideas — so listeners can follow along and contribute.

---

*Generated for the Robotics OSS Radar podcast. Stay curious, stay open-source.*
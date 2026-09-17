# 🤖 Robotics OSS Radar

> Tracking the most active open-source robotics & autonomous vehicle projects — for our podcast.

## 📡 Top 3 Projects Under the Lens

---

### 1. [ApolloAuto/apollo](https://github.com/ApolloAuto/apollo)
**⭐ 26,829 stars | Language: C++ | License: Apache-2.0 | Last updated: Sept 17, 2026**

*An open autonomous driving platform — a high-performance, flexible architecture that accelerates the development, testing, and deployment of Autonomous Vehicles. From GPS waypoint following (v1.0) to curb-to-curb urban driving (v5.5+) to large-scale functional deployment (v11.0).*

**Recent Development Highlights:**
- **Apollo 11.0 BEV+OCC perception** (`539f546`, Feb 27, 2026) — new bird's-eye-view and occupancy-grid perception models for enhanced 3D scene understanding
- **Beyond Lidar driver recovery** (`40c8a01`, Feb 28, 2026) — PR #15762 restores and hardens the lidar driver pipeline for robust sensor data ingestion
- **README cleanup** (`d53aa3d`, Apr 16, 2026) — removed invalid build status badges, improving project credibility
- **Apollo 11.0 focus on large-scale deployment** — comprehensive upgrades to perception, localization, planning, and development toolchains; support for ARM/Orin architecture; 4D millimeter-wave radar integration; functional safety framework reinforcement
- **Apollo Studio & Data Pipeline** — introduced in v7.0, matured through v10/11 as a one-stop online development platform

**Key Modules:** Perception (BEV+OCC), Localization (HD maps, GPS/IMU), Prediction, Planning & Control (PnC), Decider, CyberRT middleware, Dreamview Plus visualization, Package management v2.0, Apollo Studio.

**🎙️ Potential Episode Topics:**
- "Apollo 11.0: from research to production — the BEV+OCC revolution"
- "Inside Baidu's Apollo: 11 versions of open-source autonomous driving"
- "Beyond Lidar: why sensor redundancy is the key to safe AVs"
- "Apollo Studio: the one-stop dev platform for autonomous driving"
- "What's new in Apollo 11.0 — ARM support, 4D radar, and functional safety"
- "Package management and plugin architecture: how Apollo scales for production"

---

### 2. [carla-simulator/carla](https://github.com/carla-simulator/carla)
**⭐ 14,405 stars | Language: C++ | License: MIT | Last updated: Sept 17, 2026**

*Open-source simulator for autonomous driving research — developed from the ground up to support development, training, and validation of autonomous driving systems. Now running on Unreal Engine 5.5 with open digital assets, flexible sensor suites, and environmental conditions.*

**Recent Development Highlights:**
- **UE5 nightly builds deployed to Cloudflare R2** (`1360bb9`, Sep 2, 2026, PR #9859) — streamlined distribution of nightly builds for the UE5.5 branch, making it easier for researchers to stay current
- **Lidar smoke helper signature fix** (`0a5ce0d`, Jul 14, 2026, PR #9791) — corrected the lidar sensor simulation helper, improving accuracy of LiDAR point-cloud generation
- **WalkerManager null traffic light guard** (`39c4fda`, Jul 14, 2026, PR #9758) — defensive fix preventing crashes when traffic lights are absent in navigation scenarios
- **UE5.5 branch active in parallel with UE4.26** — significant differences between versions; UE5.5 requires Ubuntu 22.04/24.04 or Windows 11
- **ROS2 bridge maintained** — continued support for connecting CARLA to ROS 2 ecosystems

**Key Features:** UE5.5-based high-fidelity rendering, open digital assets (urban layouts, buildings, vehicles), Python API, sensor suite (camera, LiDAR, radar, IMU), WalkerManager for NPC traffic, ROS2 bridge, Driving Benchmarks, Scenario Runner, Cloudflare-hosted nightlies.

**🎙️ Potential Episode Topics:**
- "CARLA goes UE5.5: what's new in the latest simulation engine"
- "Why nightly builds matter: how CARLA democratizes access to cutting-edge simulation"
- "Lidar simulation done right: the smoke helper fix and sensor fidelity"
- "WalkerManager and safe navigation: defensive coding in autonomous simulators"
- "ROS 2 meets CARLA: bridging simulation and real-world robotics stacks"
- "From CoRL'17 to now: the evolution of CARLA as an open research platform"

---

### 3. [autonomous-ai/autonomous-os](https://github.com/autonomous-ai/autonomous-os)
**⭐ 347 stars | Language: Python | License: Apache-2.0 | Last updated: Sept 17, 2026**

*The open-source operating system for robots — install it and your robot comes alive. An agentic reasoning stack with swappable engines (Hermes, Claude Code, OpenCode), a skill-based architecture, hardware abstraction layer (HAL), and a built-in learning loop that creates skills from experience.*

**Recent Development Highlights:**
- **Scene speaker mute/unmute fix** (`2a11eea`, Sep 17, 2026) — HAL fix to drain scene speaker mute state and restore scene-muted peripherals on wake, improving user experience
- **Branch merge for speaker fix** (`d0e158d`, Sep 17, 2026) — integration merge bringing the speaker mute/restoration fix into main
- **General update** (`98bdf6b`, Sep 17, 2026) — ongoing maintenance and feature updates
- **6 agentic runtimes behind AgentGateway** — Hermes, OpenClaw, PicoClaw, Codex, Claude Code, OpenCode — all swappable via a 76-method interface
- **13 robot capabilities** — audio, vision, sensing, presence, motion, light, display, expression, lifelike, media, connectivity, companion, system
- **Safety gate as pure function** — SAFETY.md defines bounds (brightness, quiet hours, speed) with no model in the loop

**Key Architecture:** Apps (web UI), Skills (markdown-defined behaviors), Agentic Runtime (6 engines), System Services (Go daemon on :5000), Realtime Voice (Gemini Live / OpenAI Realtime), HAL (hardware abstraction, :5001), Drivers (per-subsystem classes), Boards (JSON-matched hardware).

**🎙️ Potential Episode Topics:**
- "Autonomous OS: the 'Android' for robots — install it and they come alive"
- "Agentic runtimes compared: Hermes vs Claude Code vs OpenCode for robotics"
- "Why HAL matters: hardware abstraction as the foundation of robot OS"
- "Skills as markdown: the democratization of robot programming"
- "Safety first: how Autonomous OS puts bounds on AI-driven robots"
- "From Lamp to Reachy Mini: bringing autonomous OS to real hardware"

---

## 📊 Quick Comparison

| Project | Stars | Language | Focus | Activity Status |
|---------|-------|----------|-------|-----------------|
| Apollo | 26,829 | C++ | Full autonomous driving platform (v11.0) | Active (BEV+OCC, lidar recovery, ARM support) |
| CARLA | 14,405 | C++ | Autonomous driving simulator (UE5.5) | Active (nightly builds, sensor fixes, nav safety) |
| Autonomous OS | 347 | Python | Open-source OS for robots (agentic) | Active (HAL fixes, speaker restoration, runtime updates) |

---

## 📋 Tracking Checklist

See the open issue **[Projects to Revisit & Upcoming Releases](https://github.com/bro26man-hash/robotics-oss-radar/issues/29)** for a detailed tracking checklist of these 3 projects.

## 🎙️ About This Project

This repo is a companion to our podcast on open-source robotics and autonomous systems. We track the most active GitHub projects, analyze their latest commits, and develop episode ideas — so listeners can follow along and contribute.

---

*Generated for the Robotics OSS Radar podcast. Stay curious, stay open-source.*
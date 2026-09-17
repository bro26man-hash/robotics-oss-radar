# 🤖 Robotics OSS Radar

> Tracking the most active open-source robotics & autonomous vehicle projects — for our podcast.

## 📡 Top 3 Projects Under the Lens

---

### 1. [commaai/openpilot](https://github.com/commaai/openpilot)
**⭐ 63,671 stars | Language:** Python | **License:** MIT | **Last commit:** Sep 17, 2026

> openpilot is an operating system for robotics. Currently, it upgrades the driver assistance system on 300+ supported cars.

**Recent Development Highlights:**
- **UI Cleanup** (`bd176cb`, Sep 17, 2026) — Removed stray question-mark placeholders from the UI for a cleaner user experience.
- **Not-Paired Bookmark Alert** (`4d9d1bc`, Sep 17, 2026) — New alert when a device bookmark isn't paired, improving device management UX.
- **AGNOS 19.8 Release** (`cab5343`, Sep 17, 2026) — Latest on-device OS version shipped, continuing rapid release cadence.

**What's Being Worked On:** Active daily development focused on UI/UX polish, device pairing reliability, and on-device OS releases. The project ships multiple commits per day, indicating a very healthy and active codebase.

**Key Features:** Open-source driver assistance for 300+ car models, end-to-end ML pipeline, on-device inference, crowdsourced driving data.

**🎙️ Potential Episode Topics:**
- "From Driver-Assistance to Full OS: The openpilot Vision"
- "UI/UX in Safety-Critical Robotics Interfaces"
- "What AGNOS 19.8 Means for On-Device Robotics"
- "How openpilot Scales Across 300+ Car Models"

---

### 2. [ApolloAuto/apollo](https://github.com/ApolloAuto/apollo)
**⭐ 26,829 stars | Language:** C++ | **License:** Apache-2.0 | **Last commit:** Apr 16, 2026

> An open autonomous driving platform

**Recent Development Highlights:**
- **Apollo 11.0 BEV + OCC** (`539f546`, Feb 27, 2026) — Major feature release adding Bird's-Eye-View perception and Occupancy-based collision checking, pushing the frontier of 3D scene understanding.
- **LiDAR Driver Recovery** (`40c8a01`, Feb 28, 2026) — PR merged to recover and stabilize the LiDAR driver subsystem, signalling active sensor-stack maintenance.
- **README Documentation Cleanup** (`d53aa3d`, Apr 16, 2026) — Removed invalid build-status badges, focusing on accurate and maintainable documentation.

**What's Being Worked On:** Apollo 11.0 introduces BEV (Bird's-Eye-View) perception and OCC (Occupancy-based collision checking) — cutting-edge 3D scene understanding. The LiDAR driver recovery shows ongoing hardware abstraction layer maintenance. The project is in a maintenance phase with periodic major releases.

**Key Features:** BEV perception, OCC collision checking, multi-sensor fusion (LiDAR, camera, radar), HD map integration, planning & control stack.

**🎙️ Potential Episode Topics:**
- "BEV Perception: The New Paradigm for Autonomous Driving"
- "Apollo 11.0 — What's New in the Open-Source Stack?"
- "Sensor Reliability: Inside the LiDAR Driver Recovery"
- "From Apollo 8.0 to 11.0: How the Stack Has Evolved"

---

### 3. [carla-simulator/carla](https://github.com/carla-simulator/carla)
**⭐ 14,405 stars | Language:** C++ | **License:** MIT | **Last commit:** Sep 2, 2026

> Open-source simulator for autonomous driving research.

**Recent Development Highlights:**
- **UE5 Nightly on Cloudflare R2** (`1360bb9`, Sep 2, 2026) — Deployed an Unreal Engine 5 nightly build to Cloudflare R2, enabling researchers to pull the latest simulator builds faster and more reliably.
- **LiDAR Smoke Helper Fix** (`0a5ce0d`, Jul 14, 2026) — Patched a signature bug in the LiDAR smoke helper, improving simulation fidelity for sensor modeling.
- **WalkerManager Null Guard** (`39c4fda`, Jul 14, 2026) — Added null-traffic-light guards in the WalkerManager navigation module, hardening pedestrian-scenario simulations against crashes.

**What's Being Worked On:** CARLA is evolving its UE5 integration (deploying nightly builds via Cloudflare R2 for faster distribution), improving sensor simulation fidelity (LiDAR fixes), and hardening scenario stability (null-pointer guards in pedestrian AI). The project balances feature development with robustness improvements.

**Key Features:** UE5-based high-fidelity rendering, ROS integration, flexible API, weather/lighting control, pedestrian & traffic simulation, sensor modeling (LiDAR, camera, radar, IMU).

**🎙️ Potential Episode Topics:**
- "Sim-to-Real: How CARLA Bridges the Gap"
- "UE5 in Robotics Simulation — What's Changing?"
- "Defensive Coding in Simulators: Null Guards & Sensor Fixes"
- "Cloudflare R2 for Simulator Distribution — A New Model?"

---

## 📊 Quick Comparison

| Project | Stars | Language | Focus | Last Activity | Status |
|---------|-------|----------|-------|---------------|--------|
| openpilot | 63.7k | Python | Open-source driver assistance OS | Sep 2026 (daily) | 🟢 Very Active |
| Apollo | 26.8k | C++ | Autonomous driving platform | Apr 2026 (periodic) | 🟡 Maintenance |
| CARLA | 14.4k | C++ | Autonomous driving simulator | Sep 2026 (ongoing) | 🟢 Active |

---

## 📋 Tracking Checklist

See the open issue **[Projects to Revisit & Upcoming Releases](https://github.com/bro26man-hash/robotics-oss-radar/issues/28)** for a detailed tracking checklist of these 3 projects.

## 🎙️ About This Project

This repo is a companion to our podcast on open-source robotics and autonomous systems. We track the most active GitHub projects, analyze their latest commits, and develop episode ideas — so listeners can follow along and contribute.

---

*Generated for the Robotics OSS Radar podcast. Stay curious, stay open-source.*
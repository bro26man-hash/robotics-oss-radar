# 🤖 Robotics OSS Radar

> Tracking the most active open-source robotics & autonomous-vehicle projects. Weekly progress snapshots, development highlights, and podcast episode ideas.

---

## 🔍 Why This Project?

Open-source robotics and autonomous systems are evolving at breakneck speed. This repo is the backbone of our podcast **"Robotics OSS Radar"** — a weekly deep-dive into the projects shaping the future of autonomous machines. We track commits, highlight development trends, and translate technical progress into compelling episodes.

---

## 📡 Projects Under the Microscope

### 1. 🔵 [Rerun](https://github.com/rerun-io/rerun)

| | |
|---|---|
| **Stars** | ⭐ 11,472 |
| **Language** | Rust + Python + C++ |
| **License** | Apache-2.0 |
| **Focus** | Multimodal data visualization & streaming for physical AI |
| **Last Activity** | September 18, 2026 (multiple commits same day) |

**What it does:** Rerun is the data layer for physical AI. It ingests multi-rate, multimodal data (images, point clouds, transforms, time series, joint states, video) from robot logs, human-data rigs, sim, and web video. The built-in viewer renders everything in sync, in realtime — scrub episodes, compare sensors, watch CV pipelines run live. Data is queryable with dataframes or SQL, and streams directly into training.

**Recent Development Highlights:**
- 🔦 **Volume Raymarcher** — New volume rendering capability for 3D scalar field visualization (Gábor Gyebnár)
- 🤖 **LeRobot Import Diagnostics** — `re_lerobot`: Collect and categorize import warnings when migrating LeRobot datasets into Rerun (Eric Leijonmarck)
- 🏗️ **Logging Architecture Refactor** — Lifted `LogMsg`, `ArrowMsg` and friends out of `re_log_types` into a dedicated `re_log_msg` crate, improving modularity (Antoine Beyeler)
- 🔧 **Changeset Type System** — Added `misc` as a new changeset type, expanding the granular update tracking system (Jochen Görtler)
- 📦 **Build Pinning** — Pinned `hatchling` to `v1.30.1` for reproducible Python builds (Jochen Görtler)

**🎙️ Potential Episode Topics:**
- "The Data Layer for Physical AI — Why Rerun Could Replace Rviz"
- "Rust for Robotics: Building a Columnar Storage Engine for Multi-Rate Sensor Data"
- "From LeRobot to Rerun: The Challenge of Standardizing Robotics Dataset Formats"
- "Volume Rendering for Robot Perception: What's Inside the Black Box?"

---

### 2. 🟢 [Autoware](https://github.com/autowarefoundation/autoware)

| | |
|---|---|
| **Stars** | ⭐ 12,068 |
| **Language** | C++ + Dockerfile |
| **License** | Apache-2.0 |
| **Focus** | World's leading open-source autonomous driving framework |
| **Last Activity** | September 18, 2026 (latest commit) |

**What it does:** Autoware is the world's leading open-source autonomous driving framework. It provides a comprehensive, production-ready software stack designed to accelerate the commercial deployment of autonomous vehicles across diverse platforms and use cases. From perception and planning to control and simulation, it's the de facto standard for open-source AV development.

**Recent Development Highlights:**
- 🚀 **autoware_utils v1.11.0** — Minor update to the core utilities package, keeping downstream tools current (awf-autoware-bot)
- 🔄 **Managed Transform Buffer v0.3.0** — Updated the transform coordinate management library, critical for multi-sensor calibration (awf-autoware-bot)
- 🗺️ **CARLA 0.10 Town10HD_Opt Map** — Added the high-definition optronic Town10 map to demo artifacts, expanding simulation scenarios (Masaya Kataoka)
- 🐳 **Docker Build Fix** — Fixed the simple planning simulator build with core modules, improving CI reliability (Mete Fatih Cırıt)
- 🔒 **CasADi 3.7.2 Pin for Humble ARM64** — Resolved compatibility issues for ARM64 platforms, broadening hardware support (Mete Fatih Cırıt)

**🎙️ Potential Episode Topics:**
- "Autoware: The Open-Source Stack Powering the Future of Autonomous Driving"
- "ROS 2 in Production — How Autoware Manages 12K+ Lines of C++"
- "Sim-to-Real with CARLA: From Town10HD to the Real World"
- "Why Transform Buffers Matter: The Hidden Complexity of Multi-Sensor Calibration"

---

### 3. 🟣 [Isaac Lab](https://github.com/isaac-sim/IsaacLab)

| | |
|---|---|
| **Stars** | ⭐ 8,162 |
| **Language** | Python |
| **License** | BSD-3-Clause |
| **Focus** | GPU-accelerated robot learning framework (RL, imitation, motion planning) |
| **Last Activity** | September 18, 2026 (multiple commits same day) |

**What it does:** Isaac Lab is a GPU-accelerated, open-source framework designed to unify and simplify robotics research workflows — reinforcement learning, imitation learning, and motion planning. Built on NVIDIA Isaac Sim, it combines fast physics and sensor simulation (RTX-based cameras, LIDAR, contact sensors) for effective sim-to-real transfer. Supports 16+ robot models, 30+ ready-to-train environments, and multi-agent RL.

**Recent Development Highlights:**
- 🖥️ **Isaac Sim Image Bump (600fa643bb36)** — Updated the underlying simulation container to the latest Isaac Sim image, ensuring access to newest physics and rendering features (isaaclab-bot)
- 🔐 **Trusted Checkout Fix in Backport Workflow** — Secured the automated backport pipeline, preventing untrusted code from being merged into release branches (Kelly Guo)
- 📖 **Historical Documentation Build Fixes** — Resolved redirect issues in the docs, improving navigation for users referencing older API versions (Kelly Guo)
- ⏱️ **Arms Demo Smoke Timeout Increase** — Bumped the CI timeout for the arms demo smoke test, reducing flaky failures on slower hardware (Kelly Guo)
- 🍔 **Compiled Docs Menu Fix** — Fixed the hamburger menu in compiled documentation, improving mobile/responsive UX (Kelly Guo)

**🎙️ Potential Episode Topics:**
- "GPU-Accelerated Robot Learning: Inside Isaac Lab's Simulation Pipeline"
- "Sim-to-Real Transfer: Can You Trust a Simulation to Predict Real-World Behavior?"
- "From Orbit to Isaac Lab: The Evolution of NVIDIA's Robotics Framework"
- "Reinforcement Learning at Scale — Training 30+ Environments in Parallel"

---

## 📊 Activity Snapshot (as of September 18, 2026)

| Project | Stars | Language | Latest Commit | Key Theme |
|---------|-------|----------|---------------|-----------|
| Rerun | 11,472 | Rust | Volume raymarcher + architecture refactor | Data infrastructure & rendering |
| Autoware | 12,068 | C++ | ROS 2 Humble updates + CARLA maps | AV stack maturity & simulation |
| Isaac Lab | 8,162 | Python | Isaac Sim image bump + CI hardening | Sim-to-real & GPU acceleration |

---

## 🎙️ Podcast Alignment

Each project maps to a natural episode arc:

1. **Infrastructure Episode** → Rerun: "What happens under the hood when a robot logs 100 sensor streams?"
2. **Production Episode** → Autoware: "How does an open-source AV stack actually ship to production?"
3. **Simulation Episode** → Isaac Lab: "Is simulation the future of robot training?"

---

## 📋 Tracking

See the open issue **[Projects to Revisit & Upcoming Releases](#)** for the running checklist of items to revisit before the next episode cycle.

---

## 🤝 Contributing

Pull requests and suggestions are welcome! To propose a new project or episode topic:
1. Open an issue describing the project and why it matters
2. Tag it with `proposal` and `episode-topic`
3. The maintainers will review and add to the radar

## 📄 License

This project is open-source under the [MIT License](LICENSE).
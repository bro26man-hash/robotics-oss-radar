# 🤖 Robotics OSS Radar

> **Podcast companion for open-source robotics & autonomous systems**
> Tracking the most active GitHub projects, recent development highlights, and episode opportunities.

---

## 📡 What Is This?

**Robotics OSS Radar** is a podcast companion that monitors the most recently active open-source repositories in the robotics and autonomous-vehicles ecosystem. We track recent commits, highlight development trends, and generate episode ideas — so you never miss a story worth telling.

---

## 🔍 Current Radar: Top 3 Recently Active Projects

---

### 1. 🧠 PythonRobotics — Robotics Algorithms Textbook & Reference

| Field | Detail |
|-------|--------|
| **Repo** | [`AtsushiSakai/PythonRobotics`](https://github.com/AtsushiSakai/PythonRobotics) |
| **Tag** | `robotics` |
| **Language** | Python |
| **⭐ Stars** | 30,544 |
| **Latest Commit** | `08b453a` — **Sep 2, 2026** |
| **Activity Tier** | 🟢 Actively maintained |

**What it does:** PythonRobotics is a **comprehensive textbook and reference library** for robotics algorithms — covering everything from basic kinematics to advanced SLAM, path planning, and computer vision. It's one of the most-starred open-source robotics education projects on GitHub and is used by universities, self-study enthusiasts, and engineers worldwide.

#### 📊 Recent Commit Activity

| Date | SHA | Change | Why It Matters |
|------|-----|--------|-----------------|
| Sep 2, 2026 | `08b453a` | `build(deps): bump github/codeql-action from 4.37.4 to 4.37.9` | Security scanning stays current — signals mature CI practices |
| Sep 2, 2026 | `8c3f761` | `build(deps): bump ruff from 0.16.1 to 0.16.5` | Linting tooling kept up-to-date for code quality |
| Sep 2, 2026 | `069e0fb` | `build(deps): bump scipy from 1.17.1 to 1.18.1` | Core scientific dependency updated — ensures numerical accuracy |

#### 🔑 Key Architecture Highlights
- **100+ algorithm implementations** — from 2D kinematics to 3D SLAM, Kalman filters, Monte Carlo localization, and more
- **Jupyter Notebook integration** — every algorithm is executable and visualizable in notebooks
- **Textbook structure** — each chapter builds on the previous, ideal for self-study or course adoption
- **Clean, readable code** — serves as both reference and teaching material
- **Active dependency management** — regular bumps keep it compatible with the latest Python ecosystem

#### 🎙️ Potential Episode Topics
- *"Learning Robotics From Scratch: How PythonRobotics Made Algorithms Accessible"*
- *"From Kinematics to SLAM: The Full Pipeline Inside a 30k-Star Robotics Tutorial"*
- *"Why Textbook-Code Matters More Than You Think for Robotics Engineers"*
- *"The Hidden Maintenance Cost of Open-Source Education: Keeping Dependencies Current"*

---

### 2. 🚗 AirSim — Open-Source Autonomous Vehicle Simulator

| Field | Detail |
|-------|--------|
| **Repo** | [`microsoft/AirSim`](https://github.com/microsoft/AirSim) |
| **Tag** | `autonomous-vehicles` |
| **Language** | C++ (with Python API) |
| **⭐ Stars** | 18,499 |
| **Latest Commit** | `1ca93f6` — **Sep 15, 2026** |
| **Activity Tier** | 🟢 Actively maintained |

**What it does:** AirSim is Microsoft's **open-source, high-fidelity simulator for autonomous vehicles**, built on Unreal Engine and Unity. It supports cars, drones, and rover platforms with realistic sensors (cameras, LiDAR, IMU, GPS) and AI-friendly APIs. Researchers and companies worldwide use it to train and test autonomous driving algorithms in simulation before deploying to the real world.

#### 📊 Recent Commit Activity

| Date | SHA | Change | Why It Matters |
|------|-----|--------|-----------------|
| Sep 15, 2026 | `1ca93f6` | `Merge PR #9836: Pin GitHub Actions to full-length commit SHAs` | Security hardening — pins Actions to full SHAs to prevent dependency confusion attacks |
| Aug 12, 2026 | `44f3f43` | `Pin GitHub Actions to full-length commit SHAs` | Continuation of security-focused maintenance — Microsoft taking supply-chain security seriously |
| Jun 28, 2026 | `d109f0d` | `Updated README` | Documentation refresh — keeping setup guides current |

#### 🔑 Key Architecture Highlights
- **Unreal Engine / Unity rendering** — photorealistic environments for training perception models
- **Multi-platform support** — cars, drones, rovers, with sensor suites (RGB, depth, LiDAR, IMU, GPS)
- **Python & C++ APIs** — easy integration with ROS, PyTorch, TensorFlow
- **AirLib** — lightweight C++ library for embedding AirSim into custom projects
- **AI research ready** — built-in support for reinforcement learning, imitation learning, and domain randomization
- **Microsoft-backed** — enterprise-grade maintenance and security practices

#### 🎙️ Potential Episode Topics
- *"Inside Microsoft's Autonomous Vehicle Simulator: How AirSim Trains Self-Driving Cars"*
- *"Sim-to-Real: What Happens When Your AI Leaves the Unreal Engine"*
- *"Why Security Patching Matters Even in Simulation Tools"*
- *"From Gaming Engines to Research Labs: The Unlikely Origin of AirSim"*
- *"AirSim vs CARLA: Comparing the Two Giants of Autonomous Driving Simulation"*

---

### 3. ⚡ Robium — Physical AI Skills Harness for Robotics Agents

| Field | Detail |
|-------|--------|
| **Repo** | [`robium-ai/robium`](https://github.com/robium-ai/robium) |
| **Tag** | `robotics` |
| **Language** | Python |
| **⭐ Stars** | 14 |
| **License** | MIT |
| **Latest Commit** | `b945c8f` — **Sep 19, 2026** |
| **Activity Tier** | 🔥 Very actively maintained (3 commits in last 2 days) |

**What it does:** Robium is an **open-source, continuously evolving collection of field-tested robotics expertise** designed as a plugin harness for AI coding agents (Claude Code, Codex, Gemini CLI, Cursor). It covers ROS 2, Nav2, Gazebo, MuJoCo, NVIDIA Isaac Sim, Isaac Lab, and LeRobot — essentially giving any AI coding agent the robotics domain knowledge it needs to write, simulate, and deploy real robotic systems.

#### 📊 Recent Commit Activity

| Date | SHA | Change | Why It Matters |
|------|-----|--------|-----------------|
| Sep 19, 2026 | `b945c8f` | **Release configurable editable workspaces and safe on-demand updates (#78)** | Major feature release — users can now configure custom workspace paths and safely update without risking local changes |
| Sep 19, 2026 | `2d639c6` | **Fix CLI parsing of application hardware lists (#77)** | Bug fix — improving reliability of the setup CLI |
| Sep 19, 2026 | `d044c77` | **Release example-first onboarding with plugin 0.5.1 (#76)** | New user experience — getting started is now faster with reference examples |

#### 🔑 Key Architecture Highlights
- **Skills-based architecture** — each robotics tool (ROS 2, Gazebo, MuJoCo, Isaac Sim, etc.) is a standalone, validator-checked "skill"
- **Multi-agent support** — native plugins for Claude Code, Codex, Gemini CLI, and Cursor
- **Self-maintaining catalog** — hooks capture real build learnings, mine proven patterns from upstream repos, and absorb evidence-gated corrections
- **Capture → Mine → Absorb → Verify loop** — robotics guidance that resists rot by continuously validating against current docs
- **Reference applications** — `robium-apps` repo provides runnable examples for immediate hands-on learning
- **MIT licensed** — fully open with no vendor lock-in

#### 🎙️ Potential Episode Topics
- *"Robium Explained: The Plugin That Gives AI Coding Agents Robotics Superpowers"*
- *"From Claude Code to ROS 2: How Robium Bridges AI and Robotics"*
- *"The Capture-Mine-Absorb-Verify Loop: How Robium Keeps Robotics Knowledge From Rotting"*
- *"Example-First Onboarding: Teaching Robots (and AI) to Code Like Engineers"*
- *"The New Robot Library: Why the Next Breakthrough in Robotics Might Be an AI Plugin"*

---

## 📊 Radar Summary

| # | Project | Domain | Stars | Last Commit | Vibe |
|---|---------|--------|-------|-------------|------|
| 1 | **PythonRobotics** | Robotics Algorithms & Education | 30.5K | Sep 2, 2026 | 🧠 Textbook-grade reference |
| 2 | **AirSim** | Autonomous Vehicle Simulation | 18.5K | Sep 15, 2026 | 🚗 Microsoft-backed sim platform |
| 3 | **Robium** | Physical AI / Robotics Agent Harness | 14 | Sep 19, 2026 | ⚡ Cutting-edge agent tooling |

---

## 🎙️ Episode Pipeline

| Priority | Project | Suggested Angle | Status |
|----------|---------|-------------------|--------|
| 🔴 **High** | Robium | The new wave — AI coding agents with robotics superpowers | In progress |
| 🟡 **Medium** | AirSim | Simulation infrastructure — how Microsoft trains self-driving AI | TBD |
| 🟡 **Medium** | PythonRobotics | Education & accessibility — how 30k developers learned robotics | TBD |

---

## 📋 How to Contribute

This is a **living document**. To suggest a project or submit an episode idea:

1. Fork this repo
2. Add your candidate to the radar (follow the format above)
3. Open a PR with your suggestions
4. Or open an **Issue** with the `episode-suggestion` label

---

*Built for the open-source robotics community. Licensed under MIT.*
# 🤖 Robotics OSS Radar

> A living research hub tracking the most active open-source robotics & autonomous systems projects — curated for the podcast.

## Why This Repo?

This repo is the backbone of the **Robotics OSS Radar** podcast. We scan GitHub daily for the most recently active repositories tagged with `robotics` or `autonomous-vehicles`, review their latest commits, and distill the highlights into:

- **Project summaries** with recent development highlights
- **Potential episode topics** for the podcast
- **A tracking checklist** so we never lose sight of a project that matters

---

## 🔍 How We Pick Projects

1. Search GitHub for repos tagged `topic:robotics` and `topic:autonomous-vehicles`
2. Sort by most recently updated
3. Filter for meaningful, active projects (not spam or low-effort repos)
4. Review the latest 3 commits per project
5. Summarize and assign episode potential

---

## 📡 Currently Tracked Projects

### 1. [MuJoCo](https://github.com/google-deepmind/mujoco) — `google-deepmind/mujoco`

| | |
|---|---|
| **Stars** | 15,241 ⭐ |
| **Language** | C++ (with Python, JS/WASM, C#, Julia, Rust bindings) |
| **License** | Apache-2.0 |
| **Topic** | `robotics` |
| **Last Updated** | Sep 20, 2026 |

**What it is:** MuJoCo (Multi-Joint dynamics with Contact) is a general-purpose physics engine built for fast, accurate simulation of articulated structures. It's the backbone for reinforcement learning research, biomechanics, robotics control, and graphics. Maintained by Google DeepMind, it supports Python, JAX (MJX), Unity, WebAssembly, and has bindings for MATLAB, Java, Julia, Rust, and Swift.

**Recent Commits (Sep 20, 2026):**

| Commit | What's Happening |
|---|---|
| `dc8bb13` | **MIMO actuator support** — multi-input actuators now in control history buffers and `mj_readCtrl`. Big for simulating complex robotic actuators. |
| `451e66a` | **Touch sensor fix in MJX** — isolated touch sensor evaluation from solver divergence in `test_touch_sensor_nested_vmap`. Improves reliability of tactile simulation. |
| `b9ff593` | **Fluid force normalization** — normalized velocity and semi-axes in ellipsoid fluid forces and derivatives. More accurate hydrodynamic simulation. |

**🎙️ Potential Episode Topics:**
- "Sim-to-Real: How MuJoCo Bridges the Gap Between Simulation and Physical Robots"
- "Touch Sensors in Simulation — Why It Matters for Dexterous Manipulation"
- "MJX & JAX: Differentiable Physics for Robotics Research"

---

### 2. [HORUS](https://github.com/softmata/horus) — `softmata/horus`

| | |
|---|---|
| **Stars** | 439 ⭐ |
| **Language** | Rust (with Python & C++ bindings) |
| **License** | Apache-2.0 |
| **Topic** | `autonomous-vehicles`, `robotics` |
| **Last Updated** | Sep 20, 2026 |

**What it is:** HORUS is a real-time distributed middleware for robotics — think of it as a ROS 2 alternative built from the ground up for determinism and low latency. It uses shared-memory ring buffers instead of DDS, achieving **171 ns cross-process IPC** (≈30× faster than ROS 2's default). It supports Rust, Python, and C++ in the same address space, with built-in safety monitors, watchdogs, BlackBox flight recording, and 40+ robotics message types.

**Recent Commits (Sep 20, 2026):**

| Commit | What's Happening |
|---|---|
| `adf86e0` | **Docs cleanup** — stopped advertising Terra framework in the public tree. Keeping docs lean and focused. |
| `96c4c43` | **Massive merge stack** — 6 open PRs merged in one CI cycle (#189, #198, #205, #207, #210, #213, #215). This is a big consolidation push. |
| `16ad2af` | **Dependency bump** — 11 Rust minor version updates across the workspace via Dependabot. Keeping the toolchain current. |

**🎙️ Potential Episode Topics:**
- "HORUS vs ROS 2: Can a Rust-First Middleware Really Beat 30× Latency?"
- "Shared-Memory IPC for Autonomous Vehicles — Why 171 ns Matters"
- "Building a Safe-State Architecture from Scratch (Watchdogs, BlackBox, and Fault Tolerance)"
- "The Rust Robotics Revolution — HORUS and the New Guard"

---

### 3. [NVIDIA Elements](https://github.com/NVIDIA/elements) — `NVIDIA/elements`

| | |
|---|---|
| **Stars** | 87 ⭐ |
| **Language** | TypeScript (Web Components) |
| **License** | Apache-2.0 |
| **Topic** | `autonomous-vehicles`, `robotics` |
| **Last Updated** | Sep 19, 2026 |

**What it is:** NVIDIA Elements is a design system and UI agent harness for AI/ML factories, robotics consoles, and autonomous vehicle tools. It's framework-agnostic (works in React, Angular, Vue, Svelte, Lit, plain HTML) and provides standardized UI components for operational dashboards, monitoring tools, and agent-enabled interfaces. It includes CLI + MCP access so AI assistants can consume component APIs directly.

**Recent Commits (Sep 19, 2026):**

| Commit | What's Happening |
|---|---|
| `907a7ab` | **ESLint strictness** — adopted `no-useless-default-assignment` rule for cleaner code. Quality enforcement continues. |
| `737b82c` | **Release v2.8.0** — `@nvidia-elements/core` shipped version 2.8.0. New components and improvements. |
| `c4e0edd` | **Tag slots feature** — new `feat(core): tag slots` added. Enables slot-based theming and composition patterns. |

**🎙️ Potential Episode Topics:**
- "UI for Autonomous Vehicles — Why Design Systems Matter When 100 Engineers Build Dashboards"
- "AI Agents That Build UIs: NVIDIA Elements + MCP = Component-Level AI Assistance"
- "From Dashboard to Autopilot: How UI Design Systems Shape the Future of Robotic Interfaces"

---

## 📋 Tracking Checklist

See the open issue **[Projects to Revisit & Upcoming Releases](https://github.com/bro26man-hash/robotics-oss-radar/issues)** for the full tracking checklist with timestamps and review cadence.

---

## 🎙️ Podcast Integration

Each episode should:
1. **Summarize** the project's recent commits in plain English
2. **Explain** why the change matters for the robotics/AV community
3. **Interview** a maintainer or contributor if possible
4. **Link** back to this repo for show notes and timestamps

---

## 🛠️ How to Contribute

- **Found a great new repo?** Open an issue with the repo link and why it matters
- **Want to write show notes?** Fork this repo and submit a PR with your episode draft
- **Spotted a breaking change?** Update the relevant project section and flag it in the issue tracker

---

## 📅 Review Cadence

| Cadence | Action |
|---|---|
| **Daily** | Scan for newly active repos in `robotics` & `autonomous-vehicles` |
| **Weekly** | Review latest commits for all tracked projects |
| **Monthly** | Update summaries, prune inactive projects, add new ones |
| **Per Episode** | Deep-dive one project, update show notes |

---

*Built for the open-source robotics community.*

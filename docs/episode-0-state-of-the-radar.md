# 🎙️ Episode Notes — Episode 0: State of the Radar (Sep 18, 2026)

> First-look breakdown of the three most recently active open-source robotics projects, based on live commit analysis.

---

## Project 1: 🟢 MuJoCo — google-deepmind/mujoco

| | |
|---|---|
| **Stars** | ⭐ 15,214 |
| **Language** | C++ |
| **License** | Apache-2.0 |
| **Focus** | Multi-joint dynamics with contact — general-purpose physics simulator |
| **Last Activity** | September 18, 2026 (5 commits in last 2 days) |

### What it does
MuJoCo (Multi-Joint dynamics with Contact) is a physics engine designed for research and production in robotics, biomechanics, graphics, and animation. It provides fast, accurate simulation of complex interacting bodies with contacts, fractures, soft tissues, and fluids. It's the backbone of deep reinforcement learning pipelines (notably through Gymnasium wrappers) and is used by Google DeepMind, NVIDIA, and countless academic labs worldwide.

### Latest Commits (what's being worked on)

| Commit | Author | Date | What it means |
|--------|--------|------|---------------|
| Raise error in `mjd_transitionFD`/`mjd_inverseFD` when sleeping enabled | Yuval Tassa | Sep 18 | **Safety hardening** — Silent simulation corruption was possible when sleeping flag was on; now it throws an explicit error instead of producing garbage results |
| Introduce archive resource providers | Sam Haves | Sep 18 | **New feature** — Modular asset loading from archive files; enables packed-scene workflows and easier distribution of complex robot models |
| Honor spring/damper disable flags in discrete metric | Alessio Quaglino | Sep 17 | **Bug fix** — Energy conservation was broken in fluid/passive contact terms when springs/dampers were disabled; now correctly honored |
| Compute flex stretch forces from edge tensions | Alessio Quaglino | Sep 17 | **New feature** — Soft-body and cable simulation now computes stretch forces from edge tension constraints, improving fidelity for fabric/cable/rope scenarios |
| Release GIL in filament renderer | Sam Haves | Sep 17 | **Performance** — Python bindings no longer hold the GIL during filament rendering, enabling true parallel rendering in multi-threaded training pipelines |

### 🎙️ Episode Topics
1. **"Releasing the GIL: How MuJoCo Is Unlocking True Parallel Robot Simulation"** — Deep dive into the filament renderer change and what it means for multi-threaded RL training
2. **"Silent Simulation Bugs: Why Sleeping States Need Explicit Errors"** — The importance of fail-fast in physics engines; what corrupted simulations look like in production
3. **"Soft-Body Physics at Scale — Inside MuJoCo's Flex Stretch Engine"** — Edge tension constraints and why they matter for cable/fabric simulation
4. **"Archive Resource Providers & the Future of Packed-Robot Scenes"** — How modular asset loading changes how we distribute and version robot simulation environments

---

## Project 2: 🔵 Rerun — rerun-io/rerun

| | |
|---|---|
| **Stars** | ⭐ 11,472 |
| **Language** | Rust + Python + C++ |
| **License** | Apache-2.0 |
| **Focus** | Multimodal data visualization & streaming for physical AI |
| **Last Activity** | September 18, 2026 (6 commits same day) |

### What it does
Rerun is the data layer for physical AI. It ingests multi-rate, multimodal data (images, point clouds, transforms, time series, joint states, video) from robot logs, human-data rigs, sim, and web video. The built-in viewer renders everything in sync, in realtime — scrub episodes, compare sensors, watch CV pipelines run live. Data is queryable with dataframes or SQL, and streams directly into training.

### Latest Commits (what's being worked on)

| Commit | Author | Date | What it means |
|--------|--------|------|---------------|
| Allow opting out of startup update checks from JS API | Andreas Reich | Sep 18 | **Developer experience** — Air-gapped and embedded deployments can now disable automatic update checks; critical for production robotics environments |
| Add `misc` as new changeset type | Jochen Görtler | Sep 18 | **Architecture** — Expands the granular update tracking system; `misc` fills a gap for changes that don't fit existing categories |
| `re_lerobot`: Collect and categorize LeRobot import diagnostics | Eric Leijonmarck | Sep 18 | **Interoperability** — Tackles format fragmentation by providing structured migration warnings when importing LeRobot datasets; signals Rerun is becoming the de facto target format |
| Volume raymarcher | Gábor Gyebnár | Sep 18 | **New feature** — Full 3D scalar field volume rendering; enables direct visualization of LiDAR point clouds, CT scans, and volumetric sensor data inside Rerun |
| Lift `LogMsg`/`ArrowMsg` into `re_log_msg` crate | Antoine Beyeler | Sep 18 | **Architecture refactor** — Major codebase reorg: separates logging message types into their own crate; paves the way for zero-copy streaming and cleaner crate boundaries |

### 🎙️ Episode Topics
1. **"The Data Layer for Physical AI — Why Rerun Could Replace Rviz"** — Architectural comparison; why columnar storage + SQL queryability beats RViz'srosbag approach
2. **"Rust for Robotics: Building a Columnar Storage Engine for Multi-Rate Sensor Data"** — How Rust's ownership model enables zero-copy streaming that Python can't match
3. **"From LeRobot to Rerun: The Challenge of Standardizing Robotics Dataset Formats"** — Eric Leijonmarck's import diagnostics work as a case study in format fragmentation
4. **"Volume Rendering for Robot Perception: What's Inside the Black Box?"** — Live demo of the new raymarcher with real LiDAR data
5. **"Air-Gapped Robotics: Why JS APIs Need Opt-Out Update Checks"** — The real-world constraints of deploying visualization in closed networks

---

## Project 3: 🟡 Physicar DeepRacer for Cloud — PoetAndPoem4Hu/physicar-deepracer-for-cloud

| | |
|---|---|
| **Stars** | — |
| **Language** | Java |
| **License** | Not specified |
| **Focus** | Cloud-based reinforcement learning training for AWS DeepRacer |
| **Last Activity** | September 18, 2026 (README update) |

### What it does
Physicar provides a platform for training AWS DeepRacer models in the cloud, making reinforcement learning for autonomous vehicles more accessible and effective. It bridges the gap between local sandbox training and production-grade policy optimization by leveraging cloud compute for faster, more scalable RL experiments.

### Latest Commits (what's being worked on)

| Commit | Author | Date | What it means |
|--------|--------|------|---------------|
| Update README.md | PoetAndPoem4Hu | Sep 18, 2026 | **Documentation** — Comprehensive README overhaul; suggests the project may be preparing for a community relaunch or new user onboarding push |
| Update README.md | PoetAndPoem4Hu | Sep 28, 2025 | **Documentation** — Earlier refresh; indicates a roughly annual maintenance cadence |
| version1.2 | PoetAndPoem4Hu | Mar 10, 2019 | **Core release** — Last version bump; established the cloud training pipeline architecture |

### ⚠️ Maintenance Assessment
This repo shows a **7-year gap** between core releases (v1.2 in March 2019) with only README touch-ups in 2025–2026. Two interpretations:
- **Optimistic:** The maintainer is preparing for v2.0 and refreshing docs before a relaunch
- **Pessimistic:** The project is moribund and the README updates are cosmetic patches on an abandoned codebase

### 🎙️ Episode Topics
1. **"Cloud RL for Autonomous Vehicles: Can You Train a Better Policy Faster?"** — Benchmark cloud vs. local training; is the economics actually there?
2. **"The DeepRacer Ecosystem — Hobbyist Sandbox vs. Production-Grade Training"** — Where does Physicar fit in the spectrum?
3. **"When Open-Source Projects Go Quiet: Maintenance Cadence and Community Risk"** — A cautionary tale; what happens when a tool you depend on hasn't had a core release in 7 years?
4. **"Reinforcement Learning in Practice: What AWS DeepRacer Gets Wrong (and Right)"** — Honest assessment of the hardware/software stack

---

## 📊 Activity Snapshot

| Project | Stars | Language | Key Commit Theme | Episode Arc | Activity Health |
|---------|-------|----------|------------------|-------------|-----------------|
| **MuJoCo** | 15,214 | C++ | GIL release + soft-body physics + archive providers | "Under the Hood of Parallel Simulation" | 🟢 **Very Active** — 5 commits in 2 days, multiple contributors |
| **Rerun** | 11,472 | Rust | Volume raymarcher + LeRobot integration + arch refactor | "The Data Layer for Physical AI" | 🟢 **Very Active** — 6 commits in 1 day, rapid iteration |
| **Physicar** | — | Java | README revamp + cloud RL pipeline | "Cloud RL for Autonomous Vehicles" | 🟡 **Uncertain** — Only README updates; 7-year release gap |

---

## 🎙️ Podcast Alignment — Suggested Episode Calendar

| Episode | Project | Priority | Theme | Target Date |
|---------|---------|----------|-------|-------------|
| #1 | MuJoCo — GIL & Parallel Simulation | 🔴 High | Simulation infrastructure | Week 1 |
| #2 | Rerun — Data Layer for Physical AI | 🔴 High | Data infrastructure | Week 2 |
| #3 | Physicar — Cloud RL for AVs | 🟡 Medium | RL in production | Week 3 |
| #4 | MuJoCo — Soft-Body Physics Deep-Dive | 🟡 Medium | Simulation fidelity | Week 4 |
| #5 | Rerun — LeRobot Dataset Migration | 🟡 Medium | Format standardization | Week 5 |
| #6 | Physicar — Actually Running a Training Job | 🟢 Low (conditional) | Economics of cloud RL | Week 6 |

---

## 🔔 Triggers for Early Revisit

- Any project tags a **new release** (mujoco v3.x, rerun v0.x, physicar v2.x)
- A **breaking change** is introduced in key dependencies
- A **security advisory** is filed against any project
- The podcast receives **listener questions** about a specific project

---

*See the tracking issue: [Projects to Revisit & Upcoming Releases](https://github.com/bro26man-hash/robotics-oss-radar/issues/51)*
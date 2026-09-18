# 📡 Robotics OSS Radar

> Tracking the most active open-source robotics & autonomous-vehicle projects. Weekly progress snapshots, development highlights, and podcast episode ideas.

---

## 🔍 Why This Project?

Open-source robotics and autonomous systems are evolving at breakneck speed. This repo is the backbone of our podcast **"Robotics OSS Radar"** — a weekly deep-dive into the projects shaping the future of autonomous machines. We track commits, highlight development trends, and translate technical progress into compelling episodes.

---

## 🏆 Top 3 Projects Under the Microphone

These are the three most recently active, high-impact repositories tagged with `robotics` or `autonomous-vehicles`, curated from GitHub's latest activity as of September 18, 2026.

---

### 1. 🟢 [MuJoCo](https://github.com/google-deepmind/mujoco)

| | |
|---|---|
| **Stars** | ⭐ 15,214 |
| **Language** | C++ |
| **License** | Apache-2.0 |
| **Focus** | Multi-joint dynamics with contact — general-purpose physics simulator for robotics |
| **Last Activity** | September 18, 2026 (4 commits same day) |

**What it does:** MuJoCo (Multi-Joint dynamics with Contact) is the gold-standard open-source physics simulator for robotics and biomechanics. It provides fast, accurate simulation of articulated bodies under contact forces, and is widely used for robot control research, reinforcement learning, and human-body modeling. It's the simulator behind countless papers at CoRL, RSS, and ICRA.

**Recent Development Highlights:**
- 🔧 **Error Handling for Finite-Difference Functions** — `mjd_transitionFD` and `mjd_inverseFD` now raise proper errors when sleeping is enabled, preventing silent miscalculations in sensitivity analysis (Yuval Tassa)
- 📦 **Archive Resource Providers** — New abstraction for loading resources from archived bundles, improving portability and reproducibility of simulation setups (Sam Haves)
- 🦴 **Spring & Damper Disable Flags in Discrete Metric** — Honored spring/damper disable flags in fluid and passive contact terms, giving users finer control over contact modeling in the discrete metric framework (Alessio Quaglino)
- 🧵 **Flex Stretch Forces from Edge Tensions** — Computed flex stretch forces from edge tensions, advancing soft-body and cable simulation capabilities (Alessio Quaglino)
- 🚀 **GIL Release in Filament Renderer** — Released the Python GIL in the filament renderer, enabling true multi-threaded rendering pipelines from Python (Sam Haves)

**🎙️ Potential Episode Topics:**
- "The Physics Engine Under 1,000 Robotics Papers — Inside MuJoCo"
- "Soft-Body Simulation Is Hard: How MuJoCo Models Cables and Muscles"
- "Releasing the GIL: Why Python Robotics Simulators Are Slow (And How to Fix It)"
- "From MuJoCo to Humanoids: The Simulator That Borrowed from Biomechanics"

---

### 2. 🔵 [Rerun](https://github.com/rerun-io/rerun)

| | |
|---|---|
| **Stars** | ⭐ 11,472 |
| **Language** | Rust + Python + C++ |
| **License** | Apache-2.0 |
| **Focus** | Visualize, query, and stream multimodal robotics data for physical AI |
| **Last Activity** | September 18, 2026 (5 commits same day) |

**What it does:** Rerun is the data layer for physical AI. It ingests multi-rate, multimodal data (images, point clouds, transforms, time series, joint states, video) from robot logs, human-data rigs, sim, and web video. The built-in viewer renders everything in sync, in realtime — scrub episodes, compare sensors, watch CV pipelines run live. Data is queryable with dataframes or SQL, and streams directly into training workflows.

**Recent Development Highlights:**
- 🔦 **Volume Raymarcher** — Brand-new volume rendering capability for 3D scalar field visualization, enabling ray-march-based rendering of density fields, temperature maps, and FAHR data (Gábor Gyebnár)
- 🤖 **LeRobot Import Diagnostics** — `re_lerobot`: Collect and categorize import warnings when migrating LeRobot datasets into Rerun, addressing the growing demand for HuggingFace robotics dataset interop (Eric Leijonmarck)
- 🏗️ **Logging Architecture Refactor** — Lifted `LogMsg`, `ArrowMsg` and friends out of `re_log_types` into a dedicated `re_log_msg` crate, improving code modularity and separation of concerns (Antoine Beyeler)
- 🔧 **Changeset Type System Expansion** — Added `misc` as a new changeset type, expanding the granular update tracking system for more precise change impact analysis (Jochen Görtler)
- 📦 **Build Reproducibility** — Pinned `hatchling` to `v1.30.1` for reproducible Python builds, ensuring consistent CI across environments (Jochen Görtler)

**🎙️ Potential Episode Topics:**
- "The Data Layer for Physical AI — Why Rerun Could Replace Rviz"
- "Rust for Robotics: Building a Columnar Storage Engine for Multi-Rate Sensor Data"
- "From LeRobot to Rerun: The Challenge of Standardizing Robotics Dataset Formats"
- "Volume Rendering for Robot Perception: What's Inside the Black Box?"

---

### 3. 🟣 [AlpaSim](https://github.com/NVlabs/alpasim)

| | |
|---|---|
| **Stars** | ⭐ 1,239 |
| **Language** | Python |
| **License** | Apache-2.0 |
| **Focus** | Open-source autonomous vehicle simulation platform for end-to-end AV policy development & testing |
| **Last Activity** | August 18, 2026 (latest commit); actively synced from internal GitLab |

**What it does:** AlpaSim is NVIDIA's open-source autonomous vehicle simulation platform designed for development and testing of end-to-end AV policies. Unlike traditional modular AV stacks, AlpaSim focuses on simulating complete, monolithic driving policies — from perception to control — in a photorealistic, high-fidelity environment. It's built for researchers who want to train and evaluate neural network-based driving agents in a loop.

**Recent Development Highlights:**
- 🔄 **CI Pipeline Overhaul — Avoid LFS Downloads During GitLab Replay** — Major CI improvement to avoid Large File Storage downloads when replaying GitHub changes to GitLab, dramatically speeding up sync times (jarcherNV)
- 🎲 **Reproducible Rollout Seeds via RolloutSpec** — Made rollout seeds selectable and reproducible through the `RolloutSpec` API, a critical step for scientific rigor in RL training evaluation (Alba María Téllez Fernández)
- 🚀 **Linear MPC Speed Bound Increased to 40 m/s** — Pushed the linear Model Predictive Controller speed limit from previous thresholds to 40 m/s (~90 mph), expanding the envelope for high-speed autonomous driving scenarios (Ding-ray)
- 🔄 **GitLab Sync (2026-08-11)** — Regular sync from NVIDIA's internal GitLab, bringing the latest proprietary improvements into the open-source codebase (mwatson-nvidia)
- 🐛 **Self-Hosted Build Job Fix** — Resolved `uv` install issues in self-hosted CI runners, improving build reliability for the AlpaSim ecosystem (jarcherNV)

**🎙️ Potential Episode Topics:**
- "End-to-End AV Learning: Why Monolithic Neural Networks Are Replacing Modular Stacks"
- "Reproducibility in RL: Why Your Rollout Seeds Matter (And How AlpaSim Is Fixing It)"
- "40 m/s in Simulation: Pushing the Limits of MPC-Based Autonomous Driving"
- "NVIDIA's Open Source Strategy: What AlpaSim Tells Us About the Future of AV Research"

---

## 📊 Activity Snapshot (as of September 18, 2026)

| Project | Stars | Language | Latest Commit | Key Theme |
|---------|-------|----------|---------------|-----------|
| MuJoCo | 15,214 | C++ | Soft-body forces + GIL release + archive providers | Physics engine maturity & soft-body simulation |
| Rerun | 11,472 | Rust | Volume raymarcher + architecture refactor + LeRobot interop | Data infrastructure & rendering |
| AlpaSim | 1,239 | Python | MPC speed bump + reproducible rollouts + CI overhaul | End-to-end AV policy evaluation |

---

## 🎙️ Podcast Alignment

Each project maps to a natural episode arc:

1. **Physics Episode** → MuJoCo: "What happens inside a physics engine when a robot touches the world?"
2. **Data Episode** → Rerun: "How do you log, query, and stream 100 sensor streams from a robot?"
3. **AV Policy Episode** → AlpaSim: "Can a single neural network learn to drive at 90 mph?"

---

## 📋 Tracking

See the open issue **[Projects to Revisit & Upcoming Releases](https://github.com/bro26man-hash/robotics-oss-radar/issues/50)** for the running checklist of items to revisit before the next episode cycle.

---

## 🤝 Contributing

Pull requests and suggestions are welcome! To propose a new project or episode topic:
1. Open an issue describing the project and why it matters
2. Tag it with `proposal` and `episode-topic`
3. The maintainers will review and add to the radar

## 📄 License

This project is open-source under the [MIT License](LICENSE).
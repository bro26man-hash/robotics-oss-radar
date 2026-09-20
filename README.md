# 🤖 Robotics OSS Radar

> Tracking the most active open-source robotics & autonomous-systems projects — with development highlights and podcast episode ideas.

---

## 📡 Projects Under the Lens

---

### 1. [google-deepmind/mujoco](https://github.com/google-deepmind/mujoco)
**Tag:** `robotics` · **Language:** C++ · **Stars:** 15,241★

**What it is:** MuJoCo (Mu**Jo**int dynamics with **Co**ntact) is a general-purpose physics engine built by Google DeepMind for fast, accurate simulation of articulated structures — robots, biomechanics, grippers, and more. It's the backbone of countless research labs and RL pipelines, with Python bindings, a Unity plugin, and a thriving third-party ecosystem (MATLAB, Julia, Rust, Swift, and more).

**Recent development highlights:**
- 🗓️ **Sep 20, 2026** — `Support multi-input (MIMO) actuators in control history buffers and mj_readCtrl` (dc8bb13, @YuvalTassa): Major update — MuJoCo now supports multi-input, multi-output actuators in its control history buffers and `mj_readCtrl` API, enabling more realistic actuator modeling for complex robotic systems with coupled dynamics.
- 🗓️ **Sep 20, 2026** — `mjx: isolate touch sensor evaluation from solver divergence in test_touch_sensor_nested_vmap` (451e66a, @YuvalTassa): Bug fix — touch sensor evaluation in the MuJoCo XLA (JAX) branch is now isolated from solver divergence, preventing false negatives in contact-rich simulations.
- 🗓️ **Sep 20, 2026** — `Normalize velocity and semi-axes in ellipsoid fluid forces and derivatives` (b9ff593, @YuvalTassa): Physics accuracy improvement — ellipsoid fluid force calculations now use normalized velocity and semi-axes, ensuring consistent behavior across different model scales and improving realism in fluid-structure interaction simulations.

🎙️ **Potential episode topics:**
- *"MuJoCo: The Physics Engine Powering Modern Robotics Research"* — How MuJoCo went from a research project at Stanford to the de facto standard for robot simulation, and what makes its contact dynamics so special.
- *"MIMO Actuators & the Future of Robot Control"* — What multi-input actuator support means for simulating tendon-driven robots, soft actuators, and coupled dynamics.
- *"Differentiable Physics: Training Robots with Analytical Gradients"* — How MuJoCo's differentiable simulation enables gradient-based policy optimization that's unleashing a wave of learned locomotion and manipulation behaviors.

---

### 2. [PetoiCamp/OpenCat-Quadruped-Robot](https://github.com/PetoiCamp/OpenCat-Quadruped-Robot)
**Tag:** `robotics` · **Language:** C++ · **Stars:** 5,346★

**What it is:** OpenCat is an open-source quadruped robot framework by Petoi — the maker of Bittle (robot dog) and Nybble (robot cat). Running on Arduino and Raspberry Pi, it handles gait coordination, servo control, and IMU integration so makers, researchers, and educators can build on top of it. With 30,000+ robots shipped across 60+ countries, it's one of the most widely deployed open-source legged robotics platforms.

**Recent development highlights:**
- 🗓️ **Sep 8, 2026** — `Merge PR #119: Readme / Quaddle growth update` (24563ca, @KaiMai): Documentation refresh — major README update covering the upcoming **Quaddle** Kickstarter launch (Sept 2, 2026), Petoi's newest mini quadruped with position-feedback servos and Puppet Mode.
- 🗓️ **Sep 8, 2026** — `Remove Discord link and update Kickstarter referral code to 8t25yj` (4238b67, @KaiMai): Community shift — removed Discord link, updated Kickstarter referral, signaling a focus on Kickstarter launch and open-source code release before Quaddle delivery.
- 🗓️ **Sep 2, 2026** — `Merge PR #118: Readme / Quaddle growth update` (532f016, @RongzhongLi): Pre-launch documentation — Quaddle growth update merged, building anticipation for the new desk-sized quadruped with 4-servo gait design.

🎙️ **Potential episode topics:**
- *"From Dorm Room to Kickstarter: The OpenCat Quadruped Story"* — How Dr. Rongzhong Li turned a Harvard dorm project into 30,000+ shipped robots across 60+ countries.
- *"Quaddle: 4 Servos, Position Feedback, and Puppet Mode"* — Inside the engineering of Petoi's newest quadruped — how fewer servos with position feedback enables genuinely novel gaits and human-guided motion recording.
- *"Sim-to-Real on a Budget: OpenCat + NVIDIA Isaac + RL"* — How the community is using OpenCat with Isaac Sim and reinforcement learning to train real behaviors on affordable hardware.

---

### 3. [OpenDriveLab/UniAD](https://github.com/OpenDriveLab/UniAD)
**Tag:** `autonomous-vehicles` · **Language:** Python · **Stars:** 4,761★

**What it is:** UniAD (UNified Autonomous Driving) is a planning-oriented unified framework for autonomous driving from OpenDriveLab (Shanghai AI Lab). It casts perception, prediction, and planning as a single hierarchical system — rather than modular pipelines — and achieved SOTA on nuScenes at CVPR 2023 (Best Paper Award). The just-released **UniAD 2.0** upgrades to mmdet3d 1.x & torch 2.x and integrates nuPlan and NAVSIM datasets.

**Recent development highlights:**
- 🗓️ **Oct 29, 2025** — `Update README for UniAD 2.0 Release` (609ee08, @TianyuLi): Major release documentation — comprehensive README overhaul for UniAD 2.0, including new framework architecture, dataset integrations, and benchmark results.
- 🗓️ **Oct 29, 2025** — `🚀 Release Notes for UniAD v2.X (#251)` (7d7d0c1, @zzh-yun): Official v2.0 launch — migration to mmdet3d 1.0.0rc6 and torch 2.0.1+cu118; nuPlan and NAVSIM benchmark tools coming in 2025Q2; all existing workflows preserved.
- 🗓️ **Oct 27, 2025** — `Update README.md` (713fd85, @JiazhiYang): Pre-release cleanup — final README touches ahead of the v2.0 launch.

🎙️ **Potential episode topics:**
- *"UniAD 2.0: One Model to Rule All Autonomous Driving Tasks"* — How a single unified framework replaces the modular pipeline approach, and what the nuPlan/NAVSIM integration means for the field.
- *"Planning-Oriented vs. Perception-First: The Great AV Debate"* — UniAD's philosophy that planning should drive perception, not the other way around — is this the right paradigm for self-driving?
- *"From CVPR Best Paper to Open Source: The UniAD Story"* — The journey from a research paper to one of the most widely used autonomous driving codebases, and what the 2.0 rewrite teaches us about maintaining open-source research software.

---

## 🎙️ About This Radar

This repo is the companion data source for the **Robotics OSS Radar** podcast — a show exploring the open-source projects shaping the future of autonomous systems and robotics. Each episode dives deep into one project, interviewing maintainers, walking through the code, and discussing what's coming next.

**Suggested episode cadence:**
| Week | Project | Theme |
|------|---------|-------|
| 1 | MuJoCo | MuJoCo: The Physics Engine Powering Modern Robotics Research & Differentiable Physics |
| 2 | OpenCat | From Dorm Room to Kickstarter: The OpenCat Quadruped Story & Sim-to-Real on a Budget |
| 3 | UniAD | UniAD 2.0: One Model to Rule All Autonomous Driving Tasks & Planning-Oriented vs. Perception-First |

---

## 🔧 How to Contribute

- Found a stale project? Open an issue with the repo URL and what you expected to see.
- Want your project featured? Submit a link and a 2-line description.
- Episode ideas? The issue tracker is the place.

---

## 📊 Radar Dashboard

| Project | Last Commit | Activity | Stars | Language |
|---------|-------------|----------|-------|----------|
| MuJoCo | Sep 20, 2026 | 🟢 Active (MIMO actuators + touch sensor fix + fluid force normalization) | 15,241★ | C++ |
| OpenCat | Sep 8, 2026 | 🟡 Moderate (Quaddle Kickstarter prep + README updates) | 5,346★ | C++ |
| UniAD | Oct 29, 2025 | 🟡 Periodic (v2.0 release + framework migration) | 4,761★ | Python |

---

*Built with 💡 and a lot of open-source love.*
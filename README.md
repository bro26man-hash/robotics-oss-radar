# 🤖 Robotics OSS Radar

> Tracking the most active open-source robotics & autonomous-systems projects — with development highlights and podcast episode ideas.

---

## 📡 Projects Under the Lens

### 1. [google-deepmind/mujoco](https://github.com/google-deepmind/mujoco)
**Tag:** `robotics` · **Language:** C++ · **Stars:** 15,241★

**What it is:** MuJoCo (Multi-Joint dynamics with Contact) is a general-purpose physics simulator developed by Google DeepMind. It's the de facto standard for robotics R&D — used for training legged robots, manipulators, and soft-body systems via reinforcement learning. Its speed and accuracy make it the backbone of sim-to-real transfer for companies like Unitree, Apptronik, and countless academic labs.

**Recent development highlights:**
- 🗓️ **Sep 20, 2026** — `Support multi-input (MIMO) actuators in control history buffers and mj_readCtrl` (dc8bb13, @YuvalTassa): Major capability upgrade — MIMO actuator support enables modeling of complex actuator configurations (e.g., dual-actuator joints, antagonistic muscle-tendon units), directly benefiting biomimetic and humanoid robot simulations.
- 🗓️ **Sep 20, 2026** — `mjx: isolate touch sensor evaluation from solver divergence in test_touch_sensor_nested_vmap` (451e66a, @YuvalTassa): Critical bug fix — touch sensor evaluation is now isolated from solver divergence, preventing false positives when the physics solver struggles with convergence in complex contact scenarios.
- 🗓️ **Sep 20, 2026** — `Normalize velocity and semi-axes in ellipsoid fluid forces and derivatives` (b9ff593, @YuvalTassa): Accuracy fix in fluid force computation — normalization ensures physically consistent drag and lift forces, which matters for underwater and aerial robot simulation.

🎙️ **Potential episode topics:**
- *"MuJoCo: The Physics Engine Behind the Robotics Revolution"* — How a physics simulator became the hidden engine behind every major legged-robot and VLA project.
- *"Sim-to-Real: Why Simulation Fidelity Matters"* — From MIMO actuators to fluid forces, how MuJoCo's latest features are closing the sim-to-real gap.
- *"Inside DeepMind's Robotics Stack"* — What does a world-class physics simulator tell us about where AI and robotics are heading next?

---

### 2. [isaac-sim/IsaacLab](https://github.com/isaac-sim/IsaacLab)
**Tag:** `robotics` · **Language:** Python · **Stars:** 8,176★

**What it is:** Isaac Lab is NVIDIA's unified framework for robot learning — combining Isaac Sim's photorealistic 3D simulation with PyTorch-based reinforcement learning pipelines. It's the go-to platform for training humanoids, manipulators, and quadrupeds with parallelized GPU-accelerated RL. Version 3.0 is currently in heavy development.

**Recent development highlights:**
- 🗓️ **Sep 20, 2026** — `[RL] Unify and cleanup isaaclab_rl for 3.0 release` (4b1234b, @MustafaH): Major pre-release refactor — the RL module is being unified and cleaned up for the v3.0 launch, consolidating APIs and removing deprecated wrappers. This signals that Isaac Lab 3.0 is approaching feature-complete.
- 🗓️ **Sep 20, 2026** — `[Scripts] Remove legacy benchmark_camera script and update documentation` (0daf5fe, @MustafaH): API cleanup — the old benchmark_camera script is removed and docs are refreshed, part of the broader v3.0 stabilization effort.
- 🗓️ **Sep 20, 2026** — `[Tasks] Final isaaclab_tasks cleanup pass for 3.0` (0c5dcbc, @MustafaH): Task library standardization — the final cleanup pass on the task definitions that prescribe robot behaviors, ensuring consistency across all 100+ built-in tasks before the v3.0 cut.
- 🗓️ **Sep 20, 2026** — `[Tests] Make core unit tests device-aware` (1089f00, @MustafaH): Testing infrastructure upgrade — core unit tests now run on both CPU and GPU devices, catching device-specific bugs before they hit production.
- 🗓️ **Sep 20, 2026** — `Add TorchRL environment wrapper for isaaclab_rl` (5c91e9b, @theap06): Ecosystem integration — a new TorchRL wrapper enables direct interoperability with TorchRL's RL training pipelines, expanding the framework's reach beyond NVIDIA's own learning tools.

🎙️ **Potential episode topics:**
- *"Isaac Lab 3.0: What's Changing and Why It Matters"* — A maintainer walkthrough of the biggest refactor in Isaac Lab's history and what the v3.0 release means for the robotics community.
- *"GPU-Accelerated RL: Training a Humanoid in a Weekend"* — How Isaac Lab's parallel simulation pipeline turns weeks of RL training into hours.
- *"TorchRL × Isaac Lab: The Open Ecosystem Play"* — Why NVIDIA's decision to wrap Isaac Lab for TorchRL is a signal of how the robotics RL ecosystem is converging.

---

### 3. [autowarefoundation/autoware_universe](https://github.com/autowarefoundation/autoware_universe)
**Tag:** `autonomous-vehicles` · **Language:** C++ (ROS 2) · **Stars:** 1,757★

**What it is:** Autoware.Universe is the monorepo for Autoware — the world's leading open-source autonomous driving stack. It's a full-stack ROS 2 platform covering perception (LiDAR-based 3D object detection, semantic segmentation), planning (behavioral planning, motion planning), control, HD mapping, and simulation. It's the reference implementation for many AV companies and municipal pilot programs, especially in Japan.

**Recent development highlights:**
- 🗓️ **Sep 19, 2026** — `feat(autoware_ptv3): support multisweep densification with time-lag features` (02d25ce, @AmadeuszSzymko): Perception breakthrough — the PointTransformer v3 (PTv3) now supports multisweep densification with time-lag features, dramatically improving 3D object detection accuracy in sparse-point regimes (e.g., long-range detection, adverse weather).
- 🗓️ **Sep 19, 2026** — `test(cuda_pointcloud_preprocessor): cover capacity bounds behavior` (0d81781, @MaxSchmeller): Safety testing — new characterization tests for the CUDA pointcloud preprocessor ensure it handles capacity edge cases without overflow, critical for production-grade perception pipelines.
- 🗓️ **Sep 18, 2026** — `feat(autoware_ptv3)!: per-stage voxel-count maximums and input truncation to the stage bounds` (4af11fb, @MaxSchmeller): Performance optimization — per-stage voxel-count limits and input truncation prevent the PTv3 model from over-consuming GPU memory on large pointclouds, making real-time inference feasible.
- 🗓️ **Sep 18, 2026** — `feat(autoware_path_distance_calculator): move the node to agnocast_wrapper::Node` (06df2f6, @KoichiImai): API modernization — migration to the agnocast_wrapper Node pattern improves abstraction and testability of the path distance calculator.

🎙️ **Potential episode topics:**
- *"Autoware Universe: The Open-Source AV Stack That's Powering Japan's Robotaxi Dreams"* — How Autoware became the reference AV platform and what its next milestones are.
- *"PointTransformer v3: The AI Model Making Lidar Smarter"* — Inside the multisweep densification and time-lag features that are pushing 3D perception accuracy to new highs.
- *"From ROS 2 to Production: How Autoware Manages Safety-Critical Perception"* — The testing and abstraction patterns that make an open-source AV stack trustworthy.

---

## 🎙️ About This Radar

This repo is the companion data source for the **Robotics OSS Radar** podcast — a show exploring the open-source projects shaping the future of autonomous systems and robotics. Each episode dives deep into one project, interviewing maintainers, walking through the code, and discussing what's next.

**Suggested episode cadence:**
| Week | Project | Theme |
|------|---------|-------|
| 1 | MuJoCo | The Physics Engine Behind the Robotics Revolution & Sim-to-Real |
| 2 | Isaac Lab | GPU-Accelerated RL & the v3.0 Refactor |
| 3 | Autoware Universe | The Open-Source AV Stack & PointTransformer v3 |

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
| Isaac Lab | Sep 20, 2026 | 🟢 Active (v3.0 RL refactor + TorchRL wrapper + device-aware tests) | 8,176★ | Python |
| Autoware Universe | Sep 19, 2026 | 🟢 Active (PTv3 multisweep densification + CUDA safety tests + API modernization) | 1,757★ | C++ |

---

*Built with 💡 and a lot of open-source love.*
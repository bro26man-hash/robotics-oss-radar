# 🤖 Robotics OSS Radar

> Tracking the most active open-source robotics & autonomous-systems projects — with development highlights and podcast episode ideas.

---

## 📡 Projects Under the Lens

### 1. [google-deepmind/mujoco](https://github.com/google-deepmind/mujoco)
**Tag:** `robotics` · **Language:** C++ · **Stars:** 15,241★

**What it is:** MuJoCo (Multi-Joint dynamics with Contact) is a general-purpose physics simulator designed for research and development in robotics, biomechanics, graphics, and animation. It's the gold standard for fast, accurate rigid-body simulation with contacts and is widely used in robot learning, manipulation research, and reinforcement learning environments.

**Recent development highlights:**
- 🗓️ **Sep 20, 2026** — `Support multi-input (MIMO) actuators in control history buffers and mj_readCtrl` (dc8bb13, @YuvalTassa): Major functionality upgrade — MIMO actuator support in control history buffers enables modeling of complex multi-input actuator systems (e.g., parallel actuators, differential drives) directly in MuJoCo's control API. This is a big deal for researchers simulating robots with non-trivial actuator configurations.
- 🗓️ **Sep 20, 2026** — `mjx: isolate touch sensor evaluation from solver divergence in test_touch_sensor_nested_vmap` (451e66a, @YuvalTassa): Bug fix — Touch sensor evaluation is now isolated from solver divergence in nested VMAP tests, improving numerical stability for models with tactile sensors. This matters for dexterous manipulation and prosthetic research.
- 🗓️ **Sep 20, 2026** — `Normalize velocity and semi-axes in ellipsoid fluid forces and derivatives` (b9ff593, @YuvalTassa): Physics accuracy improvement — Normalization of velocity and semi-axes in ellipsoid fluid force models ensures consistent behavior across different scale regimes, critical for underwater robotics and micro-air-vehicle simulations.

🎙️ **Potential episode topics:**
- *"The Physics Engine Under Every Robot Lab"* — How MuJoCo went from CMU research project to DeepMind-owned gold standard, and why it powers so much of the robotics RL revolution.
- *"MIMO Actuators & the Complexity of Real Robots"* — Why multi-input actuator modeling matters when your robot doesn't have a single clean motor per joint.
- *"Touch Sensors & the Next Manipulation Breakthrough"* — How MuJoCo's tactile sensor improvements are enabling the next generation of dexterous manipulation research.

---

### 2. [carla-simulator/carla](https://github.com/carla-simulator/carla)
**Tag:** `autonomous-vehicles` · **Language:** C++ · **Stars:** 14,412★

**What it is:** CARLA is an open-source simulator for autonomous driving research — built on Unreal Engine, it provides photorealistic urban environments, sensor simulations (LiDAR, camera, radar), and a robust API for building and testing autonomous driving stacks. It's the most widely used open-source driving simulator in academia and industry.

**Recent development highlights:**
- 🗓️ **Sep 2, 2026** — `Deploy UE5 nightly to Cloudflare R2` (1360bb9, @germanros1987): Major infrastructure upgrade — The Unreal Engine 5 nightly builds are now deployed to Cloudflare R2 object storage, improving global distribution and reducing setup friction for researchers using CARLA's UE5 branch. No more manual asset downloads — the simulator fetches the right build automatically.
- 🗓️ **Jul 14, 2026** — `feat(sensor): add V2X sensor family` (dd3a9d7, @JesusA-Anaya): Game-changing feature — Vehicle-to-Everything (V2X) sensor support including CAM service, path-loss models, CustomV2X, and V2I (Vehicle-to-Infrastructure) communications. This opens the door for cooperative driving and C-V2X research inside CARLA — a first for open-source driving simulators.
- 🗓️ **Jul 14, 2026** — `fix(nav): guard against null traffic light in WalkerManager` (39c4fda, @JesusA-Anaya): Robustness fix — WalkerManager now safely handles scenarios where traffic light references are null, preventing crashes in pedestrian-heavy simulations. Essential for realistic urban scenarios with complex traffic infrastructures.

🎙️ **Potential episode topics:**
- *"Inside CARLA: Building the World's Best Driving Simulator"* — A deep dive into the architecture that powers photorealistic autonomous driving simulation.
- *"V2X: When Cars Start Talking to Each Other"* — How CARLA's new V2X sensor suite enables cooperative driving research and what it means for the future of vehicle-to-infrastructure communication.
- *"UE5 in the Simulator: Why the Render Pipeline Matters"* — Why the shift to Unreal Engine 5 (and the Cloudflare R2 deployment) matters for sim-to-real transfer and photorealistic training data generation.

---

### 3. [isaac-sim/IsaacLab](https://github.com/isaac-sim/IsaacLab)
**Tag:** `robotics` · **Language:** Python · **Stars:** 8,176★

**What it is:** Isaac Lab is a unified framework for robot learning — built on NVIDIA Isaac Sim, it provides multi-physics and multi-renderer support for training robots with reinforcement learning, imitation learning, and other modern RL paradigms. It's the go-to platform for scales-up parallel robot training on GPU.

**Recent development highlights:**
- 🗓️ **Sep 20, 2026** — `[RL] Unify and cleanup isaaclab_rl for 3.0 release` (4b1234b, @MustafaH): Major release prep — The RL module is being unified and cleaned up for the upcoming v3.0 release, consolidating codepaths and modernizing the API. This signals that Isaac Lab 3.0 is on the near-term horizon.
- 🗓️ **Sep 20, 2026** — `[Scripts] Remove legacy benchmark_camera script and update documentation` (0daf5fe, @MustafaH): API modernization — Legacy benchmarking scripts are removed and documentation is updated, keeping the codebase clean and the docs current as the 3.0 release approaches.
- 🗓️ **Sep 20, 2026** — `[Tasks] Final isaaclab_tasks cleanup pass for 3.0` (0c5dcbc, @MustafaH): Release readiness — The final cleanup pass on the tasks library ensures that all robotics tasks (locomotion, manipulation, etc.) are consistent and ready for the v3.0 launch.

🎙️ **Potential episode topics:**
- *"Isaac Lab 3.0: What's Changing and Why It Matters"* — A preview of the upcoming v3.0 release and what the RL API unification means for the robot learning community.
- *"GPU-Scale Robot Training: Inside NVIDIA's Isaac Ecosystem"* — How Isaac Lab leverages massive GPU parallelism to train robots thousands of times faster than real-time.
- *"From Isaac Sim to Isaac Lab: The Modularization of Robot RL"* — Why splitting the simulation engine from the RL training framework is a game-changer for the robotics research workflow.

---

## 🎙️ About This Radar

This repo is the companion data source for the **Robotics OSS Radar** podcast — a show exploring the open-source projects shaping the future of autonomous systems and robotics. Each episode dives deep into one project, interviewing maintainers, walking through the code, and discussing what's coming next.

**Suggested episode cadence:**
| Week | Project | Theme |
|------|---------|-------|
| 1 | MuJoCo | The Physics Engine Under Every Robot Lab & MIMO Actuators |
| 2 | CARLA | Inside the World's Best Driving Simulator & V2X |
| 3 | Isaac Lab | GPU-Scale Robot Training & the Road to v3.0 |

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
| CARLA | Sep 2, 2026 | 🟢 Active (UE5 Cloudflare R2 deployment + V2X sensor family) | 14,412★ | C++ |
| IsaacLab | Sep 20, 2026 | 🟢 Active (v3.0 RL unification + task cleanup + docs update) | 8,176★ | Python |

---

*Built with 💡 and a lot of open-source love.*
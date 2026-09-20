# 🤖 Robotics OSS Radar

> Tracking the most active open-source robotics & autonomous-systems projects — with development highlights and podcast episode ideas.

---

## 📡 Projects Under the Lens

### 1. [google-deepmind/mujoco](https://github.com/google-deepmind/mujoco)
**Tag:** `robotics` · **Language:** C++ · **Stars:** 15,241★

**What it is:** MuJoCo (Multi-Joint dynamics with Contact) is the premier open-source physics simulator for robotics and embodied AI. Used by DeepMind, Stanford, MIT, and virtually every serious robotics lab, it provides fast, accurate simulation of complex rigid-body and soft-body systems — from humanoid robots to dexterous manipulation.

**Recent development highlights:**
- 🗓️ **Sep 20, 2026** — `Support multi-input (MIMO) actuators in control history buffers and mj_readCtrl` (dc8bb13, @YuvalTassa): Major framework upgrade — MIMO actuator support enables simulation of underactuated and coupled actuator systems (e.g., cable-driven robots, prosthetic limbs), expanding MuJoCo's reach into novel hardware domains.
- 🗓️ **Sep 20, 2026** — `mjx: isolate touch sensor evaluation from solver divergence in test_touch_sensor_nested_vmap` (451e66a, @YuvalTassa): Critical robustness fix — touch-sensor evaluation is now isolated from solver divergence in vectorized tests, preventing false negatives in tactile sensing research.
- 🗓️ **Sep 20, 2026** — `Normalize velocity and semi-axes in ellipsoid fluid forces and derivatives` (b9ff593, @YuvalTassa): Physics accuracy improvement — normalized fluid force computation ensures stable and physically correct simulation of ellipsoid-based fluid interactions (relevant for swimming robots and underwater manipulation).

🎙️ **Potential episode topics:**
- *"MuJoCo: The Simulator Powering the World's Best Robotics Research"* — How MuJoCo became the default physics engine for embodied AI, from DeepMind's control lab to academic labs worldwide.
- *"MIMO Actuators & the Next Generation of Underactuated Robots"* — What MIMO actuator support means for cable-driven robots, prosthetics, and novel hardware paradigms.
- *"Touch Sensors Meet Simulation: Why Isolation Matters"* — The subtle bug that could have derailed tactile sensing research, and why solver-divergence isolation is crucial for reliable simulation.

---

### 2. [carla-simulator/carla](https://github.com/carla-simulator/carla)
**Tag:** `autonomous-vehicles` · **Language:** C++ · **Stars:** 14,410★

**What it is:** CARLA is an open-source simulator for autonomous driving research — built on Unreal Engine, it provides photorealistic urban environments, sensor simulations (LiDAR, camera, radar), and a robust API for building and testing autonomous driving stacks.

**Recent development highlights:**
- 🗓️ **Sep 2, 2026** — `Deploy UE5 nightly to Cloudflare R2` (1360bb9, @germanros1987): Major infrastructure upgrade — the Unreal Engine 5 nightly builds are now deployed to Cloudflare R2 object storage, improving global distribution and reducing setup friction for researchers using CARLA's UE5 branch.
- 🗓️ **Jul 14, 2026** — `feat(sensor): add V2X sensor family` (dd3a9d7, @JesusA-Anaya): Game-changing feature — Vehicle-to-Everything (V2X) sensor support including CAM service, path-loss models, CustomV2X, and V2I (Vehicle-to-Infrastructure) communications. This opens the door for cooperative driving and C-V2X research inside CARLA.
- 🗓️ **Jul 14, 2026** — `fix(nav): guard against null traffic light in WalkerManager` (39c4fda, @JesusA-Anaya): Robustness fix — WalkerManager now safely handles scenarios where traffic light references are null, preventing crashes in pedestrian-heavy simulations.

🎙️ **Potential episode topics:**
- *"Inside CARLA: Building the World's Best Driving Simulator"* — A deep dive into the architecture that powers photorealistic autonomous driving simulation.
- *"V2X: When Cars Start Talking to Each Other"* — How CARLA's new V2X sensor suite enables cooperative driving research and what it means for the future of vehicle-to-infrastructure communication.
- *"UE5 in the Simulator: Why the Render Pipeline Matters"* — Why the shift to Unreal Engine 5 matters for sim-to-real transfer and photorealistic training data generation.

---

### 3. [autowarefoundation/autoware](https://github.com/autowarefoundation/autoware)
**Tag:** `autonomous-vehicles` · **Language:** C++ (ROS 2) · **Stars:** 12,073★

**What it is:** Autoware is the world's leading open-source software project for autonomous driving — a full-stack ROS 2-based platform covering perception, planning, control, HD mapping, and simulation. It's the reference implementation for many autonomous vehicle companies and academic labs worldwide.

**Recent development highlights:**
- 🗓️ **Sep 18, 2026** — `feat(repositories/autoware.repos): update autoware_utils to 1.11.0` (487474c, @awf-autoware-bot): Dependency bump — autoware_utils 1.11.0 brings updated math and utility functions used across the entire Autoware stack, keeping the foundation layer current.
- 🗓️ **Sep 9, 2026** — `feat(ansible): add CARLA 0.10 Town10HD_Opt map to demo_artifacts` (79446c0, @MasayaKataoka): Demo enhancement — the Town10HD_Opt map from CARLA 0.10 is now available in Autoware's demo artifacts, making it easier to spin up a full Autoware + CARLA simulation with a large, optimized urban environment.
- 🗓️ **Sep 8, 2026** — `fix(docker): build simple planning simulator with core` (87f7b60, @MeteFatihCirit): Docker fix — the simple planning simulator now builds correctly with the Autoware core image, unblocking developers who rely on Docker-based setups for rapid prototyping.

🎙️ **Potential episode topics:**
- *"Autoware: The OSS Stack for Full-Stack Autonomy"* — How Autoware went from a Toyota research project to the de facto open-source AV platform, and what's in the roadmap next.
- *"ROS 2 in Production: How Autoware Manages a Million-Line Codebase"* — The engineering challenges of maintaining a massive ROS 2 codebase with CI/CD, packaging, and dependency management at scale.
- *"Sim-to-Real with Autoware + CARLA"* — How the integration between Autoware's planning stack and CARLA's simulation environment accelerates the path from simulation to real-world deployment.

---

## 🎙️ About This Radar

This repo is the companion data source for the **Robotics OSS Radar** podcast — a show exploring the open-source projects shaping the future of autonomous systems and robotics. Each episode dives deep into one project, interviewing maintainers, walking through the code, and discussing what's coming next.

**Suggested episode cadence:**
| Week | Project | Theme |
|------|---------|-------|
| 1 | MuJoCo | The Physics Engine Powering Embodied AI & MIMO Actuators |
| 2 | CARLA | Inside the World's Best Driving Simulator & V2X |
| 3 | Autoware | The OSS Stack for Full-Stack Autonomy & Sim-to-Real |

---

## 🔧 How to Contribute

- Found a stale project? Open an issue with the repo URL and what you expected to see.
- Want your project featured? Submit a link and a 2-line description.
- Episode ideas? The issue tracker is the place.

---

## 📊 Radar Dashboard

| Project | Last Commit | Activity | Stars | Language |
|---------|-------------|----------|-------|----------|
| MuJoCo | Sep 20, 2026 | 🟢 Active (MIMO actuators + touch sensor isolation + fluid physics) | 15,241★ | C++ |
| CARLA | Sep 2, 2026 | 🟢 Active (UE5 infra + V2X sensor family + nav robustness) | 14,410★ | C++ |
| Autoware | Sep 18, 2026 | 🟢 Active (dependency bumps + CARLA map integration + Docker fix) | 12,073★ | C++ (ROS 2) |

---

*Built with 💡 and a lot of open-source love.*
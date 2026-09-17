# 🤖 Robotics & Autonomous Systems — Open-Source Radar

> A living radar for the most active open-source robotics and autonomous-vehicles repos, with commit summaries distilled from live `git log` inspection and podcast episode ideas for **Robotics OSS**.

_Last scan: 2026-09-17 · Sources: GitHub topic search on `autonomous-vehicles` & `robotics`, sorted by recent activity, followed by per-repo latest-commit inspection._

---

## 🔥 Top 3 Most Recently Active Repos

### 1. [gazebosim / gz-sim](https://github.com/gazebosim/gz-sim)
⭐ 1,504 stars · 💻 C++ · 📄 [Apache-2.0](https://github.com/gazebosim/gz-sim/blob/main/LICENSE)

**About:** Gazebo is the most widely used open-source robotics simulator. The next-generation engine (Gazebo Harmonic / gz-sim) powers simulation for research, education, and industrial robotics — from warehouse bots to humanoids. It integrates with ROS 2 seamlessly and supports realistic sensor models, multi-robot scenarios, and plugin-based extensibility.

**Latest Commits (Sep 15–17, 2026):**
- `6cdb9b3` — `JointStatePublisher: build joint message once, update fields in place` (#3853) *(9/17)* — Performance optimization: reuse the JointState message instead of reconstructing it each time.
- `7a6d8c4` — `ECM Implementation with Entt` (#3447) *(9/15)* — A major architectural shift: a new Entity-Component-Manager built on the [EnTT](https://github.com/skypjack/entt) ECS library, modernizing how simulation entities are managed.
- `f33f82e` — `Fix: Preserve PYTHONPATH in INTEGRATION_python_system_loader` (#3890) *(9/15)* — Python sandboxing fix ensuring correct module resolution in plugin-loaded Python systems.

**What's Cooking:** gz-sim is undergoing a **fundamental architecture overhaul**. The new ECM built on EnTT replaces the legacy component system, promising faster entity lookups, cleaner plugin APIs, and better alignment with modern C++ ECS patterns. Meanwhile, performance optimizations in state publishing and Python sandbox reliability fixes show a project maturing under heavy community use.

**🎙️ Episode Ideas:**
- *"From Entity-Component to Robot PHD: Inside Gazebo's ECM Overhaul"* — why the simulation engine switched to EnTT and what it means for robotics developers.
- *"Speedin' Up State Publishing: Micro-Optimizations That Matter at Scale"* — the art of avoiding redundant copies in real-time simulation loops.
- *"Python Plugins & Sandbox Escapes: Keeping Simulation Safe"* — how gz-sim isolates user code and what can go wrong.

---

### 2. [autowarefoundation / autoware_universe](https://github.com/autowarefoundation/autoware_universe)
⭐ 1,756 stars · 💻 C++ · 📄 [Apache-2.0](https://github.com/autowarefoundation/autoware_universe/blob/main/LICENSE)

**About:** Autoware is the world's first open-source software stack for autonomous driving. The unified repo (`autoware_universe`) aggregates all sub-projects — perception, planning, control, mapping, and simulation — into a single, continuously integrated codebase. It's backed by the Autoware Foundation and used in production autonomy stacks worldwide.

**Latest Commits (Sep 17, 2026):**
- `3886fd6` — `feat(autoware_topic_relay_controller): add throttle mode` (#13395) — New throttle-mode support in the topic relay controller, enabling actuator command passthrough for testing and development.
- `9ff8961` — `fix(pid_long): fix slope sign` (#13247) — Critical bugfix correcting the slope sign in the longitudinal PID controller, which directly impacts vehicle stability on grades.
- `d52d236` — `feat(autoware_traffic_light_pipeline): add traffic_light_recognition node` (#13367) — A new perception node dedicated to traffic-light recognition, expanding the existing pipeline.

**What's Cooking:** Autoware is shipping **real production fixes alongside new features**. The slope sign bug in the PID controller is the kind of bug that could cause real-world safety issues — finding and fixing it shows the project's maturity. The traffic-light recognition node adds a new perception capability, and the throttle mode in the relay controller improves the development/testing workflow. This is a "hitting stride" release cycle.

**🎙️ Episode Ideas:**
- *"The Bug That Could've Caused a Crash: Inside Autoware's Slope Sign Fix"* — how a sign error in a PID controller could destabilize a vehicle on a hill, and how the community caught it.
- *"Traffic Lights, Please! Autoware's New Perception Node"* — building a dedicated traffic-light recognition pipeline from sensor fusion to launch.
- *"Throttle Mode & the Development Sandwich: Testing Autonomy Safely"* — how relay controllers and simulated actuator commands speed up AV development without endangering anyone.

---

### 3. [carla-simulator / carla](https://github.com/carla-simulator/carla)
⭐ 14,404 stars · 💻 C++ · 📄 [MIT](https://github.com/carla-simulator/carla/blob/master/LICENSE)

**About:** CARLA is the go-to open-source simulator for autonomous-driving research — built on Unreal Engine, it provides high-fidelity sensor simulation (LiDAR, camera, radar), urban scenarios, and a rich API for benchmarking perception, planning, and control stacks. Used by academic labs, OEMs, and startups worldwide.

**Latest Commits (Jul 2, 2026):**
- `1360bb9` — `Deploy UE5 nightly to Cloudflare R2` (#9859) — Automated CI pipeline that pushes Unreal Engine 5 nightly builds to Cloudflare R2 object storage, enabling cloud-based simulation and distribution.
- `0a5ce0d` — `Fix lidar smoke helper signature` (#9791) — Corrects a parameter mismatch in the LiDAR sensor's smoke rendering helper, fixing visual artifacts.
- `39c4fda` — `fix(nav): guard against null traffic light in WalkerManager` (#9758) — Defensive null-pointer check in the pedestrian (Walker) manager's navigation code, preventing crashes when traffic-light references are missing.

**What's Cooking:** CARLA's recent work focuses on **cloud-deployable simulation infrastructure** and **robustness hardening**. The UE5 nightly-to-R2 pipeline is a CI breakthrough that lets researchers pull the latest Unreal integration without rebuilding from scratch. Defensive programming fixes (null traffic-light guard, LiDAR signature fix) show a codebase being battle-tested for automation and headless runs.

**🎙️ Episode Ideas:**
- *"From UE5 to the Cloud: CARLA's R2 Deployment Pipeline"* — how automated nightly builds to object storage are changing how researchers get simulation assets.
- *"When the Traffic Light Disappears: Null-Safety in AV Stack Code"* — the hidden crash sinks that only appear in simulation at 3 AM.
- *"LiDAR Smoke & Sensor Debugging: The Visual Tools Making Sim Sensors Trustworthy"* — why rendering helpers matter for validating sensor models.

---

## 🎙️ About This Radar

Curated for the **Robotics OSS** podcast and refreshed periodically. Selection priorities:
- Genuine open-source robotics / autonomous-vehicle projects
- Active recent commit cadence (truly "being worked on")
- Strong narrative potential for podcast episodes

See the companion issue **[Projects to Revisit & Upcoming Releases](#)** for the tracking checklist.

---

## 🔎 How to Use

1. Scan the **Top 3** above for current development highlights.
2. Pick an episode idea that resonates.
3. Check the companion issue for follow-up items (revisit dates, upcoming releases to watch).

---

_Licensed as part of the open-source robotics podcast ecosystem. Contributions and episode suggestions welcome._
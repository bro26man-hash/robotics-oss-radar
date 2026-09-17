# 🤖 Robotics & Autonomous Systems — Open-Source Radar

> A living radar for the most active open-source robotics and autonomous-vehicles repos, with commit summaries distilled from live `git log` inspection and podcast episode ideas for **Robotics OSS**.

_Last scan: 2026-09-17 · Sources: GitHub topic search on `autonomous-vehicles` & `robotics`, sorted by recent activity, followed by per-repo latest-commit inspection._

---

## 🔥 Top 3 Most Recently Active Repos

### 1. [commaai / openpilot](https://github.com/commaai/openpilot)
⭐ 63,671 stars · 💻 C++ · 📄 [Apache-2.0](https://github.com/commaai/openpilot/blob/master/LICENSE)

**About:** openpilot is an open-source operating system for robotics — currently upgrading the driver-assistance system on 300+ supported production vehicles. It's one of the most starred robotics repos on GitHub and the backbone of comma.ai's research into open autonomous driving.

**Latest Commits (Sep 16–17, 2026):**
- `bd176cb` — ui: remove question marks (#38938) *(9/17)*
- `4d9d1bc` — ui: not paired bookmark alert (#38936) *(9/17)*
- `cab5343` — AGNOS 19.8 release (#38935) *(9/17)*
- `6080cc6` — Use a precompiled eGPU driving model (#38930) *(9/16)*
- `81ae1a2` — Use tinygrad generic ONNX compiler artifacts (#38926) *(9/16)*

**What's Cooking:** openpilot is in the middle of a **model-compilation revolution**. The team is shipping precompiled eGPU driving-model artifacts using the tinygrad ONNX compiler — a major step toward reproducible, hardware-accelerated model runs on comma's custom hardware. The AGNOS 19.8 release is landing alongside UI polish (removing question marks, adding pairing alerts). Expect a big wave of community testing as new builds roll out to devices in the field.

**🎙️ Episode Ideas:**
- *"63K Stars and No Google: Inside openpilot's Open-Source AV Stack"* — how comma.ai built the most-starred robotics repo without any automaker backing.
- *"eGPU Driving Models & tinygrad: The Compiler Wars Come to Cars"* — precompiled model artifacts and what they mean for on-device inference.
- *"AGNOS: comma's Secret Operating System for Vehicles"* — the release cycle, the custom hardware, and why it matters.

---

### 2. [carla-simulator / carla](https://github.com/carla-simulator/carla)
⭐ 14,403 stars · 💻 C++ · 📄 [MIT](https://github.com/carla-simulator/carla/blob/master/LICENSE)

**About:** CARLA is the go-to open-source simulator for autonomous-driving research — built on Unreal Engine, it provides high-fidelity sensor simulation (LiDAR, camera, radar), urban scenarios, and a rich API for benchmarking perception, planning, and control stacks.

**Latest Commits (Jul 10–Sep 2, 2026):**
- `1360bb9` — Deploy UE5 nightly to Cloudflare R2 (#9859) *(9/2)*
- `0a5ce0d` — Fix lidar smoke helper signature *(7/14)*
- `39c4fda` — fix(nav): guard against null traffic light in WalkerManager *(7/14)*
- `dd3a9d7` — feat(sensor): add V2X sensor family — CAM service, path-loss, CustomV2X, V2I *(7/13)*
- `6279162` — feat(cmake): add CARLA_MAPS_TO_COOK for packaged maps *(7/10)*

**What's Cooking:** CARLA is pushing hard on **V2X communication simulation** — a new sensor family covers C-V2X (Cellular Vehicle-to-Everything), including path-loss modeling and V2I/V2V message exchange. The UE5 nightly deployment to Cloudflare R2 means cloud-based simulation is becoming a first-class use case. Navigation fixes (null traffic-light guard) and map-packaging tooling round out a busy cycle that bridges real-world connectivity and realistic urban simulation.

**🎙️ Episode Ideas:**
- *"Simulating the Connected Car: CARLA's V2X Sensor Family"* — why vehicle-to-everything simulation matters for AV safety validation.
- *"From Unreal Engine to Cloudflare: Cloud-Based Autonomous Driving Simulation"* — the R2 deployment and the future of remote sim infrastructure.
- *"The traffic_light that Wasn't There: Defensive Programming in AV Simulators"* — null-pointer safety in autonomous-stack simulation.

---

### 3. [isaac-sim / IsaacLab](https://github.com/isaac-sim/IsaacLab)
⭐ 8,151 stars · 💻 Python · 📄 [Apache-2.0](https://github.com/isaac-sim/IsaacLab/blob/main/LICENSE)

**About:** Isaac Lab is NVIDIA's unified framework for robot learning — built on Isaac Sim's multi-physics simulation renderer, it gives researchers an end-to-end environment for training, evaluating, and deploying robot policies via RL, imitation learning, and world models.

**Latest Commits (Sep 16–17, 2026):**
- `237fe2b` — [CI][Auto Version Bump] Compile changelog fragments (schedule) *(9/17)*
- `7a7575d` — [Docs] Fix develop README documentation links (#7770) *(9/16)*
- `8b58e0c` — [CI] Prepare develop as repository and docs default *(9/16)*
- `94a8ad5` — [Bump] Bump Newton to 1.6.0 *(9/16)*
- `0c12bab` — Avoid Newton VBD graph coloring hangs *(9/16)*

**What's Cooking:** Isaac Lab is in a **release-cadence sprint** — auto version-bumping and changelog compilation signal a mature CI pipeline gearing up for the next stable release. The Newton physics engine just bumped to 1.6.0 with a fix for VBD (Velocity-Based Dynamics) graph-coloring hangs — a performance issue that could stall large-scale parallel simulation. Docs are being cleaned up for the develop branch, suggesting a documentation refresh alongside the upcoming Isaac Lab release.

**🎙️ Episode Ideas:**
- *"Newton 1.6: The Physics Engine Behind Robot Learning at Scale"* — VBD, graph coloring, and why physics simformance matters for RL.
- *"Training a Robot in a Simulator: Inside Isaac Lab's Pipeline"* — from URDF to trained policy, end-to-end.
- *"NVIDIA's Playbook for Open-Source Robot Learning"* — how Isaac Lab fits into the broader Isaac ecosystem and the AV research stack.

---

## 🎙️ About This Radar

Curated for the **Robotics OSS** podcast and refreshed periodically. Selection priorities:
- Genuine open-source robotics / autonomous-vehicle projects
- Active recent commit cadence (truly "being worked on")
- Strong narrative potential for podcast episodes

See the companion issue **[Projects to Revisit & Upcoming Releases](../../issues/13)** for the tracking checklist.

---

## 🔎 How to Use

1. Scan the **Top 3** above for current development highlights.
2. Pick an episode idea that resonates.
3. Check the companion issue for follow-up items (revisit dates, upcoming releases to watch).

---

_Licensed as part of the open-source robotics podcast ecosystem. Contributions and episode suggestions welcome._
# 🤖 Robotics OSS Radar

> Tracking the most active open-source robotics & autonomous-systems projects — with development highlights and podcast episode ideas.

---

## 📡 Projects Under the Lens

### 1. [commaai/openpilot](https://github.com/commaai/openpilot)
**Tag:** `robotics` · **Language:** Python · **Stars:** 63,682★

**What it is:** openpilot is an operating system for robotics — currently it upgrades the driver assistance system on 300+ supported cars. It's the most-starred open-source project in our radar and a cornerstone of the OE (open piloting) movement.

**Recent development highlights:**
- 🗓️ **Sep 19, 2026** — `cabana: generate dbc files during builds` (1b1b60b, @TreyMoen): Automates DBC file generation in the cabana debugging tool — critical for parsing CAN bus signals across 300+ supported vehicle variants without manual effort.
- 🗓️ **Sep 19, 2026** — `cabana: brighten quiet signals in dark mode` (d375e7f, @TreyMoen): UI polish — improved signal readability in dark mode by adjusting brightness clamps, making it easier to spot subtle CAN signals during debugging.
- 🗓️ **Sep 19, 2026** — `cabana: refine signal heatmap grid` (95ed021, @TreyMoen): Visualization upgrade for the signal heatmap, helping developers quickly identify which CAN signals are active and which are noisy.

🎙️ **Potential episode topics:**
- *"Open Piloting at Scale"* — How openpilot went from a weekend project to 300+ car support and what that means for the future of ADAS.
- *"The cabana Debugging Lifeline"* — Inside openpilot's tools that let developers and users see exactly what the car is thinking on the CAN bus.
- *"DBC Files & the CAN Bus Maze"* — Why automated signal parsing matters when you support hundreds of different car models.

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
| 1 | openpilot | Open Piloting at Scale & the CAN Bus Debugging Lifeline |
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
| openpilot | Sep 19, 2026 | 🟢 Active (cabana DBC automation + UI polish) | 63,682★ | Python |
| CARLA | Sep 2, 2026 | 🟢 Active (UE5 infra + V2X sensor family) | 14,410★ | C++ |
| Autoware | Sep 18, 2026 | 🟢 Active (dependency bumps + CARLA map integration) | 12,073★ | C++ |

---

*Built with 💡 and a lot of open-source love.*
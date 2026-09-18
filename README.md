# 🤖 Robotics OSS Radar

> Open-source robotics & autonomous systems radar — tracking the most active projects, recent development highlights, and podcast episode ideas.

## 📡 Tracked Projects

We monitor three flagship open-source projects at the intersection of robotics and autonomous vehicles. Here's what's happening right now:

---

### 1. 🚗 [commaai/openpilot](https://github.com/commaai/openpilot)
**⭐ 63,675 stars | Python**

> *openpilot is an operating system for robotics. Currently, it upgrades the driver assistance system on 300+ supported cars.*

**Recent Development Highlights (as of Sep 17, 2026):**

| Commit | What's Happening |
|---|---|
| `1328ace` — Remove model chunking & use LFS for Chestnut releases | Refactoring model storage — switching from chunked files to Git LFS for the new "Chestnut" release, streamlining CI and download sizes. |
| `cd1490a` — modeld: 2× faster chestnut build | **Big performance win** — the model inference engine (`modeld`) build time cut in half for the Chestnut release. Faster iteration for contributors. |
| `7db7735` — rm chestnut power test | Cleaning up experimental power-test scripts that were only needed during hardware validation. |
| `bd176cb` — ui: remove question marks | UI polish — removing deprecated help icons from the interface. |
| `4d9d1bc` — ui: not paired bookmark alert | New UX feature: alerts drivers when their phone bookmark isn't paired correctly. |

**🎙️ Potential Podcast Episode Topics:**
- *"Why commaai Switched to Git LFS for Model Releases"* — A deep-dive into how they manage 5GB+ model files at scale.
- *"2× Faster Builds: Inside the modeld Optimization"* — What CI/CD tricks enabled a 2× speedup in model compilation.
- *"300+ Cars on One Open-Source Stack"* — How openpilot maintains compatibility across an enormous vehicle matrix.
- *"Chestnut on the Horizon: What's Next for openpilot?"* — Roadmap discussion with the community.

---

### 2. 🧠 [ApolloAuto/apollo](https://github.com/ApolloAuto/apollo)
**⭐ 26,830 stars | C++**

> *An open autonomous driving platform*

**Recent Development Highlights (as of Feb 28, 2026):**

| Commit | What's Happening |
|---|---|
| `539f546` — feat: add Apollo 11.0 bev+occ | **Major release** — Apollo 11.0 introduces **Bird's-Eye-View (BEV) + Occupancy (OCC)** perception pipelines. This is a leap in 3D scene understanding for autonomous driving. |
| `40c8a01` — Recover Seyond lidar driver | Lidar hardware support restored — re-enabling compatibility with the Seyond lidar line after a driver regression. |
| `d53aa3d` — docs: fix README build status badges | Maintenance cleanup — removing stale CI badges from the README. |
| `6680288` / `995b75a` — Seyond lidar driver config & readme updates | Documentation improvements for lidar integration, making it easier for new users to configure hardware. |

**🎙️ Potential Podcast Episode Topics:**
- *"BEV + OCC: How Apollo 11.0 Changes the Perception Game"* — What Bird's-Eye-View and Occupancy networks mean for the future of autonomous driving stacks.
- *"Open-Source Autonomous Driving at Baidu Scale"* — The story behind Apollo, from internal Baidu project to the world's leading open autonomous driving platform.
- *"When Lidar Drivers Break: Hardware Compatibility in Open Source"* — Lessons from the Seyond lidar regression and recovery.
- *"Apollo vs. Autoware: Two Giants, Two Philosophies"* — A comparative episode on China's Apollo and the Autoware Foundation.

---

### 3. 🌍 [carla-simulator/carla](https://github.com/carla-simulator/carla)
**⭐ 14,405 stars | C++**

> *Open-source simulator for autonomous driving research.*

**Recent Development Highlights (as of Sep 2, 2026):**

| Commit | What's Happening |
|---|---|
| `1360bb9` — Deploy UE5 nightly to Cloudflare R2 | **Infrastructure upgrade** — CARLA's Unreal Engine 5 nightlies are now served via Cloudflare R2, dramatically improving global download reliability and speed. |
| `dd3a9d7` — feat(sensor): add V2X sensor family (CAM, path-loss, CustomV2X, V2I) | **New sensor suite** — added a full **Vehicle-to-Everything (V2X)** sensor family, enabling communication-aware simulations. This is huge for connected/autonomous vehicle research. |
| `0a5ce0d` — Fix lidar smoke helper signature | Bug fix for lidar rendering helpers — ensuring correct point-cloud visualization in debug sessions. |
| `39c4fda` — guard against null traffic light in WalkerManager | Robustness fix — WalkerManager (pedestrian/AI traffic controller) no longer crashes when traffic light entities are missing. |
| `6279162` — add CARLA_MAPS_TO_COOK to select packaged maps | Build system improvement — developers can now selectively cook packaged maps via CMake option, reducing build times for minimal installations. |

**🎙️ Potential Podcast Episode Topics:**
- *"V2X in Simulation: Why CARLA's New Sensor Family Changes Everything"* — How Vehicle-to-Everything simulation enables research into connected autonomy that was impossible before.
- *"From UE4 to UE5: The CARLA Graphics Overhaul"* — What migrating to Unreal Engine 5 means for photorealistic autonomous driving simulation.
- *"Cloudflare R2 vs. S3: How CARLA Scaled Global Downloads"* — A practical episode on infrastructure choices for open-source projects with large binary assets.
- *"Sim-to-Real: Can CARLA's V2X Predictions Transfer to the Real World?"* — The eternal simulation-to-reality gap, and whether V2X adds new capabilities or new uncertainties.

---

## 📋 Episode Planning Checklist

| # | Project | Episode Idea | Status |
|---|---|---|---|
| 1 | commaai/openpilot | "Why commaai Switched to Git LFS for Model Releases" | 🔴 Not started |
| 2 | commaai/openpilot | "2× Faster Builds: Inside the modeld Optimization" | 🔴 Not started |
| 3 | ApolloAuto/apollo | "BEV + OCC: How Apollo 11.0 Changes the Perception Game" | 🔴 Not started |
| 4 | ApolloAuto/apollo | "Open-Source Autonomous Driving at Baidu Scale" | 🔴 Not started |
| 5 | carla-simulator/carla | "V2X in Simulation: Why CARLA's New Sensor Family Changes Everything" | 🔴 Not started |
| 6 | carla-simulator/carla | "From UE4 to UE5: The CARLA Graphics Overhaul" | 🔴 Not started |

---

## 🔗 Quick Links

- [commaai/openpilot](https://github.com/commaai/openpilot)
- [ApolloAuto/apollo](https://github.com/ApolloAuto/apollo)
- [carla-simulator/carla](https://github.com/carla-simulator/carla)

## 📌 How This Repo Works

This repo is a **living tracker** for the *Robotics OSS Radar* podcast. We:

1. **Monitor** the most active open-source robotics & autonomous-vehicle repos on GitHub.
2. **Log** recent commits and development highlights.
3. **Brainstorm** podcast episode topics tied to real code changes.
4. **Track** upcoming releases and milestones to revisit.

Contributions are welcome! Open an issue to suggest a new project or episode idea.

---

*Built for makers, by makers. 🛠️*
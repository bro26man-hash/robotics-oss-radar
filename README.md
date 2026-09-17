# 🤖 Robotics & Autonomous Systems — Open-Source Radar

> A living radar for the most active open-source robotics and autonomous-vehicles repos, with commit summaries distilled from live `git log` inspection and podcast episode ideas for **Robotics OSS**.

_Last scan: 2026-09-17 · Sources: GitHub topic search on `autonomous-vehicles` & `robotics`, sorted by recent activity, followed by per-repo latest-commit inspection._

---

## 🔥 Top 3 Most Recently Active Repos

### 1. [autowarefoundation / autoware_universe](https://github.com/autowarefoundation/autoware_universe)
⭐ 1,756 stars · 💻 C++

**About:** Autoware Universe is the world's leading open-source autonomous driving software stack. It provides a modular, extensible framework for perception, planning, control, and driver abstraction — built on ROS 2 and designed for real-world deployment.

**Latest Commits (Sep 16–17, 2026):**
- `d52d236` — feat(autoware_traffic_light_pipeline): add traffic_light_recognition node *(9/17)*
- `d7d242d` — fix(mission_planner): guard against empty planned path to prevent SIGSEGV *(9/17)*
- `a071cee` — fix(autoware_system_monitor): migrate deprecated NVML APIs for CUDA 13 *(9/17)*
- `956e938` — refactor(autoware_topic_relay_controller): migrate to agnocast_wrapper::Node *(9/16)*
- `9d3d964` — fix(design): align the vehicle node designs with the packages they build *(9/16)*

**What's Cooking:** The team is deep in a **hardware-abstraction migration** — moving legacy NVIDIA NVML API calls to the new `agnocast_wrapper::Node` interface (ROS 2 compatibility layer), while simultaneously hardening the mission planner against crash conditions and adding a dedicated traffic-light recognition node. This is a pivotal moment: Autoware is modernizing its driver abstraction layer while expanding perception capabilities.

**🎙️ Episode Ideas:**
- *"Migrating a Million-Line AV Stack to a New Hardware Abstraction"* — the `agnocast_wrapper::Node` transition and why it matters.
- *"From Traffic Lights to Crash Guards: Hardening an Autonomous Stack"* — how perception and planning robustness go hand-in-hand.
- *"Autoware Universe: The World's Open-Source Driving Brain"* — an overview of the stack and its role in the AV ecosystem.

---

### 2. [cyberbotics / webots](https://github.com/cyberbotics/webots)
⭐ 4,634 stars · 💻 C++

**About:** Webots is a mature, open-source 3D robot simulator with a long history dating back to the 1990s. It supports a vast library of robot models ( wheeled, legged, aerial, manipulators) and is widely used in education, research, and industry prototyping.

**Latest Commits (Sep 11–16, 2026):**
- `d2ba706` — fix-controller-pose-cache-removal *(9/16)*
- `777eee4` — Merge pull request #7018: sync released bc0f6e839 *(9/12)*
- `a6f0361` — Merge branch 'master' into sync-released branch *(9/12)*
- `bc0f6e8` — Fix regex patterns for websocket rules in documentation *(9/11)*
- `c1dc211` — Fix relative texture URLs in web streaming *(9/11)*

**What's Cooking:** Activity is Focused on **stability and portability** — a controller pose-cache removal (likely a long-standing rendering bug), a branch sync for a released version (indicating an upcoming or recent stable release), and documentation fixes for WebSocket and texture-loading edge cases in web-streamed simulations. The cadence suggests a maintenance/quality-release cycle.

**🎙️ Episode Ideas:**
- *"Webots at 30: How a '90s Simulator Still Leads Robotic Simulation"* — history, philosophy, and why it endures.
- *"Web Streaming Your Robot: The Rise of Browser-Based Sim"* — web streaming, WebSocket rule fixes, and cloud robotics.
- *"Controller Caches, Texture URLs, and the Hidden Bugs of Simulation"* — what it takes to keep a simulator reliable at scale.

---

### 3. [autowarefoundation / autoware_core](https://github.com/autowarefoundation/autoware_core)
⭐ 186 stars · 💻 C++

**About:** Autoware Core is the foundational layer of the Autoware ecosystem — low-level perception, localization, planning, and control nodes that powers autonomous vehicle prototypes. It's the engine beneath Autoware Universe's higher-level abstractions.

**Latest Commits (Sep 14–17, 2026):**
- `11f8749` — test(autoware_gnss_poser): characterize orientation, antenna TF composition and covariance *(9/17)*
- `cfac5ee` — feat(api, motion_velocity_planner): add the node designs required by the AD API and motion planning design modules *(9/17)*
- `017dbf7` — perf(autoware_lanelet2_utils): improve LaneletRTree::get_closest_lanelet *(9/15)*
- `41b16df` — test(gyro_odometer): reorganized test suite *(9/15)*
- `42d6b69` — feat(map_height_fitter, pose_initializer, adapi_adaptors): move the nodes to agnocast_wrapper::Node *(9/14)*

**What's Cooking:** Core is mirroring Universe's **`agnocast_wrapper::Node` migration** at the lower level — moving foundational nodes (map-height-fitter, pose-initializer, ADAPI adaptors) to the new abstraction. Meanwhile, GPS/IMU sensor characterization is being formalized into tests, and the motion planner is being redesigned around a new AD API spec. Lanelet2 lookup performance is also getting a boost. This is the foundational modernization of the entire stack.

**🎙️ Episode Ideas:**
- *"The Layer Beneath the Stack: Inside Autoware Core"* — how foundational perception and localization modules are engineered.
- *"When the Foundation Migrates: Coordinating a refactor Across a Full AV Stack"* — the agnocast_wrapper rollout and its challenges.
- *"Lanelet2 at Speed: Performance Engineering for HD Map Lookups"* — spatial-indexing optimizations in autonomous driving.

---

## 🎙️ About This Radar

Curated for the **Robotics OSS** podcast and refreshed periodically. Selection priorities:
- Genuine open-source robotics / autonomous-vehicle projects
- Active recent commit cadence (truly "being worked on")
- Strong narrative potential for podcast episodes

See the companion issue **[Projects to Revisit & Upcoming Releases](../../issues/1)** for the tracking checklist.

---

## 🔎 How to Use

1. Scan the **Top 3** above for current development highlights.
2. Pick an episode idea that resonates.
3. Check the companion issue for follow-up items (revisit dates, upcoming releases to watch).

---

_Licensed as part of the open-source robotics podcast ecosystem. Contributions and episode suggestions welcome._

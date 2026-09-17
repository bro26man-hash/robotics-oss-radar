# 🤖 Robotics OSS Radar

> A living radar tracking the most active open-source robotics and autonomous-vehicle repositories — built for the **Robotics OSS Podcast**.

This repo is our HQ for monitoring top-tier open-source projects, documenting recent development highlights, and brainstorming episode topics.

---

## 📡 Tracked Projects

### 1. [Autoware Universe](https://github.com/autowarefoundation/autoware_universe)
**Owner:** autowarefoundation | **Language:** C++ | **License:** Apache-2.0 | **Stars:** ⭐ 1,756 | **Forks:** 🍴 964

The extension layer of the Autoware ecosystem — a massive collection of ROS packages that supercharge Autoware Core with advanced autonomous-driving capabilities.

**Package domains:** Common · Control · Evaluator · Localization · Map · Perception · Planning · Sensing · Simulator · System · Vehicle

#### 🔬 Recent Development Highlights
| Commit | Description | Date |
|--------|-------------|------|
| `d52d236` | Added `traffic_light_recognition` node to autoware_traffic_light_pipeline | 2026-09-17 |
| `d7d242d` | Guarded mission_planner against empty planned path (SIGSEGV fix) | 2026-09-17 |
| `a071cee` | Migrated deprecated NVML APIs for CUDA 13 compatibility | 2026-09-17 |
| `956e938` | Refactored autoware_topic_relay_controller to agnocast_wrapper::Node | 2026-09-16 |
| `9d3d964` | Aligned vehicle node designs with the packages they build | 2026-09-16 |

#### 🎙️ Potential Episode Topics
- **Traffic Light Recognition Pipeline** — How Autoware Universe is adding dedicated perception nodes for signal detection
- **Safety-Critical Fixes** — Preventing SIGSEGVs in mission planning: what it means for real-world deployment
- **CUDA 13 Migration** — Keeping huge C++ codebases current with GPU driver stacks
- **Agnocast Migration** — The shift from ros2 topic relay to agnocast communication middleware
- **Vehicle Interface Standardization** — Designing vehicle nodes that cleanly map to their packages

---

### 2. [Autoware Core](https://github.com/autowarefoundation/autoware_core)
**Owner:** autowarefoundation | **Language:** C++ | **License:** Apache-2.0 | **Stars:** ⭐ 186 | **Forks:** 🍴 167

The stable, minimal core of Autoware — a curated set of high-quality ROS packages for autonomous driving. Currently a thin layer; the real action happens in Universe and will port over once the Core/Universe interface freeze is resolved.

#### 🔬 Recent Development Highlights
| Commit | Description | Date |
|--------|-------------|------|
| `11f8749` | Characterized GNSS poser: orientation, antenna TF, and covariance | 2026-09-17 |
| `cfac5ee` | Added node designs required by the AD API & motion planning design modules | 2026-09-17 |
| `017dbf7` | Improved LaneletRTree::get_closest_lanelet performance | 2026-09-15 |
| `41b16df` | Reorganized gyro_odometer test suite | 2026-09-15 |
| `42d6b69` | Moved map_height_fitter, pose_initializer, adapi_adaptors to agnocast_wrapper::Node | 2026-09-14 |

#### 🎙️ Potential Episode Topics
- **Core vs. Universe Architecture Debate** — Why does Autoware split into two, and what's the philosophy?
- **GNSS Poser Characterization** — How precise sensor calibration kills drift in localization
- **AD API & Motion Planning Interface** — The design modules shaping the next generation of driving stacks
- **Lanelet2 Performance Optimization** — Spatial indexing tricks for HD map queries
- **Agnocast Adoption Across the Ecosystem** — How communication middleware choices ripple through the community

---

### 3. [Webots Robot Simulator](https://github.com/cyberbotics/webots)
**Owner:** cyberbotics | **Language:** C++ | **License:** Apache-2.0 | **Stars:** ⭐ 4,634 | **Forks:** 🍴 2,057

A full-featured open-source robot simulator — model, program, and simulate robots, vehicles, and mechanical systems. Originally designed at EPFL in 1996, open-sourced in 2018.

#### 🔬 Recent Development Highlights
| Commit | Description | Date |
|--------|-------------|------|
| `d2ba706` | Fixed controller pose cache removal logic | 2026-09-16 |
| `777eee4` | Merged sync-released branch (release pipeline update) | 2026-09-12 |
| `bc0f6e8` | Fixed regex patterns for websocket rules in documentation | 2026-09-11 |
| `c1dc211` | Fixed relative texture URLs in web streaming | 2026-09-11 |

#### 🎙️ Potential Episode Topics
- **Web Streaming & Texture Fix** — How simulators are evolving for cloud-based and browser-powered robotics
- **Pose Cache Architecture** — Why cached transforms matter for real-time simulation fidelity
- **Release Pipeline Automation** — Sync-release branches and how large sim projects manage CI/CD
- **Webots in Education & Research** — 25+ years of robotics simulation and why it still matters
- **Open-Source Simulation vs. Gazebo/Ignition** — Competitive landscape and where Webots shines

---

## 📊 Comparison Matrix

| Project | Stars | Language | Focus Area | Activity Level |
|---------|-------|----------|------------|---------------|
| [Autoware Universe](https://github.com/autowarefoundation/autoware_universe) | 1,756 | C++ | AV perception/planning/control extensions | 🔥 Daily commits |
| [Autoware Core](https://github.com/autowarefoundation/autoware_core) | 186 | C++ | Foundational AV ROS packages | 📅 Daily commits |
| [Webots](https://github.com/cyberbotics/webots) | 4,634 | C++ | Robot simulation & virtual testing | 📅 Daily commits |

---

## 🗓️ Podcast Workflow

1. **Weekly sweep** — Pull latest commits from each repo
2. **Highlight extraction** — Summarize what changed and why it matters
3. **Episode brainstorming** — Add topics to this README or open an issue
4. **Release tracking** — Use the issue tracker for upcoming releases

---

## 📋 Quick Links

| Project | GitHub | Docs |
|---------|--------|------|
| Autoware Universe | [github.com/autowarefoundation/autoware_universe](https://github.com/autowarefoundation/autoware_universe) | [autoware_universe docs](https://autowarefoundation.github.io/autoware_universe/) |
| Autoware Core | [github.com/autowarefoundation/autoware_core](https://github.com/autowarefoundation/autoware_core) | [autoware_core docs](https://autowarefoundation.github.io/autoware_core/) |
| Webots | [github.com/cyberbotics/webots](https://github.com/cyberbotics/webots) | [Cyberbotics docs](https://cyberbotics.com/doc/reference/index) |

---

_🔄 Last updated: September 2026 · Radar refreshed weekly_
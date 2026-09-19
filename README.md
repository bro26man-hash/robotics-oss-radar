# 🚗 Robotics OSS Radar

> A living research hub tracking the most active open-source robotics & autonomous systems projects — curated for the podcast

This repo is the **companion radar** for the *Robotics OSS Radar* podcast. We monitor the most recently active, high-impact open-source projects in robotics and autonomous vehicles, surface their latest development highlights, and generate episode topics for each.

---

## 📡 Tracked Projects

### 1. [commaai/openpilot](https://github.com/commaai/openpilot)
| | |
|---|---|
| ⭐ Stars | 63,682 |
| 🛠 Language | Python |
| 📜 License | MIT |
| 🏷 Topic | `autonomous-vehicles`, `robotics` |

**What it is:** openpilot is an open-source operating system for robotics. It currently upgrades the driver assistance system in **300+ supported cars**, turning consumer vehicles into semi-autonomous drives with minimal hardware (comma four device + car harness).

**Latest Commits (Sept 2026):**

| Date | Commit | What's Happening |
|------|--------|-----------------|
| Sep 19, 2026 | `cabana: improve theme contrast` | UI polish — improving the Cabin app's visual contrast for better driver UX |
| Sep 19, 2026 | `DM: Super Leicht Model` | 🔥 **Big one** — developing a new lightweight perception model ("Super Leicht") for on-device inference |
| Sep 18, 2026 | `ui: allow delay of scroller start` | UI tweak — delayed scroller start to reduce distraction during driving |

**🎙️ Potential Episode Topics:**
- *"Super Leicht: How openpilot is shrinking perception models for edge devices"*
- *"From 300 cars to 3000: openpilot's hardware-agnostic strategy"*
- *"The ethics of driver-facing cameras: openpilot's privacy model"*
- *"ISO 26262 safety in an open-source driving OS"*

---

### 2. [ApolloAuto/apollo](https://github.com/ApolloAuto/apollo)
| | |
|---|---|
| ⭐ Stars | 26,829 |
| 🛠 Language | C++ |
| 📜 License | Apache-2.0 |
| 🏷 Topic | `autonomous-vehicles`, `robotics` |

**What it is:** Apollo is Baidu's full-stack open autonomous driving platform. It provides a complete stack from perception → prediction → planning → control, with versions ranging from simple waypoint following (Apollo 1.0) to geo-fenced urban autonomous driving (Apollo 11.0). It's one of the most mature and widely studied open-source AV platforms.

**Latest Commits (2026):**

| Date | Commit | What's Happening |
|------|--------|-----------------|
| Apr 16, 2026 | `docs: fix README - remove invalid build status badges` | Documentation cleanup |
| Feb 28, 2026 | `Merge PR #15762: recover_seyond_lidar_driver` | 🔧 Recovering beyond-lidar driver support — expanding sensor hardware compatibility |
| Feb 27, 2026 | `feat: add Apollo 11.0 bev+occ` | 🔥 **Big one** — Adding **Bird's-Eye-View (BEV) + Occupancy (Occ) networks** for Apollo 11.0, the next-gen perception pipeline |

**🎙️ Potential Episode Topics:**
- *"Apollo 11.0: BEV + Occupancy networks and the future of 3D perception"*
- *"From Apollo 1.0 to 11.0: the 10-year journey of Baidu's open AV platform"*
- *"Beyond-lidar: how Apollo is recovering sensor diversity"*
- *"Open-source vs. closed: can Apollo compete with Waymo/Cruise?"*

---

### 3. [carla-simulator/carla](https://github.com/carla-simulator/carla)
| | |
|---|---|
| ⭐ Stars | 14,409 |
| 🛠 Language | C++ |
| 📜 License | MIT |
| 🏷 Topic | `autonomous-vehicles`, `robotics` |

**What it is:** CARLA is an open-source urban driving simulator built on Unreal Engine, purpose-designed for developing, training, and validating autonomous driving systems. It provides open digital assets (roads, buildings, vehicles), flexible sensor suites, and realistic environmental conditions. The `ue5-dev` branch brings the power of **Unreal Engine 5.5** to autonomous driving research.

**Latest Commits (2026):**

| Date | Commit | What's Happening |
|------|--------|-----------------|
| Sep 2, 2026 | `Deploy UE5 nightly to Cloudflare R2` | ☁️ Hosting UE5 nightly builds on Cloudflare R2 — making the simulator more accessible globally |
| Jul 14, 2026 | `Fix lidar smoke helper signature` | 🔧 Bug fix for LiDAR sensor simulation — critical for accurate perception testing |
| Jul 14, 2026 | `fix(nav): guard against null traffic light in WalkerManager` | 🔧 Navigation robustness — preventing crashes when AI pedestrians encounter missing traffic signals |

**🎙️ Potential Episode Topics:**
- *"CARLA + UE5: How Unreal Engine 5.5 is revolutionizing autonomous driving simulation"*
- *"Sim-to-real gap: what CARLA gets right (and wrong) about the real world"*
- *"Open digital assets: the case for free urban environments in AV research"*

---

## 🎙️ Podcast Overview

The *Robotics OSS Radar* podcast explores the people, code, and politics behind the open-source robotics and autonomous systems movement. Each episode dives into a tracked project — its architecture, its community, and where it's headed next.

**Recurring Segments:**
- **Commit Spotlight** — One interesting commit from the week
- **Architectural Deep-Dive** — How the system is designed
- **Community Pulse** — Who's contributing and what they're building
- **Sim-to-Real / Policy Corner** — The gap between code on GitHub and robots on the road

---

## 📋 Tracking & Roadmap

See the open issue **[Projects to Revisit & Upcoming Releases](https://github.com/bro26man-hash/robotics-oss-radar/issues)** for a checklist of all tracked projects and their upcoming milestones.

---

## 🤝 Contributing

Got a project suggestion, a cool commit to spotlight, or an episode idea? Open an issue or submit a PR — this radar is community-driven.

## 📜 License

This project is open-source and available under the [MIT License](LICENSE).

# 🤖 Robotics & Autonomous Systems — Open-Source Radar

> A living radar for the most active open-source robotics and autonomous-vehicles repos, with commit summaries distilled from live `git log` inspection and podcast episode ideas for **Robotics OSS**.

_Last scan: 2026-09-17 · Sources: GitHub topic search on `robotics` & `autonomous-vehicles`, sorted by recent activity, followed by per-repo latest-commit inspection._

---

## 🔥 Top 3 Most Recently Active Repos

### 1. [commaai/openpilot](https://github.com/commaai/openpilot)
⭐ 63,671 stars · 🐍 Python

**About:** openpilot is an open-source **operating system for robotics**, primarily deployed as an aftermarket advanced driver-assistance system (ADAS) upgrade for 300+ consumer vehicles. Built by comma.ai, it turns a $200 device into a lane-centering, adaptive cruise control system powered by end-to-end neural networks.

**Latest Commits (Sep 17, 2026):**
- `bd176cb` — ui: remove question marks (#38938) *(9/17, Shane Smiskol)*
- `4d9d1bc` — ui: not paired bookmark alert (#38936) *(9/17, stef)*
- `cab5343` — AGNOS 19.8 (#38935) *(9/17, Daniel Koepping)*

**What's Cooking:** A fresh wave of UI polish landed — removing confusing question marks, fixing the "not paired" bookmark alert, and shipping **AGNOS 19.8**, the latest version of comma.ai's automotive-grade operating system. Three separate commits on the same day signals a rapid release cadence for their closed-platform device software. The "not paired bookmark" fix suggests active work on the reconnect/linking UX flow between the device and phone app. Expect the next big story to be the AGNOS 19.8 feature drop.

**🎙️ Episode Ideas:**
- *"AGNOS 19.8: What's Inside comma.ai's Latest OS Release"* — Deep-dive into what AGNOS ships each cycle and why it matters for edge autonomy.
- *"The $200 Self-Driving Upgrade, Still Going Strong"* — How openpilot maintains daily commits 5+ years after launch.
- *"UI Failures in Autonomy: When the Dashboard Confuses the Driver"* — Why removing question marks and fixing pairing alerts are safety-critical engineering work.
- *"Operating Systems for Cars: comma.ai's Vertical Stack"* — How a small team runs an entire vehicle OS from end-to-end.

---

### 2. [AtsushiSakai/PythonRobotics](https://github.com/AtsushiSakai/PythonRobotics)
⭐ 30,531 stars · 🐍 Python

**About:** Python sample codes and textbook for robotics algorithms. Covers everything from path planning (A*, D*, RRT) to SLAM, computer vision, and control — the go-to educational repository for learning robotics algorithms in Python.

**Latest Commits (Sep 2, 2026):**
- `08b453a` — build(deps): bump github/codeql-action from 4.37.4 to 4.37.9 (#1423) *(9/2, dependabot)*
- `8c3f761` — build(deps): bump ruff from 0.16.1 to 0.16.5 in /requirements (#1424) *(9/2, dependabot)*
- `069e0fb` — build(deps): bump scipy from 1.17.1 to 1.18.1 in /requirements (#1425) *(9/2, dependabot)*

**What's Cooking:** The latest commits are all dependency maintenance — CodeQL security scanning updates, ruff linter bumps, and scipy version upgrades. While not feature-facing, this is a healthy signal: the project is actively maintaining its CI/CD pipeline and keeping dependencies current, which is essential for a widely-used educational resource that thousands of students and researchers rely on. The scipy bump to 1.18.1 is notable — it supports newer Python versions and may bring performance improvements to the numerical algorithms that underpin the path-planning and control examples.

**🎙️ Episode Ideas:**
- *"The Invisible Labor of Open-Source Maintenance"* — Why dependency bumps matter more than they look (security, performance, compatibility).
- *"Teaching Robotics with Python"* — How PythonRobotics became the de facto textbook for robotics algorithms.
- *"Scipy 1.18 & Numerical Computing in Robotics"* — What the latest scipy release means for robotics algorithm performance.
- *"From Textbook to Training Wheels"* — The role of well-maintained READMEs and sample code in lowering the barrier to entry for robotics engineering.

---

### 3. [ApolloAuto/apollo](https://github.com/ApolloAuto/apollo)
⭐ 26,828 stars · ⬜ C++

**About:** Apollo is Baidu's **open autonomous driving platform** — one of the most comprehensive full-stack AV systems available in open source. It covers perception, prediction, planning, control, HD mapping, and simulation, and is used by dozens of automotive OEMs and research institutions worldwide.

**Latest Commits (Apr 16, 2026):**
- `d53aa3d` — docs: fix README - remove invalid build status badges *(4/16, xiaoxinyu)*
- `40c8a01` — Merge pull request #15762 from guyuechaocc/recover_seyond_lidar_driver *(2/28, yuxin)*
- `539f546` — feat: add Apollo 11.0 bev+occ *(2/27, yuxin)*

**What's Cooking:** The most significant recent work is **Apollo 11.0's BEV + Occupancy perception stack** — a major architectural shift toward Bird's Eye View transformers and 3D occupancy grids, replacing traditional LiDAR-centric pipelines. The "recover seyond lidar driver" PR restores support for Seyond LiDAR hardware, expanding the sensor ecosystem. The README badge fix is routine maintenance, but the fact that the two most substantive commits are from late February suggests Apollo 11.0's release cycle was still the dominant activity through spring. The BEV+occ work is the big one to watch — it signals Apollo is investing in the same perception paradigm that's becoming industry standard.

**🎙️ Episode Ideas:**
- *"Apollo 11.0 & the BEV Revolution"* — How Bird's Eye View transformers are replacing point cloud processing in AV perception.
- *"Occupancy Networks: The New Map"* — Why 3D occupancy grids may be the future of scene understanding for autonomous driving.
- *"Open-Source AV at Scale"* — How Baidu open-sourced a production AV stack and what that means for the industry.
- *"LiDAR Wars & Hardware Ecosystems"* — The sensor hardware landscape (Velodyne, Ouster, Seyond) and how open-source drivers shape adoption.
- *"From Apollo to Robotaxi"* — Tracing how open-source Apollo code ends up in commercial robotaxi fleets.

---

## 🎙️ About This Radar

Curated for the **Robotics OSS** podcast and refreshed periodically. Selection priorities:
- Genuine open-source robotics / autonomous-vehicle projects
- Active recent commit cadence (truly "being worked on")
- Strong narrative potential for podcast episodes

See the companion issue **[Projects to Revisit & Upcoming Releases](../../issues/11)** for the tracking checklist.

---

## 🔎 How to Use

1. Scan the **Top 3** above for current development highlights.
2. Pick an episode idea that resonates.
3. Check the companion issue for follow-up items (revisit dates, upcoming releases to watch).

---

_Licensed as part of the open-source robotics podcast ecosystem. Contributions and episode suggestions welcome._
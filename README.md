# 🤖 Robotics OSS Radar

> **Open-Source Robotics & Autonomous Systems Podcast**
> Tracking the projects, commits, and conversations that are shaping the future of autonomous systems.

---

## 🎙️ What Is This?

**Robotics OSS Radar** is a podcast (and accompanying tracker) that dives into the most actively developed open-source robotics and autonomous-vehicle projects on GitHub. Each episode profiles a project, interviews maintainers, and breaks down the latest commits so you don't have to read the diffs yourself.

---

## 📡 Projects Currently Tracked

### 1. 🚗 AlpaSim — `NVlabs/alpasim`

| | |
|---|---|
| **Stars** | ⭐ 1,239 |
| **Language** | Python |
| **Focus** | End-to-end autonomous vehicle simulation |
| **Last Activity** | August 2026 |

**Recent Development Highlights:**
- **Reproducible Rollouts** — Commit `9a3832b` (Aug 17, 2026) made rollout seeds selectable and reproducible via `RolloutSpec`, a huge win for researchers who need identical simulation runs for benchmarking.
- **High-Speed MPC** — Commit `1e801ca` (Aug 12, 2026) increased the linear MPC speed bound to **40 m/s** (~90 mph), pushing the platform toward real-world highway-speed scenario testing.
- **CI Pipeline Overhaul** — Commits `affc2ea` & `0d0f522` (Aug 11, 2026) eliminated LFS downloads during replay and fixed self-hosted build jobs, signaling serious investment in developer experience.
- **GitLab Sync** — Regular sync from internal GitLab (commit `6870924`, Aug 11, 2026) shows NVIDIA is using this as a production-grade internal tool, not just a research demo.

**🎙️ Potential Episode Topics:**
- *"Why Reproducible Rollouts Change Everything"* — The science of benchmarking AV policies
- *"From 5 m/s to 90 mph: Inside AlpaSim's Speed Revolution"*
- *"NVIDIA's Secret Sauce: How Internal CI Shapes Open-Source AV Dev"*

---

### 2. 🚢 BlueOS — `bluerobotics/BlueOS`

| | |
|---|---|
| **Stars** | ⭐ 456 |
| **Language** | Vue (frontend) + backend services |
| **Focus** | Open-source operational platform for ROVs, USVs & robotic systems |
| **Last Activity** | September 2026 |

**Recent Development Highlights:**
- **Version Chooser Overhaul** — Five commits on a single day (Sep 15, 2026, all by Patrick José Pereira) rebuilt the entire version-selection UI: new `VersionChooser` component, `VersionCard` with commit button, `NestedVersion` & `parent_sha` types, and dedicated service-layer tests. This is a major UX upgrade for fleet operators who need to manage software versions across fleets of underwater robots.
- **Commit-Level Traceability** — The new "commit dialog" and "commit button" features mean every deployed version is traceable to its exact source commit — critical for safety-certified ROV operations.
- **Test-First Approach** — Commit `91e81ab` added tests for commit and parent detection, showing the team is prioritizing reliability as the UI grows more complex.

**🎙️ Potential Episode Topics:**
- *"Underwater Robots Need Software Updates Too — Inside BlueOS's Version Revolution"*
- *"From Play to Production: How BlueOS Is Making ROVOps Developer-Friendly"*
- *"Commit Traceability for Safety-Critical Robots — Why It Matters"*

---

### 3. 🧠 Autonomous-OS — `autonomous-ai/autonomous-os`

| | |
|---|---|
| **Stars** | ⭐ 348 |
| **Language** | Python |
| **Focus** | Open-source operating system that brings robots to life |
| **Last Activity** | September 2026 (very active!) |

**Recent Development Highlights:**
- **Rapid Release Cadence** — Commit `2668ac9` (Sep 18, 2026) bumped `os-server` to **v0.1.142** and `web` to **v0.1.64** — an incredibly fast release cycle, suggesting a mature CI/CD pipeline and agile development.
- **Schedule Connector Guard** — PR #455 (merged Sep 18, 2026) introduced a `schedule-connector-guard` feature, likely a safety mechanism to prevent scheduling conflicts or runaway task dispatching in multi-robot environments.
- **Voice-Enabled Real-Time Controls** — Commit `71dbd54` (Sep 18, 2026) added a "realtime wait filler before the post-capture session handshake" for voice commands, indicating they're building voice-controlled robot interaction with low-latency guarantees.
- **Daily Deployments** — Multiple commits on Sep 18 alone (`2e9deab` — "deploy") show this team ships daily, a hallmark of a serious production-grade project.

**🎙️ Potential Episode Topics:**
- *"Daily Deploys & 142 Versions: What We Can Learn from Autonomous-OS's Velocity"*
- *"Talking to Your Robot: The Science of Voice-Controlled Autonomous Systems"*
- *"Schedule Guards & Safety: How to Prevent Multi-Robot Chaos"*

---

## 🗓️ Episode Planning Calendar

| Episode | Project | Focus Area | Status |
|---------|---------|-----------|--------|
| 01 | AlpaSim | Reproducible Rollouts & AV Benchmarking | 📋 Planned |
| 02 | BlueOS | Version Traceability for Underwater Robots | 📋 Planned |
| 03 | Autonomous-OS | Voice Controls & Daily Deploy Cadence | 📋 Planned |

---

## 📡 How to Contribute

1. Fork this repo
2. Add your favorite OSS robotics project to `projects/`
3. Open a PR with commit highlights and episode ideas
4. Subscribe to the podcast!

## 🔗 Related Resources

- [GitHub Topics: Robotics](https://github.com/topics/robotics)
- [GitHub Topics: Autonomous Vehicles](https://github.com/topics/autonomous-vehicles)
- [ROS 2 Documentation](https://docs.ros.org/)
- [Autoware Foundation](https://autoware.org/)

---

*Built for the open-source robotics community. Built with ❤️ and a lot of `git log`.*
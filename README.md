# 🤖 Robotics OSS Radar

> Podcast companion repo tracking the most actively-developed open-source robotics & autonomous systems projects on GitHub.

## Why This Repo?

Every episode of the **Robotics OSS Radar** podcast dives deep into a real open-source robotics project — what's shipping, what's breaking, and what it means for the future of autonomous systems. This repo is the living behind-the-scenes tracker: project summaries, recent commit highlights, and episode-ready topic ideas.

---

## 📡 Projects on the Radar

### 1. [commaai/openpilot](https://github.com/commaai/openpilot)
**Stars:** 63,676 ⭐ | **Language:** Python | **Focus:** Open-source driver assistance / autonomous driving OS

> *"openpilot is an operating system for robotics. Currently, it upgrades the driver assistance system on 300+ supported cars."*

**Recent Development Highlights (as of Sep 18, 2026):**

| Commit | What's Happening |
|---|---|
| `df7e0e5` — Use upstream tinygrad disk tensors for model loading (#38956) | Swapping in tinygrad's disk tensors for faster, more efficient model loading — a signal they're optimizing the inference pipeline at the TensorFlow level. |
| `6c69ebe` — cabana: improve heatmap readability (#38955) | UX improvements in the **Cabana** debugging UI, making attention/heatmap visualizations clearer for developers tuning perception models. |
| `c504b92` — cabana: clarify signal button states (#38953) | Further Cabana polish — clarifying interactive signal states so engineers can more easily diagnose input/output issues. |

**🎙️ Potential Episode Topics:**
- "tinygrad vs. TensorFlow: What openpilot's model-loading pivot means for the autonomy stack"
- "Building the Debugging UI: Inside openpilot's Cabana tool"
- "300+ cars, one codebase — how openpilot maintains scalability across vehicle platforms"
- "OpenPilot vs. Tesla FSD: The open-source advantage in data-driven driving"

---

### 2. [autowarefoundation/autoware](https://github.com/autowarefoundation/autoware)
**Stars:** 12,067 ⭐ | **Language:** Dockerfile / C++ / Python | **Focus:** The world's leading open-source autonomous driving software

> *"Autoware — the world's leading open-source software project for autonomous driving"*

**Recent Development Highlights (as of Sep 18, 2026):**

| Commit | What's Happening |
|---|---|
| `487474c` — Update autoware_utils to v1.11.0 (#7319) | Minor release bump on `autoware_utils` — the foundational utility library that everything else depends on. |
| `a45f9ba` — Update managed_transform_buffer to v0.3.0 (#7316) | Another dependency bump — the `managed_transform_buffer` package (critical for coordinate-frame management in autonomous stacks) gets a patch release. |
| `79446c0` — Add CARLA 0.10 Town10HD_Opt map to demo_artifacts (#7308) | High-Definition map support for CARLA 0.10 simulations — big for anyone testing Autoware in synthetic urban environments. |

**🎙️ Potential Episode Topics:**
- "Inside Autoware's release cadence: how a 12K-star project manages dependencies"
- "CARLA + HD Maps: Simulating the real world for autonomous driving testing"
- "The Autoware Foundation: how open-source governance scales a global autonomy project"
- "managed_transform_buffer — the unsung hero of coordinate-frame safety"

---

### 3. [RobotWebTools/rclnodejs](https://github.com/RobotWebTools/rclnodejs)
**Stars:** 448 ⭐ | **Language:** JavaScript | **Focus:** ROS 2 client library for Node.js with browser integration

> *"ROS 2 client library for Node.js, with browser integration"*

**Recent Development Highlights (as of Sep 18, 2026):**

| Commit | What's Happening |
|---|---|
| `a66e983` — Fix Windows test execution and WebSocket cleanup (#1610) | Cross-platform CI fix — Windows test execution and WebSocket resource cleanup. Critical for anyone running rclnodejs on Windows dev machines. |
| `58411a9` — Preserve native type-description responses and prevent test leaks (#1608) | Hardening around type-description handling and preventing test leaks — signs of maturing reliability for production ROS 2 + Node.js deployments. |
| `c8cf887` — Report CI failures and resolve Node.js 26 test regressions (#1601) | Proactive CI failure reporting and fixing regressions on the bleeding-edge Node.js 26 — keeping the library compatible with the latest runtime. |

**🎙️ Potential Episode Topics:**
- "ROS 2 in the Browser: What rclnodejs makes possible for web developers"
- "Cross-platform robotics: Why Windows support matters for the ROS ecosystem"
- "From Node.js to ROS 2: Bridging the web and robotics worlds"
- "Node.js 26 compatibility — how open-source libraries keep pace with runtime changes"

---

## 📋 How to Use This Repo

- **New episodes?** Update the relevant project section with latest commits & topic ideas.
- **Spotted a trending PR?** Open an issue to flag it for a future episode.
- **Listener contributions?** Accept pull requests with additional project suggestions or topic notes.

---

## 🔗 Links

- **Podcast:** _[insert link]_
- **Twitter/X:** _[insert link]_
- **Discord/Community:** _[insert link]_

---

*Built for the open-source robotics community. Star the repos, fork the ideas, ship the future.* 🚀

# 🤖 Robotics OSS Radar

> Open-source robotics & autonomous systems radar — tracking the most active projects, recent highlights, and podcast episode ideas.

---

## 📡 Monitored Projects

We track the top recently active open-source repos tagged with **autonomous-vehicles** or **robotics**, summarizing weekly development highlights and brainstorming podcast episode angles.

---

### 1. 🦾 [autonomous-ai/autonomous-os](https://github.com/autonomous-ai/autonomous-os)

> The open-source operating system for robots — install it and your robot comes alive.

| ⭐ Stars | 🍴 Forks | Language | Last Updated |
|----------|----------|----------|--------------|
| 348      | —        | Python   | Sep 18, 2026 |

**Latest Commits (Sep 18, 2026):**

| Commit | Message | Author |
|--------|---------|--------|
| `6c828c6` | chore: bump lamp device profile version | leo |
| `ce220c5` | lamp: reverse MPR121 swipe axis to match mirrored pad wiring | leo |
| `39d7914` | lamp: max_volume 15 for the C-Media speaker card | leo |
| `63c921e` | lamp: C-Media card id device_cmedia backs speaker and sensing mic; ZVCAI gain 64 | leo |
| `8b5c343` | lamp: swap primary/factory-reset GPIO lines to match wiring (99/100) | leo |

**Development Highlights:**
- **Hardware bring-up momentum** — five commits in a single day all focused on "lamp," a physical robot device. This is raw, hands-on embedded work: GPIO wiring, audio driver configuration, and capacitive touch sensor calibration.
- **Audio system integration** — C-Media speaker card and mic characterization with ZVCAI gain staging. This shows the project is maturing beyond "just ROS" into real hardware audio pipelines — critical for voice-interactive robots.
- **Capacitive touch debugging** — reversing the MPR121 swipe axis to match mirrored pad wiring. This is the kind of bug that only surfaces when software meets the physical world. Great podcast material on the frustration and triumph of hardware bring-up.
- **Device profile versioning** — systematic bumping of device profiles signals a growing ecosystem of supported hardware platforms.

**🎙️ Potential Episode Topics:**
- "From Software to Silicon: What Happens When Your Robot Won't Boot"
- "The MPR121 Nightmare: Capacitive Touch Debugging at 2 AM"
- "Audio Pipelines for Robots: Why Your C-Media Card Matters"
- "autonomous-os: Installing an OS That Makes Your Robot Come Alive"
- "GPIO Wiring 101: The Undocumented Art of connecting Robots to Reality"

---

### 2. 🚗 [autowarefoundation/autoware](https://github.com/autowarefoundation/autoware)

> The world's leading open-source software project for autonomous driving.

| ⭐ Stars | 🍴 Forks | Language | Last Updated |
|----------|----------|----------|--------------|
| 12,068   | —        | C++ / Dockerfile | Sep 18, 2026 |

**Latest Commits:**

| Commit | Message | Author | Date |
|--------|---------|---------|------|
| `487474c` | feat(repositories/autoware.repos): minor update autoware_utils to 1.11.0 (#7319) | awf-bot | Sep 18, 2026 |
| `a45f9ba` | feat(repositories/autoware.repos): minor update managed_transform_buffer to 0.3.0 (#7316) | awf-bot | Sep 16, 2026 |
| `79446c0` | feat(ansible): add the CARLA 0.10 Town10HD_Opt map to demo_artifacts (#7308) | Masaya Kataoka | Sep 9, 2026 |

**Development Highlights:**
- **Dependency hygiene** — systematic minor-version bumps across the ecosystem (autoware_utils → 1.11.0, managed_transform_buffer → 0.3.0), showing mature CI/CD practices and a well-orchestrated release pipeline.
- **Simulation expansion** — new CARLA 0.10 Town10HD_Opt high-definition map added for demo artifacts. This is a big deal — HD maps are essential for L4 autonomy testing and urban scenario replay.
- **Infrastructure-as-code** — using Ansible for demo artifact management, signaling professionalism in how they manage complex multi-robot demo environments.

**🎙️ Potential Episode Topics:**
- "Autoware 1.11: What's New in the Latest Release and Why It Matters"
- "Simulation as a Service: How CARLA HD Maps Are Shaping Autonomous Testing"
- "The ROS 2 Ecosystem: Inside Autoware's Dependency Management Strategy"
- "From Research to Road: How Autoware Bridges the Gap Between Simulation and Real-World Deployment"

---

### 3. 🛡️ [Hebbian-Robotics/hflow](https://github.com/Hebbian-Robotics/hflow)

> SDK for robotics teams to verify the quality of data used for AI model training.

| ⭐ Stars | 🍴 Forks | Language | Last Updated |
|----------|----------|----------|--------------|
| 272      | —        | Python   | Sep 18, 2026 |

**Latest Commits:**

| Commit | Message | Author | Date |
|--------|---------|---------|------|
| `4d17559` | fix(lerobot): refuse task_index referencing unpublished tasks before … (#559) | Shobhit agnihotri | Sep 18, 2026 |
| `e7a615b` | fix(import): guard meta/episodes tree loop against missing 'path' (#555) | Sravan Avvaru | Sep 18, 2026 |
| `1ae107d` | chore(deps): bump astral-sh/setup-uv in github-actions (#557) | dependabot | Sep 18, 2026 |
| `9c9fd21` | feat(examples): reproducible real-camera LeRobot workflow (#552) | Ayam | Sep 16, 2026 |
| `f2e3cf0` | fix(checks): fail closed on unmeasurable joint-motion steps (#546) (#549) | Sagar Kharal | Sep 16, 2026 |

**Development Highlights:**
- **Robustness fixes** — guarding against missing path keys in meta/episodes trees and refusing unpublished task references. These are real-world data pipeline edge cases that break when datasets are imperfect. Good sign they're listening to user pain points.
- **LeRobot integration** — new reproducible real-camera example workflow, bridging the gap between simulation-trained models and real-world deployment. This is the sim-to-real story everyone wants to hear.
- **Safety-first validation** — "fail closed on unmeasurable joint-motion steps" means the SDK refuses to pass data it can't verify, which is a philosophy worth discussing on a podcast about responsible robotics.
- **DevEx improvements** — migrating to `setup-uv` for faster, more reliable Python environment setup in CI. Small but meaningful: faster CI = faster feedback = faster shipping.

**🎙️ Potential Episode Topics:**
- "Data Quality Is the Real Robot Problem: Why hflow Exists"
- "Sim-to-Real: How LeRobot Workflows Are Closing the Gap"
- "From 0 to 1: Building a Robotics Data Verification SDK from Scratch"
- "The 90% Problem: Why Data Quality Eats 90% of Robotics Dev Time"
- "Fail Closed: The Philosophy of Refusing to Ship Unverifiable Robots"

---

## 🔍 Why These Three?

| Repo | Domain | Stars | Activity | Podcast Potential |
|------|--------|-------|----------|-------------------|
| autonomous-os | Robot OS / Hardware Bring-up | 348 | 🔥 Daily | High — the physical robot story |
| autoware | Autonomous Driving (Stack) | 12K | 🔥 Daily | High — L4 roadmap |
| hflow | Robotics Data Quality | 272 | 🔥 Daily | Medium — niche but critical |

These three were selected from GitHub's **topic:autonomous-vehicles** and **topic:robotics** searches, filtered by recent commit activity (all three had commits within the last 48 hours).

---

## 📋 Tracking Checklist

See the open issue **[Projects to Revisit & Upcoming Releases](https://github.com/bro26man-hash/robotics-oss-radar/issues)** for a full checklist of projects to track going forward.

---

## 🔧 How to Contribute

1. Fork this repo
2. Add your favorite robotics OSS project to `projects/`
3. Submit a PR with weekly commit summaries and episode ideas

---

## 📅 Update Cadence

- **Weekly** — Latest commits reviewed & summarized
- **Monthly** — Release notes & milestone deep-dives
- **Per Episode** — In-depth project spotlights

---

*Built for the open-source robotics community. ★ Star this repo if you find it useful!*
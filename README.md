# 🤖 Robotics OSS Radar

> Open-source robotics & autonomous systems radar — tracking the most active projects, recent highlights, and podcast episode ideas.

---

## 📡 Monitored Projects

We track the top recently active open-source repos tagged with **autonomous-vehicles** or **robotics**, summarizing weekly development highlights and brainstorming podcast episode angles.

---

### 1. 🚗 [commaai/openpilot](https://github.com/commaai/openpilot)

> An operating system for robotics — currently upgrading driver assistance on **300+ supported cars**.

| ⭐ Stars | 🍴 Forks | Language | Last Updated |
|----------|----------|----------|--------------|
| 63,676   | —        | Python   | Sep 18, 2026 |

**Latest Commits (Sep 18, 2026):**

| Commit | Message | Author |
|--------|---------|--------|
| `df7e0e5` | Use upstream tinygrad disk tensors for model loading (#38956) | Harald Schäfer |
| `6c69ebe` | cabana: improve heatmap readability (#38955) | Trey Moen |
| `c504b92` | cabana: clarify signal button states (#38953) | Trey Moen |

**Development Highlights:**
- **Model loading optimization** — migrating to upstream tinygrad disk tensors for faster, more efficient model inference. This signals a major push toward lighter-edge deployment and reduced memory footprint on commodity hardware.
- **Cabana UI overhaul** — heatmap readability improvements and clearer signal button states, indicating investment in driver-facing UX clarity. Better interpretability = more trust in autonomous systems.
- **Rapid iteration pace** — 3 commits in a single day shows a highly active, responsive development team.

**🎙️ Potential Episode Topics:**
- "TinyGrad & Edge Inference: How openpilot is shrinking its model footprint"
- "UX Matters: Why driver-facing UIs make or break ADAS adoption"
- "300+ Cars, One OS: The scaling challenges of open-source ADAS"
- "From Pilot to Production: How commaai ships to 300+ car models"

---

### 2. 🛰️ [autowarefoundation/autoware](https://github.com/autowarefoundation/autoware)

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
- "Autoware 1.11: What's new in the latest release and why it matters"
- "Simulation as a Service: How CARLA HD maps are shaping autonomous testing"
- "The ROS 2 Ecosystem: Inside Autoware's dependency management strategy"
- "From Research to Road: How Autoware bridges the gap between simulation and real-world deployment"

---

### 3. 🦾 [Hebbian-Robotics/hflow](https://github.com/Hebbian-Robotics/hflow)

> SDK for robotics teams to verify the quality of data used for AI model training.

| ⭐ Stars | 🍴 Forks | Language | Last Updated |
|----------|----------|----------|--------------|
| 272      | —        | Python   | Sep 18, 2026 |

**Latest Commits:**

| Commit | Message | Author | Date |
|--------|---------|---------|------|
| `e7a615b` | fix(import): guard meta/episodes tree loop against missing 'path' (#555) | Sravan Avvaru | Sep 18, 2026 |
| `1ae107d` | chore(deps): bump astral-sh/setup-uv in github-actions (#557) | dependabot | Sep 18, 2026 |
| `9c9fd21` | feat(examples): reproducible real-camera LeRobot workflow (#552) | Ayam | Sep 16, 2026 |

**Development Highlights:**
- **Robustness fixes** — guarding against missing path keys in meta/episodes trees. This is a real-world data pipeline edge case that breaks when datasets are imperfect. Good sign they're listening to user pain points.
- **LeRobot integration** — new reproducible real-camera example workflow, bridging the gap between simulation-trained models and real-world deployment. This is the sim-to-real story everyone wants to hear.
- **DevEx improvements** — migrating to `setup-uv` for faster, more reliable Python environment setup in CI. Small but meaningful: faster CI = faster feedback = faster shipping.

**🎙️ Potential Episode Topics:**
- "Data Quality is the Real Robot Problem: Why hflow exists"
- "Sim-to-Real: How LeRobot workflows are closing the gap"
- "From 0 to 1: Building a robotics data verification SDK from scratch"
- "The 90% Problem: Why data quality eats 90% of robotics dev time"

---

## 🔍 Why These Three?

| Repo | Domain | Stars | Activity | Podcast Potential |
|------|--------|-------|----------|-------------------|
| openpilot | Autonomous Driving (Production) | 63K | 🔥 Daily | High — mass adoption story |
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
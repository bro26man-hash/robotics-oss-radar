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
| `1090e28` — ui: add pairing provider to prime state (#38950) | New pairing provider integrated into the Prime state UI — streamlining device pairing workflows for mobile integration. |
| `b55e37b` — cabana: right-align numeric message values (#38959) | UI refinement in Cabana — numeric values now right-aligned for easier scanning and comparison across telemetry streams. |

**🎙️ Potential Episode Topics:**
- "tinygrad vs. TensorFlow: What openpilot's model-loading pivot means for the autonomy stack"
- "Building the Debugging UI: Inside openpilot's Cabana tool"
- "300+ cars, one codebase — how openpilot maintains scalability across vehicle platforms"
- "OpenPilot vs. Tesla FSD: The open-source advantage in data-driven driving"
- "From Prime State to Pairing: How openpilot is evolving its mobile UX"

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
| `87f7b60` — fix(docker): build simple planning simulator with core (#7311) | Docker build fix for the simple planning simulator — ensuring the core simulator can be built and run in containerized environments. |
| `3354a27` — fix(acados): pin CasADi to 3.7.2 for Humble ARM64 (#7307) | Critical fix pinning CasADi to 3.7.2 for Ubuntu Humble on ARM64 — addressing compatibility issues on the rising ARM64 platform. |

**🎙️ Potential Episode Topics:**
- "Inside Autoware's release cadence: how a 12K-star project manages dependencies"
- "CARLA + HD Maps: Simulating the real world for autonomous driving testing"
- "The Autoware Foundation: how open-source governance scales a global autonomy project"
- "managed_transform_buffer — the unsung hero of coordinate-frame safety"
- "ARM64 & CasADi: Why platform compatibility matters in autonomous stacks"

---

### 3. [Hebbian-Robotics/hflow](https://github.com/Hebbian-Robotics/hflow)
**Stars:** 272 ⭐ | **Language:** Python | **Focus:** SDK for robotics teams to verify the quality of their data used for AI model training

> *"SDK for robotics teams to verify the quality of their data used for AI model training."*

**Recent Development Highlights (as of Sep 18, 2026):**

| Commit | What's Happening |
|---|---|
| `e7a615b` — fix(import): guard the meta/episodes tree loop against a missing 'path' (#555) | Robustness fix — preventing crashes when a `path` key is missing in the metadata tree. Signals growing real-world usage where incomplete metadata is common. |
| `1ae107d` — chore(deps): bump astral-sh/setup-uv in the github-actions group (#557) | Keeping CI tooling current with the latest `setup-uv` action — faster, cleaner Python environment setup for tests and builds. |
| `9c9fd21` — feat(examples): reproducible real-camera LeRobot workflow (fixes #191) (#552) | Major new example showing a fully reproducible pipeline using real camera data with LeRobot — bridges the gap between simulation and real-world robotics data collection. |
| `f2e3cf0` — fix(checks): fail closed on unmeasurable joint-motion steps (#546) (#549) | Safety-first design decision — the SDK now fails closed when joint-motion steps can't be measured, ensuring unreliable data never passes validation silently. |
| `590b05f` — test: fold copy-pasted guard tests into their parametrized siblings | Test cleanup — reducing duplication and improving test coverage for guard pathways. |

**🎙️ Potential Episode Topics:**
- "Data Quality is the Next Bottleneck in Robotics AI — why hflow matters"
- "From Simulation to Reality: hflow's LeRobot camera workflow explained"
- "Building a Robotics Data SDK: what it takes to validate training data at scale"
- "The gap between imitation learning and real-world data — hflow's approach"
- "Fail-Closed Safety: How hflow ensures bad data never trains a bad model"

---

## 📋 How to Use This Repo

- **New episodes?** Update the relevant project section with latest commits & topic ideas.
- **Spotted a trending PR?** Open an issue to flag it for a future episode.
- **Listener contributions?** Accept pull requests with additional project suggestions or topic notes.

## 🔗 Links

- **Podcast:** _[insert link]_
- **Twitter/X:** _[insert link]_
- **Discord/Community:** _[insert link]_

---

*Built for the open-source robotics community. Star the repos, fork the ideas, ship the future.* 🚀
# 🤖 Robotics OSS Radar

**Open-source robotics & autonomous systems tracker** — curated for the podcast. We monitor the most active repos, recent commits, and brainstorm episode topics across the ROS/autonomous-vehicles ecosystem.

---

## 🔥 Top 3 Most Recently Active Projects

### 1. ⚙️ HORUS — `[softmata/horus]` (432 ⭐ · Rust)
> *Fastest Robotics Runtime System* — "If phones have Android, robots deserve HORUS."

**Recent Development Highlights (Sept 2026):**
- **`#155`** — Scoped SHM (shared memory) corruption tests to their own namespace, improving test isolation and reliability.
- **`#143`** — Fixed a critical pool-file truncation bug that previously caused a `SIGBUS` crash on robots — now properly errors out instead of taking down the whole system.
- **`#126`** — Enabled 404 tests that the repo already contained but had never been executed, boosting test coverage.

**Potential Episode Topics:**
- 🎙️ *"Why Rust is replacing C++ in robot runtimes"* — HORUS's choice of Rust for safety-critical robot middleware.
- 🎙️ *"Shared memory pitfalls in robotics"* — The SIGBUS → graceful error journey and what it means for real-world deployments.
- 🎙️ *"Testing robotics systems at scale"* — How HORUS approaches isolating faults in shared-memory IPC.

---

### 2. 🌾 Fields2Cover — `[Fields2Cover/Fields2Cover]` (881 ⭐ · C++)
> *Robust and efficient coverage paths for autonomous agricultural vehicles* — A modular, extensible Coverage Path Planning (CPP) library.

**Recent Development Highlights (Sept 2026):**
- **Release `2.1.0`** — A new stable release dropped on Sept 3, bringing fresh features and fixes to the ecosystem.
- **`#248`** — Added corridor attribution: reports which cell each corridor belongs to, and lets callers request a *fair split* across cells — a huge UX win for field-map visualization.
- **`#232`** — Fixed parsing of single-digit UTM zones, a subtle bug that could cause path-planning failures in certain geographic regions.

**Potential Episode Topics:**
- 🎙️ *"Coverage path planning in 2026"* — FromCNN-based promoters to fair-split algorithms: how autonomous tractors are getting smarter.
- 🎙️ *"Release engineering for robotics libraries"* — What goes into a major release like Fields2Cover v2.1.0.
- 🎙️ *"Geospatial pitfalls in autonomous farming"* — Why a single-digit UTM zone bug could derail an entire harvest season.

---

### 3. 🧠 hflow — `[Hebbian-Robotics/hflow]` (230 ⭐ · Python)
> *SDK for robotics teams to verify the quality of their data used for AI model training.*

**Recent Development Highlights (Sept 2026):**
- **`#382`** — Added **hosted Build AI check execution** — a new feature enabling CI-style validation of AI training pipelines directly in the cloud.
- **`ci: reduce flaky and duplicate checks`** — Improved CI reliability by cleaning up redundant checks, making the data-quality feedback loop faster.
- **`update docs`** — Fresh documentation to help new adopters onboard quickly.

**Potential Episode Topics:**
- 🎙️ *"Data quality = AI quality"* — Why Hebbian Robotics built a dedicated SDK for dataset validation before model training even starts.
- 🎙️ *"CI/CD for AI training data"* — The `Build AI check` execution model and how it mirrors software CI principles for robotics datasets.
- 🎙️ *"Flaky tests in robotics ML pipelines"* — Lessons learned from systematically eliminating CI noise in data-quality verification.

---

## 📡 Radar Key

| Tag | Meaning |
|-----|---------|
| 🔴 | Actively developed · recent commits this week |
| 🟡 | Steady progress · commits within the month |
| 🟢 | Stable · watched for releases |

**Current Radar Status:**
- **HORUS** 🔴 — 3 commits in the last 3 days; active investigation of SHM hardening
- **Fields2Cover** 🔴 — Just shipped v2.1.0 with new corridor-split features
- **hflow** 🔴 — New cloud AI-check feature live; CI quality improvements landing

---

*Curated by the robotics-oss-radar podcast crew. For episode ideas or project suggestions, open an issue!*

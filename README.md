# 🤖 Robotics & Autonomous Systems — Open-Source Radar

> A living radar for the most active open-source robotics and autonomous-vehicles repos, with commit summaries distilled from live `git log` inspection and podcast episode ideas for **Robotics OSS**.

_Last scan: 2026-09-10 · Sources: GitHub topic search on `robotics` & `autonomous-vehicles`, sorted by recent activity, followed by per-repo latest-commit inspection._

---

## 🔥 Top 3 Most Recently Active Repos

### 1. [NVIDIA / elements](https://github.com/NVIDIA/elements)
⭐ 85 stars · 🦶 TypeScript

**About:** NVIDIA Design System and UI Agent Harness for AI/ML Factories, Robotics, and Autonomous Vehicles. A web-based design-system plus agent-harness patterns layer that underpins robotics and autonomy software factories.

**Latest Commits (Sep 2026):**
- `9577c5c` — chore(ci): update svgo *(9/9)*
- `5b9b0ee` — chore(starters): update dependencies *(9/8)*
- `2c79c02` — chore(forms): drop unnecessary boolean conversions in checkbox mixin *(9/10, 🤖 Cursor Agent)*
- `d6dc590` — chore(core): cover connected move in format-truncate *(9/9, 🤖 Cursor Agent)*
- `6126e1c` — fix(docs): update responsive pattern icon *(9/8)*

**What's Cooking:** Steady maintenance on CI tooling, component mixins/accessibility, and docs — and notably several commits were authored by a **Cursor Agent**, hinting that NVIDIA's own software-factory tooling is agentic. A fascinating signal: the design system feeding robotics/AV factory UIs is partly authored by AI agents.

**🎙️ Episode Ideas:**
- *"When a Design System Runs on Agentic Code"* — NVIDIA elements and AI-assisted UI infrastructure for autonomy.
- *"Software Factories for Autonomy"* — how design systems & UI agent harnesses enable AV/robotics software factories.
- *"Open-Sourcing the UI Layer of a Robot Factory"* — trade-offs of an open design system in safety-critical robotics.

---

### 2. [haidmoham / spider](https://github.com/haidmoham/spider)
⭐ Community · 🐍 Python

**About:** **C-1N** — a MuJoCo hexapod simulation for reproducible standing control, locomotion experiments, and evaluation. A research/teaching bench for curricular reinforcement and control learning on a six-legged robot.

**Latest Commits (Sep 2026):**
- `722428d` — Merge pull request #23 from haidmoham/codex/assignment-scaffolding *(9/10)*
- `0c9f7ea` — docs(practice): use assignment-sized policy exercises *(9/10)*
- `7abb115` — Merge pull request #22 from haidmoham/codex/first-c1n-policy-lesson *(9/10)*
- `c6243a2` — docs(learning): scaffold one policy line at a time *(9/10)*
- `cb21c4c` — docs(learning): prepare the first C1N policy lesson *(9/10)*

**What's Cooking:** Momentum has shifted strongly toward **documentation and pedagogy** — a flurry of PRs scaffolding the "C1N" policy lessons and assignment-sized exercises. The project is evolving from pure simulation into a reproducible locomotion-control curriculum — a great angle on teaching RL/control.

**🎙️ Episode Ideas:**
- *"Teaching a Hexapod to Stand: Curricular Reinforcement Learning"* — the C1N approach and policy scaffolding.
- *"MuJoCo as a Classroom"* — building reproducible robotics micro-experiments.
- *"From Simulation to a Locomotion Curriculum"* — structuring RL training via lesson-style scaffolding.

---

### 3. [willv678 / autolab-harness](https://github.com/willv678/autolab-harness)
⭐ New / early · 🐍 Python

**About:** An **agentic test harness and orchestration framework** for LLM-driven autonomous vehicle safety verification and automated red-teaming in closed-loop simulators.

**Latest Commits (Sep 2026):**
- `71513c0` — [draft] training script *(9/10)*
- `bdeb1b2` — result processing shell script *(9/10)*
- `068b046` — feat: complete initial harness, SFT formatter, and failure boundary plotting *(9/10)*
- `9f4f7ab` — feat: Initial commit of AutoLab agent harness and orchestrator *(9/9)*

**What's Cooking:** Very early and fast-moving. The initial harness, orchestrator, SFT (supervised fine-tuning) formatter, and failure-boundary plotting landed in a single day, and a **training script** + result-processing shell script are now in draft. The trajectory: turn red-team AV-safety failures into training data via closed-loop simulation.

**🎙️ Episode Ideas:**
- *"Red-Teaming Autonomous Vehicles with LLMs"* — agentic harnesses for closed-loop AV safety testing.
- *"From Safety Failures to Training Data"* — SFT formatters, failure-boundary plotting, and result pipelines.
- *"AutoLab: Orchestrating a Robot Red Team"* — building test harnesses that run autonomy in a loop against an LLM "adversary."

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

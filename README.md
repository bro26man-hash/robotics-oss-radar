# 🤖 Robotics & Autonomous Systems — Open-Source Radar

> A living radar for the most active open-source robotics and autonomous-vehicles repos, with commit summaries and podcast episode ideas.

_Sourced on 2026-09-10. Activity verified via live latest-commit checks._

---

## 🔥 Top 3 Most Recently Active Repos

### 1. [commaai / openpilot](https://github.com/commaai/openpilot)
⭐ 63,626 stars · 🐍 Python · License: MIT · Forks: 11,360

**About:** openpilot is "an operating system for robotics." It upgrades the driver-assistance system on 300+ supported cars and runs an entire stacked driving model on commodity edge hardware (the comma four). It's the largest and most-proven open-source ADAS stack in the wild.

**Latest Commits (Sep 10, 2026):**
- `511c1f1` — chestnut updater: close files explicitly
- `443967d` — enable caching in chestnut CI
- `633117b` — test_onroad in chestnut CI
- `f174e39` — add powertest for mici
- `68d829c` — selfdrived: no localizer alerts from capnp defaults

**What's Cooking:** Platoon of quick, focused commits all titled around the new **Chestnut** hardware branch — file-handle hygiene, CI caching, on-road testing, and a powertest. The cadence (5 commits in one day by Daniel Koepping and Zeph) is the rhythm of a production embedded stack preparing a release branch. Meanwhile the internal model/inference side ("selfdrived") is being quietly hardened. This is a mature project where most work is incremental CI/hardware readiness, not flashy algorithmic PRs.

**🎙️ Episode Ideas:**
- *"openpilot Is an Operating System for Robotics"* — What it actually means to run a full driving stack on a $500 edge device.
- *"Deploying Autonomy at 60 mph: How openpilot Tests for Safety"* — ISO26262, SIL/HIL tests, and the 10-closet replay rig.
- *"From Dashcam to Driver: The openpilot Release Pipeline"* — Walking the release/staging/nightly/chestnut branches.
- *"The Business of Open-Source Autonomy"* — comma.ai's model (hardware shop, bounties, hired core devs).

---

### 2. [NVIDIA / elements](https://github.com/NVIDIA/elements)
⭐ 85 stars · TypeScript · License: Apache-2.0 · Forks: 16

**About:** NVIDIA Design System and UI Agent Harness for AI/ML Factories, Robotics, and Autonomous Vehicles. Framework-agnostic Web Components (React, Angular, Vue, Svelte, Lit, plain HTML) plus a CLI/MCP layer that exposes components, tokens, and validation to terminals and AI assistants.

**Latest Commits (Sep 8–10, 2026):**
- `9577c5c` — chore(ci): update svgo *(Cory Rylan)*
- `5b9b0ee` — chore(starters): update dependencies
- `2c79c02` — chore(forms): drop unnecessary boolean conversions in checkbox mixin *(Cursor Agent)*
- `d6dc590` — chore(core): cover connected move in format-truncate *(Cursor Agent)*
- `6126e1c` — fix(docs): update responsive pattern icon *(Cormac Rada)*

**What's Cooking:** A healthy mix of CI/tool-maintenance (svgo bump, starter deps) and real feature work in the forms + core libraries — specifically cleaning up mixin logic and covering edge cases in utility components like `format-truncate`. Notably, **Cursor AI agents** are authoring a couple of the commits, which is itself a podcast-worthy signal about how NVIDIA's design-system ergonomics are being shaped by AI-assisted development. Semantic Release + commitlint governs publish.

**🎙️ Episode Ideas:**
- *"Building a Design System for Autonomous-Vehicle Consoles"* — Why UI for AV/robotics dashboards is a different beast.
- *"AI Agents Are Committing to NVIDIA's Repo"* — The rises of agent-authored design-system contributions.
- *"Web Components as the Universal Runtime for Robotics UIs"* — Framework agnosticism in practice.
- *"MCP, CLI, and AI Agent Harnesses"* — How NVIDIA exposes a design system to LLM tooling.

---

### 3. [willv678 / autolab-harness](https://github.com/willv678/autolab-harness)
⭐ 0 stars · 🐍 Python · (No license yet) · Forks: 0

**About:** An agentic test harness and orchestration framework for LLM-driven autonomous vehicle safety verification and automated red-teaming in closed-loop simulation. Runs inside NVIDIA AlpaSim: a local reasoning model (Qwen 2.5) evaluates rollout telemetry and iteratively mutates control/init boundaries to discover failures.

**Latest Commits (Sep 9–10, 2026):**
- `71513c0` — [draft] training script *(Will Varner, Sep 10)*
- `bdeb1b2` — result processing shell script *(Sep 10)*
- `068b046` — feat: complete initial harness, SFT formatter, and failure boundary plotting *(Sep 10)*
- `9f4f7ab` — feat: Initial commit of AutoLab agent harness and orchestrator *(Sep 9)*

**What's Cooking:** Brand-new repo (initial commit just yesterday) with a burst of focused work: the full orchestration loop, an SFT trace formatter (ChatML JSONL), failure-boundary plotting, and a draft training script. The entire arc — from "initial commit" to a working red-teaming + data-formatting pipeline — landed in ~48 hours. It's a fascinating micro-case of an individual researcher bootstrapping an LLM-as-judge / red-team tool for AV safety in simulation. Watch this one: it may be the smallest and newest on the radar but it points at a real trend (AI red-teaming autonomy).

**🎙️ Episode Ideas:**
- *"Red-Teaming Self-Driving Cars with LLMs"* — Using an agentic harness to break AV controllers in simulation.
- *"From Zero to Red-Team Pipeline in 48 Hours"* — A solo dev builds an AV safety tool (autolab story).
- *"Failure Boundaries & SFT: Turning Rollouts into Training Data"* — Deep-dive on plot_boundaries + format_sft.
- *"Is Autonomous-Vehicle Safety Verified by Simulation + AI?"* — Promise and limits of closed-loop red-teaming.

---

## 📡 How This Radar Works

Repos are sourced by topic (`:autonomous-vehicles`, `:robotics`) filtered for genuine, high-signal projects, then verified against their **latest commits** so the highlights reflect what's actually being worked on right now — not stale marketing copy. Star counts are a signal but not the only one; see "What's Cooking" for the real story behind each repo's activity.

---

## 🎙️ About This Project

`robotics-oss-radar` is the research backbone for an open-source robotics & autonomous-systems podcast. Each entry ties a live GitHub repo to concrete recent development highlights and a menu of potential episode topics.

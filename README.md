# 🤖 Robotics & Autonomous Systems — Open-Source Radar

> A living radar for the most active open-source robotics and autonomous-vehicles repos, with commit summaries and podcast episode ideas.

_Last radar sweep: 2026-09-10. Activity verified against each repo's latest commits via the GitHub API._

---

## 🔭 Top 3 Most Recently Active Projects

All three were among the most recently updated repos tagged `robotics` or `autonomous-vehicles` in the week of 2026-09-10. Selection favours genuine, high-signal work over raw star counts.

### 1. willv678 / autolab-harness
⭐ Topic: `autonomous-vehicles` · 🐍 Python · (No license yet) · Forks: 0

**What it is:** An agentic test harness and orchestration framework for **LLM-driven autonomous vehicle safety verification and automated red-teaming** in closed-loop simulation. It runs inside NVIDIA AlpaSim: a local reasoning model (Qwen 2.5) evaluates rollout telemetry and iteratively mutates control and initialization boundaries to discover failures. Repo: https://github.com/willv678/autolab-harness

**Recent development highlights (Sep 10, 2026):**
- `068b046` — feat: complete initial harness, SFT formatter, and failure boundary plotting
- `71513c0` — [draft] training script
- `bdeb1b2` — result processing shell script

A brand-new repo that went from "initial commit" (~48 hours earlier) to a working red-teaming + data-formatting pipeline: full orchestration loop (`autolab_loop.py`), ChatML JSONL SFT trace formatter (`format_sft.py`), telemetry parser / sensitivity-boundary scatter plotter (`plot_boundaries.py`), and a draft LoRA training script (`train_lora.py`). A compelling micro-case study of a solo researcher bootstrapping an LLM-as-judge safety tool for AVs.

**🎙️ Episode ideas:**
- *"Red-Teaming Self-Driving Cars with LLMs"* — breaking AV controllers in closed-loop simulation.
- *"From Zero to Red-Team Pipeline in 48 Hours"* — the autolab story.
- *"Failure Boundaries & SFT: Turning Rollouts into Training Data"* — deep-dive on plotting + formatting.
- *"Is AV Safety Verified by Simulation + AI?"* — promise and limits of closed-loop red-teaming.

---

### 2. ubrobotics-ai / nvidia-codefest-2026
⭐ Topic: `robotics` · 🐍 Python · License: Apache-2.0 · Forks: 0

**What it is:** Cluster-side scripts for **Team UBR Stack** (UB Robotics) at the NVIDIA Open Models Codefest 2026 — an offline-first **physical AI search-and-rescue teammate**. The edge robot (Jetson Orin Nano) keeps searching when the network degrades or drops, fed by a hybrid pipeline of real UGV/UAV footage plus synthetic scenes that run on NVIDIA B300 cluster nodes. Repo: https://github.com/ubrobotics-ai/nvidia-codefest-2026

**Recent development highlights (Sep 10, 2026):**
- `583f269` — Add audited INT4 quantise and export wrappers for Cosmos3-Edge
- `277f592` — Add the night-run analysis scripts and drop a cluster path from the docs
- `41366ea` — Add the L0 model x precision bake-off

Focused work on the synthetic-data side of Physical AI: (1) auditing INT4 quantize/export of `nvidia/Cosmos3-Nano` (16B image→video) for edge deployment, (2) batch generation of condition-variant clips (day, dusk smoke, night, dense smoke) from real UGV frames with timing sidecars, (3) indexing real rover blackbox recordings, and (4) a model-vs-precision bake-off to stay inside the GPU budget — all Apache-2.0 with a clean separation between cluster scripts and edge/robot code.

**🎙️ Episode ideas:**
- *"Physical AI Search & Rescue"* — offline-first autonomy for when the network goes down.
- *"Synthetic Data Pipelines for Robots"* — Cosmos 3 image→video and the emerging ML-engineer role in robotics.
- *"Edge AI on Jetson Orin Nano"* — INT4 quantization and model export for in-field inference.
- *"Open Models for Public-Sector Robotics"* — the Codefest theme and open-model licensing.

---

### 3. haidmoham / spider (C-1N)
⭐ Topic: `robotics` · 🐍 Python · (No license yet) · Forks: 0

**What it is:** **C-1N**, a six-legged MuJoCo hexapod simulation for reproducible standing control, locomotion experiments, and evaluation. Jupyter-first learning surface with a deterministic headless baseline and a rich telemetry system. Repo: https://github.com/haidmoham/spider

**Recent development highlights (Sep 10, 2026):**
- `722428d` — Merge PR #23: codex/assignment-scaffolding
- `0c9f7ea` — docs(practice): use assignment-sized policy exercises
- `7abb115` — Merge PR #22: codex/first-C1N-policy-lesson

Steady educational scaffolding work — merging policy-lesson PRs, refining assignment-sized exercises, and iterating on the `LEARNING.md` path toward learned locomotion. The codebase sits at the `C-1N v0.2 - STAND` checkpoint (reproducible six-contact support baseline), with `STRIDE` (sustained walking) as the next earned target. Notably disciplined: it preserves failure cases (the 1 mg shove) rather than cherry-picking pretty rollouts — a thoughtful counter-example to flashy-perfection highlights.

**🎙️ Episode ideas:**
- *"Teaching a Hexapod to Stand"* — reproducible baselines, support margins, and the art of the fail-case.
- *"Simulation-First Locomotion"* — why MuJoCo + Jupyter is a legit robotics dev environment.
- *"Don't Claim STRIDE from One Pretty Rollout"* — the discipline of reproducible evaluation in robotics research.
- *"From Stand to Walk: Milestone-Based Robotics Development"* — C-1N's checkpoint lineage (SPAWN → SHUFFLE → STAND → STRIDE).

---

## 📡 How This Radar Works

Repos are sourced by topic (`:autonomous-vehicles`, `:robotics`) and filtered for genuine, high-signal projects, then **verified against their latest commits** so the highlights reflect what's actually being worked on right now — not stale marketing copy. Star counts are a signal, not the only one; see "What's Cooking" for the real story behind each repo's activity.

---

## 🎙️ About This Project

`robotics-oss-radar` is the research backbone for an open-source robotics & autonomous-systems podcast. Each entry ties a live GitHub repo to concrete recent development highlights and a menu of potential episode topics.

---

_Data sourced from GitHub repository metadata and latest-commit inspection (week of 2026-09-10). All repository names, logos, and trademarks are property of their respective owners._

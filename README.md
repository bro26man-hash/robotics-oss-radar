# 🤖 Robotics OSS Radar

A living research hub tracking the most active open-source robotics and autonomous-systems projects on GitHub — curated for the **Robotics OSS Podcast**. Each entry captures recent development highlights and angles worth turning into an episode.

_Last radar sweep: 2026-09-10._

---

## How to Use This Repo

- **Top Projects** — the 3 most recently active, high-impact repos we're tracking.
- **Episode Ideas** — podcast angles drawn from each project's current work.
- **Projects to Revisit & Upcoming Releases** — a living checklist (see the issue of the same name) for follow-up episodes.
- Raise a PR or issue to suggest adding / retiring a project from the radar.

---

## 🔭 Top 3 Most Recently Active Projects

All three below were among the most recently updated in the week of 2026-09-10 and sit at the intersection of community momentum and technical substance.

### 1. NVIDIA Cosmos ⭐ 11,794

**Repo:** [NVIDIA/cosmos](https://github.com/NVIDIA/cosmos) · **License:** NOASSERTION (NVIDIA release) · **Language:** Jupyter Notebook

**What it is:** An open platform of world models, datasets, and tools for building **Physical AI** — robots, autonomous vehicles, and smart infrastructure. The newest generation, **Cosmos 3**, is an omnimodal world model (Mixture-of-Transformers) that unifies a **Reasoner** (text/vision → text) and a **Generator** (text/vision/sound/action → vision/sound/action) in a single framework.

**Recent dev highlights:**
- Active Cosmos 3 rollout in the 9/4–9/10 window: NIM docs, the "Certified NIM" environment-setup guide, a SGLang transfer-test script, and a new **RoboCasa mobile-manipulation post-training recipe** (#318).
- Rich inference serving stack — vLLM-Omni, SGLang Diffusion, TensorRT-LLM, and NVIDIA NIM containers — plus a full Diffusers research path and Transformers Reasoner path.
- Post-training focus: supervised fine-tuning (SFT) recipes for action, vision, and reasoner workflows are landing ("Coming Soon" → in progress), along with distill/export tooling.

**Why it matters for the show:** Cosmos is effectively NVIDIA's open bet that *world models* are the next substrate for robotics and autonomy — blending video generation with action/physics reasoning. It's a rich "foundation model meets the physical world" story.

**🎙️ Episode angles:**
- "World Models for Robotics" — from simulated rollouts to real policies (generator vs. reasoner modes).
- Democratizing Physical AI — how open weight/model access (Cosmos 3 Nano/Super/Edge) changes who can build AV and robot policies.
- Synthetic data & sim-to-real: generating training rollouts instead of collecting them.
- The serving jungle — vLLM-Omni, SGLang, TensorRT-LLM, NIM — what's actually shipping today.

**⚠️ Note:** Resource-heavy (large downloads, CUDA 12.8/13, strong GPU). Good "how to get started" episode, not a 5-min showcase.

---

### 2. OpenBot ⭐ 3,485

**Repo:** [ob-f/OpenBot](https://github.com/ob-f/OpenBot) · **License:** MIT · **Language:** Swift

**What it is:** Turns **smartphones into robot brains**. A ~$50 electric vehicle body plus an Android (and now iOS) software stack supporting person following and real-time autonomous navigation. Built on work from the Intel Labs / Vladlen Koltun group (ICRA 2021 paper).

**Recent dev highlights:**
- Ongoing mobile-app hardening in Aug 2026: updated Android package name + target API/Gradle (#534), iOS bundle identifier standardization (#535), iOS in-app language support with flag icons + Settings redesign (#531), and Node.js controller compatibility widened to Node 18–25 (#511).
- New **node-js controller command tests** and a `DriveValue.read` rounding fix (#537) — signs of a maturing cross-platform controller layer.
- Multi-language documentation (EN, ZH-CN, DE, FR, ES, KO) and an active community (Slack, videos, 3rd-party builds).

**Why it matters for the show:** The ultimate "democratization" story — $50 hardware + a smartphone gives you perception and navigation. It's the counterpoint to massive-budget AV: what autonomy looks like at the bottom of the cost curve.

**🎙️ Episode angles:**
- "Autonomy on $50" — smartphone-as-brain vs. custom compute; what you gain and lose.
- Cross-platform robotics software — building one stack that runs on Android *and* iOS.
- From sample deployment to your own driving policy (the `policy/` module and RL-on-phone ideas).
- Community corner: cool DIY builds built on OpenBot (tank, cardboard chassis, etc.).

**⚠️ Note:** Relies on physical hardware to fully demo; can still be covered via the software stack, controller/web UI, and policy-training story.

---

### 3. NVIDIA Alpamayo ⭐ 2,019

**Repo:** [NVlabs/alpamayo](https://github.com/NVlabs/alpamayo) · **License:** Apache-2.0 (code) / OpenMDW-1.1 (weights) · **Language:** Python

**What it is:** An open **10B-parameter reasoning Vision-Language-Action (VLA) model for autonomous vehicles**. Alpamayo-R1 pairs driving trajectories with **Chain-of-Causation (CoC) reasoning** — a Cosmos-Reason backbone + action diffusion expert delivering a 6.4s, 64-waypoint @10Hz trajectory forecast. Note: this repo is in maintenance mode; active development has moved to **[NVlabs/alpamayo-recipes](https://github.com/NVlabs/alpamayo-recipes)** (SFT + RL post-training) and the newer **Alpamayo 1.5 / Alpamayo 2** family.

**Recent dev highlights:**
- Fine-tuning + post-training landed: SFT script (April 2026), RL pipeline via Cosmos-RL; both subsequently migrated to the **Alpamayo Recipes** hub.
- CUDA-graph acceleration for the diffusion expert (`enable_diffusion_expert_cuda_graph`) to cut inference launch overhead on repeated trajectory queries.
- Maintenance-state note: the maintainers explicitly redirect users to `alpamayo-recipes` and the Alpamayo 1.5/2 models — a signal that the *post-trained* generations are where the action is.

**Why it matters for the show:** Alpamayo is the "reasoning driver" — a model that doesn't just predict a trajectory but *explains* its reasoning chain, bridging the gap between coherent world-model reasoning and low-level vehicle control. The migration to a recipes + newer-model ecosystem is itself an interesting governance/community story.

**🎙️ Episode angles:**
- "The reasoning driver" — Chain-of-Causation reasoning behind the wheel; why traceability matters for AV safety.
- VLA models 101 — how a single vision-language-action backbone replaces modular perception→planning→control stacks.
- From model to ecosystem: release, maintenance-mode, recipes hub — how NVIDIA is open-sourcing *process*, not just weights.
- Alpamayo 1.5 vs. 1.0: what the newer generations add (compare with latest commit cadence on `alpamayo-recipes`).

**⚠️ Note:** 24 GB+ VRAM GPU required for inference. Weigh the "newer versions available / maintenance mode" caveat carefully in the episode framing.

---

## 🎬 Cross-Cutting Podcast Themes

| Theme | Projects | Angle |
|-------|----------|-------|
| **World models + synthetic data** | Cosmos, Alpamayo (VLA reasoning) | Sim-to-real, generating driving data instead of collecting it |
| **Democratization of autonomy** | OpenBot, Cosmos (Edge) | High-end AV vs. $50 robot; open tooling lowering the bar |
| **Reasoning + action** | Alpamayo, Cosmos Reasoner | From chain-of-thought to steering/throttle |
| **Open vs. "open"** | All three | Apache/MIT/NVIDIA release licenses; what "open" really means for weights, data & governance |
| **Serving & deployment** | Cosmos (vLLM/SGLang/NIM), OpenBot (Node controller, mobile) | How you actually run these things in production |

---

## 📅 Suggested Release/Revisit Cadence

- **Per-project deep dives** — one episode each for Cosmos, OpenBot, Alpamayo (in this order works well: big-vision → low-cost → reasoning-driver).
- **Ecosystem check-ins** — revisit this radar monthly / snapshots of commit cadence, new releases, and episode-worthy moves.
- **Listener challenge** — spin up a Cosmos Generator path / train an OpenBot policy / run Alpamayo inference; report back.

---

## Contributing

Found a more recently active repo? Spot a stale commit detail? Open an issue or PR and we'll cross-check against the latest `git log` before updating the radar.

---

_Data sourced from GitHub repository metadata and latest-commit inspection (week of 2026-09-10). All repository names, logos, and trademarks are property of their respective owners._

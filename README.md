# 🤖 Robotics OSS Radar

> Open-source robotics & autonomous systems — tracking the most active projects, recent development highlights, and podcast episode topics.

## 📡 Why This Radar?

For hosts, reporters, and engineers who want to stay on top of what's actually being *built* in open-source robotics — not just what's being announced. We track the repos with the freshest commit activity, summarize what's changing, and surface episode-worthy stories.

---

## 🔍 Tracked Projects

### 1. [autowarefoundation/openadkit](https://github.com/autowarefoundation/openadkit)
**Containerized Components for Autoware** · Apache-2.0 · 11 ⭐ · 10 🍴

The first **SOAFEE blueprint** for deploying Autoware as containerized, cloud/edge-ready, software-defined vehicle components. Provides component images, deployment configurations, versioned runtime bundles, and CI metadata.

| Deployment | Description |
|---|---|
| `planning-simulation` | Planning with simulator-backed vehicle interface |
| `logging-simulation` | Replay sample data through logging/perception stack |
| `scenario-simulation` | Scenario-based simulation workflows |
| `carla-simulation` | Connect Autoware to CARLA (Humble, amd64, GPU) |
| `zenoh-bridge` | Bridge isolated edge and visualization ROS domains |

**Latest Commits (Sep 2026):**

| Date | Commit | What's Happening |
|---|---|---|
| Sep 17 | `ba151c1` — docs: align product documentation and publication (#111) | Documentation overhaul to align published docs with actual product capabilities |
| Sep 15 | `98137cc` — feat: add unified dual-distro release pipeline (#113) | New CI pipeline building and releasing for Ubuntu 22.04 AND 24.04 in one flow |
| Sep 9 | `21bc68e` — feat: add manifest-driven deployment CLI (#138) | Manifest-driven CLI that pulls images, starts the stack, and verifies readiness — openadkit run planning-simulation just works |

**🎙️ Potential Episode Topics:**
- "From Source to Container: How Autoware is Shipping SDV Stacks" — the dual-distro pipeline, OCI images, and what it means for production AV deployments
- "CARLA + Autoware: Closing the Simulation-to-Real Gap" — the carla-simulation deployment and Zenoh bridge for ROS domain isolation
- "SOAFEE: The Standardization Layer Nobody Talks About" — why a common deployment spec matters for the AV ecosystem

---

### 2. [lololem/diamants-collab](https://github.com/lololem/diamants-collab)
**DIAMANTS — Distributed Intelligence & Swarm Robotics** · PolyForm Noncommercial · 0 ⭐ (new & growing)

**Fly a drone swarm in your browser, and plug in your own intelligence.** A heterogeneous fleet of Crazyflie micro-drones, X500/S500 cognitive platforms, and Colossus tracked UGVs simulation. Rendering, flight physics, and collision avoidance handled — you bring the coordination algorithm.

**The Neurosymbolic Contract:** Models propose → symbolic rules dispose. A model that times out, answers garbage, or proposes something forbidden changes nothing — the drone keeps flying on reactive behavior.

| Module | Status |
|---|---|
| Swarm exploration & flight physics | ✅ Working |
| Stigmergy engine (pheromone trails) | 🧪 Shell — waiting for your algorithm |
| Distributed swarm engine | 🧪 Shell |
| LLM Intelligence (Ollama / custom providers) | ✅ Wired, demo with simulated decisions |
| Wildfire response (3-tier: survey → inspect → suppress) | 🎬 Filmed, code being finalized |

**Latest Commits (Sep 2026):**

| Date | Commit | What's Happening |
|---|---|---|
| Sep 17 | `256a5c5` — feat: bring your own drone and model — neurosymbolic contract | **Major feature**: full neurosymbolic bridge — plug in any model (LLM, RL policy, ONNX) with a deterministic rule layer vetoing unsafe actions |
| Sep 16 | `f763e46` — docs: cleaner badge labels | README polish |
| Sep 16 | `7909c36` — docs: live demo and film player as badges | Added links to the live browser demo and two 2026 demonstration films (unmapped sector recon + wildfire response) |

**🎙️ Potential Episode Topics:**
- "Neurosymbolic AI on a Drone: Why Your LLM Can't Fly a Quadcopter (And How to Fix That)" — the model-proposes-rules-dispose pattern
- "Swarm Robotics Without a Leader: Stigmergy, Consensus, and Emergent Coordination" — decentralized task allocation in the wildfire scenario
- "From Simulation to Field: What It Takes to Fly 11 Drones in a Browser" — Three.js, WebGL, PID physics, and the engineering behind the frontend
- "Wildfire Response: A 3-Tier Swarm with No Dispatcher" — the upcoming mission where micro-drones survey, camera platforms confirm with YOLO, and UGVs suppress

---

### 3. [NVIDIA/skills](https://github.com/NVIDIA/skills)
**Agent Skills for NVIDIA Products — Physical AI, Robotics, CUDA & More** · Apache-2.0 + CC-BY-4.0 · 3,324 ⭐ · 397 🍴

Official, **NVIDIA-verified** agent skills for Claude Code, Codex, Cursor, and other AI coding agents. A catalog of 200+ portable instruction sets covering Isaac for Healthcare, Holoscan, Jetson, TAO, Warp, Physical AI Data Factory, and more. Every skill ships with OMS signature verification, Tier-3 evaluation datasets, and benchmark reports.

**Key Robotics-Adjacent Skill Families:**

| Family | Highlights |
|---|---|
| **Isaac for Healthcare** | Catheter navigation, digital twins, DRR rendering, RL training & validation (15 skills) |
| **Holoscan SDK / Sensor Bridge** | FPGA flashing, real-time signal processing, sensor pipeline workflows (20+ skills) |
| **Jetson BSP / Device** | Board bring-up, camera customization, inference tuning, LLM serving on edge (40+ skills) |
| **TAO Toolkit** | Fine-tune 100+ vision models — BEVFusion, PointPillars, RT-DETR, and more (60+ skills) |
| **Physical AI Data Factory** | Synthetic data generation, auto-labeling, augmentation, and curation pipelines (10+ skills) |
| **Warp** | GPU-accelerated simulation and ML — compile-time optimization, gradient debugging (3 skills) |

**Latest Commits (Sep 2026):**

| Date | Commit | What's Happening |
|---|---|---|
| Sep 17 | `08ea07e` — chore(metadata): regenerate metadata.json, skills.sh.json, benchmarks.json, and versions.json | Daily metadata refresh — catalog is actively maintained and growing |
| Sep 17 | `7619498` — chore: sync skills (catalog maintenance) | Routine daily sync from upstream product repos |
| Sep 17 | `165d900` — [catalog] register Isaac Mission Control manual component | **New product registered**: Isaac Mission Control skills now in the catalog |

**🎙️ Potential Episode Topics:**
- "AI Agents That Know Your GPU: Inside NVIDIA's 200+ Skill Catalog" — what it takes to verify and sign agent skills at scale
- "Isaac for Healthcare: Training Robots to Navigate Blood Vessels" — catheter navigation, digital twins, and RL in the clinical domain
- "From Notebook to Edge: The Jetson Skill Pipeline" — how agents can now flash, customize, and validate Jetson boards autonomously
- "The Trust Pipeline: OMS Signatures and Why Agent Skills Need Verification" — supply-chain security for AI agent instructions

---

## 📋 How to Use This Radar

1. **Browse** the tracked projects above for fresh open-source developments
2. **Listen** — each project has curated episode topics ready for your podcast
3. **Contribute** — suggest new projects, correct highlights, or propose episode outlines by opening an issue
4. **Track** — see the Projects to Revisit & Upcoming Releases issue for a living checklist

---

## 🔗 Quick Links

- [Autoware OpenAD Kit](https://github.com/autowarefoundation/openadkit) — Containerized SDV components
- [DIAMANTS Swarm Robotics](https://github.com/lololem/diamants-collab) — Neurosymbolic drone swarm simulation
- [NVIDIA Agent Skills](https://github.com/NVIDIA/skills) — Verified skills for Physical AI & robotics
- [Issues](../../issues) — Track upcoming releases and revisit lists
- [Discussions](../../discussions) — Share episode ideas and feedback

---

## 📜 License

This radar is released under the **MIT License** — use it, fork it, build on it. Individual projects retain their own licenses.

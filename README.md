# 🤖 Robotics OSS Radar

> **Open-source robotics & autonomous systems — podcast companion**
> Tracking the most recently active repositories, recent commits, and episode ideas for your show.

---

## 📡 Why This Radar?

The open-source robotics and autonomous-vehicles ecosystem is moving fast. To keep your podcast audience informed, we track the **most recently active** projects, distill what's being worked on, and surface **episode-worthy stories** — from multi-UAV swarms to robot-cell observability to safety-caged RL training.

---

## 🔍 Tracked Projects

### 1. 🏭 Metriplane — Physical Observability for Robotics Workcells
| | |
|---|---|
| **Repo** | [Miko997/metriplane](https://github.com/Miko997/metriplane) |
| **Language** | Python |
| **Topic** | `robotics` |
| **Last Activity** | **September 18, 2026** — PR #133 merged (production owner keyring delegation) |
| **Stars** | 7 |
| **Contributors** | Miko Parkkinen + automated health-publisher bot |

**What it is:** Open-source **physical observability** for robotics workcells. It provides deterministic replay, verifiable incident evidence, and generated regression tests — essentially making robotics workflows auditable and reproducible the way software DevOps makes code deployments traceable.

**Recent development highlights:**
- **PR #133 merged (Sept 18, 2026)** — Agent now registers production-delegation public keys, extending the security and traceability model to production environments.
- **PR #85 merged (Sept 14, 2026)** — AMR (Autonomous Mobile Robot) perspective work lands, adding a dedicated view for AMR use cases including replay and quote generation.
- **Active agent development** — Multiple agent-driven PRs (#131, #133) show the project is building toward automated, agent-assisted observability workflows.
- **SoftwareX licence integration** — PR #131 adds proper licensing infrastructure, signaling maturity and readiness for broader adoption.
- **Deterministic replay pipeline** is the killer feature: record a robot cell's execution, then replay it bit-for-bit to reproduce incidents or validate changes.

**🎙️ Potential episode topics:**
- *"Why Your Robot Can't Be Witnessed — and How Metriplane Fixes That"* — the case for observability in physical systems.
- *"Deterministic Replay for Robotics: rrRulez?"* — how replay-driven development could change how we test robots.
- *"From Black Box to Glass Box: Making Robot Cells Auditable"* — the intersection of safety compliance and open-source tooling.
- *"Agents That Watch Robots Watch Themselves"* — the emerging role of AI agents in robotics observability.

---

### 2. 🛸 AeroWeaver — Multi-UAV Coordination Console
| | |
|---|---|
| **Repo** | [Admire-ljb/AeroWeaver](https://github.com/Admire-ljb/AeroWeaver) |
| **Language** | Python |
| **Topic** | `robotics` |
| **Last Activity** | **September 18, 2026** — 5 commits: docs overhaul, CI stabilization, preprint citation |
| **Stars** | 3 |

**What it is:** A **multi-UAV coordination console** for planning and executing manual and LLM-driven missions. It bridges the gap between low-level swarm protocols and high-level mission intent, letting operators control fleets of drones through natural language or direct commands.

**Recent development highlights:**
- **Massive docs overhaul (Sept 18, 2026)** — 4 of 5 commits were documentation work: restructuring the README around core capabilities, moving details into separate usage guides, replacing homepage screenshots with updated layouts, and citing the AeroWeaver preprint.
- **CI stabilization** — Commit `685f5e9` fixed the pursuit (pursuit-evasion) test pipeline and formally cited the research preprint, signaling the project is transitioning from research prototype to citable, reproducible tool.
- **README quickstart validation** — Commit `262b7d9` added automated validation tests for the README quickstart guide, a sign of serious engineering discipline.
- **LLM-driven mission planning** — the headline feature: operators can describe missions in natural language and the system generates coordinated multi-UAV plans.
- **Preprint now citable** — the project has a research paper behind it, making it credible for academic and industrial adoption.

**🎙️ Potential episode topics:**
- *"Swarming Drones with Your Voice: AeroWeaver's LLM Interface"* — how large language models are changing multi-robot command.
- *"From Research Paper to Production Repo: The AeroWeaver Journey"* — what it takes to make a swarm framework citable and usable.
- *"Pursuit-Evasion Swarms: The Math Behind Drone Tag"* — the game-theory algorithms powering coordinated UAV motion.
- *"Why Every Swarm Needs a Console"* — the missing UX layer in multi-robot systems.

---

### 3. 🛡️ SE4AI Safety Cages for Autonomous Driving (CobraFlex)
| | |
|---|---|
| **Repo** | [snchz46/MT-SE4AI-Safe-RL-Cobraflex](https://github.com/snchz46/MT-SE4AI-Safe-RL-Cobraflex) |
| **Language** | Python |
| **Topic** | `autonomous-vehicles` |
| **Last Activity** | **September 18, 2026** — 5 commits on Chapter 6 draft writing (thesis closure) |
| **Stars** | 1 |
| **License** | MIT |

**What it is:** Full research artifacts for a master's thesis at Hochschule Esslingen investigating how **runtime safety cages** can constrain a Reinforcement Learning agent in an autonomous driving context. Built on a 1:14 scale physical vehicle (CobraFlex) with 360° LiDAR, stereo camera, and skid-steer drive, simulated in Gazebo with ROS 2.

**Recent development highlights:**
- **Thesis sprint in full gear (Sept 18, 2026)** — 5 commits all titled "E6: draft writing v6," showing the author is in the final sprint of Chapter 6 (closure & defence, Gate G6).
- **Phase 5 (physical deployment) just closed** — the sim-to-real transfer was validated: the PPO policy drove 18.05 m of the real circuit uninterrupted with **zero safety interventions**.
- **1,890 simulation runs across 27 scenarios** completed — nominal, edge-case, and perturbed conditions all logged and traceable.
- **Traceability gate is rigorous** — every hazard (H-01…H-12) traces through safety requirements → cage rules → scenarios → metrics → logged evidence. A mechanical check (`check_traceability.py`) blocks any Gate review with orphans.
- **Shocking finding:** The reward-peak checkpoint (475k steps) was actually the *worst* performer; selecting by training reward alone would have picked the wrong model. The cage-intervention rate was the real discriminating signal.
- **Results:** 5.32 continuous laps on `complex_b`, 8.6 mm mean lateral error, 27 mm max, **0 emergencies, 0 safety interventions** — only the benign C-06 rate limiter fired.

**🎙️ Potential episode topics:**
- *"Wrapping AI in a Safety Cage: Can We Trust an RL Driver?"* — the SE4AI methodology and why traceability matters.
- *"The Checkpoint That Looked Best But Was Actually Worst"* — why training reward is a terrible proxy for real-world safety.
- *"Sim-to-Real Transfer of an End-to-End Camera Policy"* — what it takes to move from Gazebo to a physical 1:14 car.
- *"12 Hazards, 14 Requirements, 6 Cage Rules: The Math of Autonomous Safety"* — the engineering behind runtime monitoring.
- *"From Simulation to Hardware: Phase 5 Closes on CobraFlex"* — the emotional journey of a thesis defense.

---

## 📊 Summary Dashboard

| Project | Domain | Activity Level | Episode Potential | Maturity |
|---|---|---|---|---|
| Metriplane | Robotics Observability | 🔥 Very High (agent-driven PRs) | ⭐⭐⭐⭐ | Advanced / Production |
| AeroWeaver | Multi-UAV Coordination | 🔥 Very High (docs + CI sprint) | ⭐⭐⭐⭐⭐ | Research → Production |
| SE4AI CobraFlex | Safety-Caged RL | 🔥 Very High (thesis sprint) | ⭐⭐⭐⭐⭐ | Advanced / Publishing |

---

## 🎙️ Podcast Episode Pipeline

| Priority | Episode Title | Featured Project | Angle |
|---|---|---|---|
| 🔴 **1** | *"The Safety Cage: Wrapping AI in a Life-or-Death Box"* | SE4AI CobraFlex | Deep-dive into runtime safety monitoring |
| 🔴 **2** | *"Swarming Drones with Your Voice"* | AeroWeaver | LLM-driven multi-UAV coordination |
| 🟡 **3** | *"Why Your Robot Can't Be Witnessed"* | Metriplane | Observability and deterministic replay |
| 🟡 **4** | *"The Checkpoint That Lied"* | SE4AI CobraFlex | Why training metrics deceive |
| 🟢 **5** | *"From Research Paper to Production Repo"* | AeroWeaver | Making a swarm framework citable |
| 🟢 **6** | *"Agents That Watch Robots Watch Themselves"* | Metriplane | AI agents in robotics observability |

---

## 🔧 How to Use This Radar

1. **Browse** the tracked projects above for ready-to-record episode ideas.
2. **Watch** the `Projects to Revisit & Upcoming Releases` issue for a checklist of what to track next.
3. **Contribute** by opening a PR with your own project picks or episode drafts.
4. **Subscribe** to each repo's release notifications so you never miss an update.

## 🤝 Contributing

- Found an active robotics repo worth tracking? Open an issue!
- Have an episode outline? PRs welcome.
- Want to co-host a segment? Let's discuss.

## 📜 License

This radar is open-source under the [MIT License](LICENSE). All tracked project repos have their own licenses — check each one before reusing code.

---

*Built for the open-source robotics community. Follow the radar, don't get lost in the noise.*
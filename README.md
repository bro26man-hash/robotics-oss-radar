# 🤖 Robotics OSS Radar

> **Open-source robotics & autonomous systems — podcast companion**
> Tracking the most recently active repositories, recent commits, and episode ideas for your show.

---

## 📡 Why This Radar?

The open-source robotics and autonomous-vehicles ecosystem is moving fast. To keep your podcast audience informed, we track the **most recently active** projects, distill what's being worked on, and surface **episode-worthy stories** — from safety-cage research to cloud-based RL training to industrial simulation.

---

## 🔍 Tracked Projects

### 1. 🚗 PhysiCar DeepRacer for Cloud
| | |
|---|---|
| **Repo** | [PoetAndPoem4Hu/physicar-deepracer-for-cloud](https://github.com/PoetAndPoem4Hu/physicar-deepracer-for-cloud) |
| **Language** | Java |
| **Topic** | `autonomous-vehicles` |
| **Last Activity** | **September 18, 2026** — README overhaul |
| **Stars** | 0 |

**What it is:** A platform from PhysiCar AI that lets you train AWS DeepRacer reinforcement-learning models in the cloud. It simplifies the setup of cloud-based RL environments for autonomous-vehicle research and education.

**Recent development highlights:**
- **README redesigned** (Sept 2026) — the project just refreshed its documentation, signaling renewed community interest and onboarding improvements.
- **Version 1.2** released back in 2019, with README updates in 2025 and 2026 suggesting the maintainer is re-activating the project after a long dormancy.

**🎙️ Potential episode topics:**
- *"Cloud-Native RL: Training Autonomous Cars Without a Garage"* — how cloud platforms are democratizing RL for AV research.
- *"From Toy Car to Thermal Runway: The DeepRacer Ecosystem"* — the gap between simulation toys and real autonomy stacks.
- *"Why Did PhysiCar Revive This Repo?"* — discovering what re-awakens dormant open-source projects.

---

### 2. 🛡️ SE4AI Safety Cages for Autonomous Driving (CobraFlex)
| | |
|---|---|
| **Repo** | [snchz46/MT-SE4AI-Safe-RL-Cobraflex](https://github.com/snchz46/MT-SE4AI-Safe-RL-Cobraflex) |
| **Language** | Python |
| **Topic** | `autonomous-vehicles` |
| **Last Activity** | **September 18, 2026** — 5 commits on draft writing (Chapter 6 of thesis) |
| **Stars** | 1 |
| **License** | MIT |

**What it is:** Full research artifacts for a master's thesis at Hochschule Esslingen investigating how **runtime safety cages** can constrain a Reinforcement Learning agent in an autonomous driving context. Built on a 1:14 scale physical vehicle (CobraFlex) with 360° LiDAR, stereo camera, and skid-steer drive, all simulated in Gazebo with ROS 2.

**Recent development highlights:**
- **Active thesis writing** — 5 commits on September 18 alone, all titled "E6: draft writing v6," showing the author is in the final sprint of Chapter 6 (closure & defence, Gate G6).
- **Phase 5 (physical deployment) just closed** on September 1, 2026 — the sim-to-real transfer was validated: the PPO policy drove 18.05 m of the real circuit uninterrupted with **zero safety interventions**.
- **Massive validation campaign** — 1,890 simulation runs across 27 scenarios (nominal, edge-case, perturbed) are complete; the verdict campaign data is fresh and being analyzed.
- **Traceability gate is rigorous** — every hazard (H-01…H-12) traces through safety requirements → cage rules → scenarios → metrics → logged evidence. A mechanical check (`check_traceability.py`) blocks any Gate review with orphans.
- **Key finding:** The reward-peak checkpoint (475k steps) was actually the *worst* performer; selecting by training reward alone would have picked the wrong model. The cage-intervention rate was the discriminating signal.
- **Results at a glance:** 5.32 continuous laps on `complex_b`, 8.6 mm mean lateral error, 27 mm max, **0 emergencies, 0 safety interventions** — only the benign C-06 rate limiter fired.

**🎙️ Potential episode topics:**
- *"Wrapping AI in a Safety Cage: Can We Trust an RL Driver?"* — the SE4AI methodology and why traceability matters.
- *"The Checkpoint That Looked Best But Was Actually Worst"* — why training reward is a terrible proxy for real-world safety.
- *"Sim-to-Real Transfer of an End-to-End Camera Policy"* — what it takes to move from Gazebo to a physical 1:14 car.
- *"12 Hazards, 14 Requirements, 6 Cage Rules: The Math of Autonomous Safety"* — the engineering behind runtime monitoring.
- *"From Simulation to Hardware: Phase 5 Closes on CobraFlex"* — the emotional journey of a thesis defense.

---

### 3. 🏭 Sim-Foundry — Virtual Factory Simulator
| | |
|---|---|
| **Repo** | [wailhoud/sim-foundry](https://github.com/wailhoud/sim-foundry) |
| **Language** | Python |
| **Topic** | `autonomous-vehicles` (industrial automation & robotics) |
| **Last Activity** | **September 18, 2026** — initial commit (`88a953b`) |
| **Stars** | 0 |
| **License** | MIT |

**What it is:** A free, open-source platform that simulates PLCs, industrial cameras, sensors, conveyor belts, robotic arms, and more — so you can test HMI, IoT gateway, and SCADA software without waiting for hardware. Supports Modbus, OPC-UA, MQTT, and cloud integrations (AWS IoT, Azure IoT Hub).

**Recent development highlights:**
- **Brand-new repo** — first commits landed on September 17–18, 2026. This is a fresh project looking for early adopters and contributors.
- **Full-stack architecture** — includes Docker/Kubernetes deployment, a web frontend, Grafana dashboards, database migrations (Alembic), and an SDK for custom device profiles (JavaScript).
- **Enterprise-ready design** — built with security in mind (local-only execution, corporate IT policy compliance) and designed for VMs and containers.
- **Rich documentation** — comprehensive README covers setup, troubleshooting, use cases, and FAQ. Migration scripts and CI/CD pipelines already in place.
- **Protocol support** — Modbus TCP, OPC-UA, MQTT out of the box; cloud-compatible with AWS IoT Core, Azure IoT Hub, Google Cloud IoT.

**🎙️ Potential episode topics:**
- *"Why You Shouldn't Need $50K in Hardware to Test Your Robot"* — the case for industrial simulation.
- *"From PLC to Kubernetes: How Sim-Foundry Modernizes Factory Testing"* — bridging legacy industrial protocols with modern DevOps.
- *"Build Your Own Digital Twin (For Free)"* — getting started with Sim-Foundry for robotics R&D.
- *"Robotics in the Enterprise: When Simulation Replaces the Hardware Roundtrip"* — real stories from engineers who ditched the procurement queue.

---

## 📊 Summary Dashboard

| Project | Domain | Activity Level | Episode Potential | Maturity |
|---|---|---|---|---|
| PhysiCar DeepRacer | Cloud RL Training | 🔄 Re-activating | ⭐⭐⭐ | Early / Dormant |
| SE4AI CobraFlex | Safety-Caged RL | 🔥 Very High (thesis sprint) | ⭐⭐⭐⭐⭐ | Advanced / Publishing |
| Sim-Foundry | Industrial Simulation | 🆕 Brand New | ⭐⭐⭐⭐ | Early / Fresh |

---

## 🎙️ Podcast Episode Pipeline

| Priority | Episode Title | Featured Project | Angle |
|---|---|---|---|
| 🔴 **1** | *"The Safety Cage: Wrapping AI in a Life-or-Death Box"* | SE4AI CobraFlex | Deep-dive into runtime safety monitoring |
| 🔴 **2** | *"Why Your Robot Doesn't Need Your Hardware Budget"* | Sim-Foundry | Industrial simulation for robotics |
| 🟡 **3** | *"Cloud Kernels: Training Autonomy at Scale"* | PhysiCar DeepRacer | Cloud RL and the democratization of AV research |
| 🟡 **4** | *"The Checkpoint That Lied"* | SE4AI CobraFlex | Why training metrics deceive and how to catch it |
| 🟢 **5** | *"From Garage to Gazebo: Sim-to-Real Transfers"* | SE4AI CobraFlex | The full journey from simulation to hardware |

---

## 🔧 How to Use This Radar

1. **Browse** the tracked projects above for ready-to-record episode ideas.
2. **Watch** the `Projects to Revisit & Upcoming Releases` issue for a checklist of what to track next.
3. **Contribute** by opening a PR with your own project picks or episode drafts.
4. **Subscribe** to each repo's release notifications so you never miss an update.

---

## 🤝 Contributing

- Found an active robotics repo worth tracking? Open an issue!
- Have an episode outline? PRs welcome.
- Want to co-host a segment? Let's discuss.

## 📜 License

This radar is open-source under the [MIT License](LICENSE). All tracked project repos have their own licenses — check each one before reusing code.

---

*Built for the open-source robotics community. Follow the radar, don't get lost in the noise.*
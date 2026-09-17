# 🤖 Robotics OSS Radar

> Tracking the most active open-source robotics & autonomous vehicle projects — for our podcast.

## 📡 Top 3 Projects Under the Lens

---

### 1. [autowarefoundation/openadkit](https://github.com/autowarefoundation/openadkit)
**⭐ 11 stars | Language: Shell | License: Apache-2.0 | Last updated: Sept 17, 2026**

*Open AD Kit — the first SOAFEE blueprint for deploying Autoware as containerized, cloud/edge-ready software-defined vehicle components. Provides component images, deployment configurations, a versioned runtime bundle, and CI metadata to run and ship Autoware-based stacks more predictably.*

**Recent Development Highlights:**
- **Unified dual-distro release pipeline** (`98137cc`, Sept 15, 2026) — new CI pipeline enabling releases for both Ubuntu 22.04 and 24.04, expanding platform reach
- **Manifest-driven deployment CLI** (`21bc68e`, Sept 9, 2026) — major feature: a CLI tool that uses manifest files to orchestrate deployment of the entire Autoware stack with a single command
- **MRM before/after demo with stop-distance grading** (`aa7a28a`, Sept 2, 2026) — new demonstration showcasing the MRM (Motion Reasoning Module) with quantitative stop-distance evaluation
- **Open AD Kit component stack on AutoSD for R-Car X5H** (`774c459`, Sept 1, 2026) — hardware-specific integration for Renesas R-Car X5H SoC, pushing Autoware onto real edge hardware
- **Documentation alignment & publication** (`ba151c1`, Sept 17, 2026) — docs overhaul ensuring product documentation matches the latest release

**Key Deployments:** planning-simulation, logging-simulation, scenario-simulation, carla-simulation (Humble, amd64, GPU), and a standalone zenoh-bridge for bridging isolated edge and visualization ROS domains.

**🎙️ Potential Episode Topics:**
- "SOAFEE and the future of cloud-edge autonomous driving — inside Open AD Kit's containerized stack"
- "From source to deploy: how the manifest-driven CLI changes Autoware adoption"
- "Running Autoware on real hardware: the R-Car X5H integration story"
- "What is MRM? Understanding Motion Reasoning in open-source AV stacks"
- "Zenoh and ROS 2: bridging isolated domains for edge autonomy"

---

### 2. [lololem/diamants-collab](https://github.com/lololem/diamants-collab)
**⭐ 0 stars | Language: JavaScript | License: PolyForm Noncommercial 1.0.0 | Last updated: Sept 17, 2026**

*DIAMANTS — an open-source platform for distributed intelligence and swarm robotics. Unites ROS 2, Python/Mesa, WebGL, and Kubernetes into a scalable stack enabling real-time orchestration of autonomous systems, from collaborative simulation to large-scale drone operations. "Fly a drone swarm in your browser, and plug in your own intelligence."*

**Recent Development Highlights:**
- **Bring Your Own Drone & Model — neurosymbolic contract** (`256a5c5`, Sept 17, 2026) — landmark feature: users can now plug in custom drone profiles (JSON) and their own decision models (LLM, RL policy, ONNX, etc.) into the swarm simulator through a well-defined interface
- **Demonstration films released** (Sept 2026) — two 1080p films showcasing the wildfire response mission (distributed air-ground coordination with no dispatcher) and unmapped sector reconnaissance (heterogeneous swarm with decentralized architecture)
- **Live online demo** — browser-based demo now live at diamants-hypervision.pages.dev, letting anyone try DIAMANTS in their browser
- **Neurosymbolic architecture refined** — model proposals are vetted by a deterministic symbolic rule layer before execution, ensuring safety guarantees even with neural network decision-makers
- **Documentation & badge polish** (`f763e46`, `7909c36`, `66286da`, `85f84d0`, Sept 16, 2026) — multiple doc and UX improvements to make the project more accessible

**Architecture Highlights:** Three-tier wildfire response (Crazyflie survey → X500/S500 inspect → Colossus suppress), stigmergy-based exploration, SLAM reconstruction, federated RL, and P2P communication tracking — all running in the browser with WebGL.

**🎙️ Potential Episode Topics:**
- "Swarm robotics in your browser: the DIAMANTS open-source drone simulator"
- "Neurosymbolic AI for drones: why your model proposes and rules dispose"
- "Wildfire response with no dispatcher: how distributed autonomy emerges"
- "Fly a swarm in your browser: the democratization of robotics simulation"
- "From stigmergy to federated learning: the math behind swarm intelligence"
- "Privacy in swarm robotics: why federated learning matters for multi-agent systems"

---

### 3. [mstfcen/flydrone-connectome](https://github.com/mstfcen/flydrone-connectome)
**⭐ 0 stars | Language: Python | License: MIT | Last updated: Sept 17, 2026**

*FlyDrone — Connectome-inspired reactive obstacle avoidance for micro-UAVs. Investigates whether compact Drosophila-inspired visuomotor motifs (from the FlyWire connectome) can provide robust reactive obstacle avoidance for micro-UAVs, validated from deterministic 2D arenas through to PX4/Gazebo SITL.*

**Recent Development Highlights:**
- **MIT license & citation metadata added** (`561c1db`, Sept 17, 2026) —正式开源 with CITATION.cff, making it easier for researchers to cite in academic papers
- **v0.2: Learned sparse connectome study** (`24d03aa`, Sept 16, 2026) — groundbreaking result: a 24-neuron learned mask matched the 377-neuron model's 83.3% success rate, with 85.0–86.7% in the 32–40 neuron sweet spot. Random masks averaged only 14.3%, proving the learned gate ranking carries task-relevant pruning information
- **PX4/Gazebo avoidance experiment finalized** (`61f0a14`, Sept 15, 2026) — completed the final experiment in the validation ladder, bridging simulation to real flight software
- **Public research presentation polished** (`0d9938a`, Sept 15, 2026) — documentation and validation status cleaned up for broader audience access
- **Hard timeout & flight-stage diagnostics** (`7aa2035`, Sept 15, 2026) — improved experimental rigor with timeout handling and per-stage diagnostics

**Headline Result:** Modified fly-inspired controller retained 100% success across all tested perturbations (clean, sensor noise + dropout, 160ms latency, gusty wind, combined), outperforming both Bilateral FlyWire and Classical VFH under stress.

**Validation Ladder:** 2D arena ✅ → Idealized 3D ✅ → 6-DoF quadcopter ✅ → PX4/Gazebo flight boundary ✅ → Gazebo x500_lidar_2d ✅ → Runtime obstacle spawn ✅ → MAVLink obstacle bridge ⚠️ → Learned connectome sparsification ✅ → Closed-loop PX4 avoidance 🚧

**🎙️ Potential Episode Topics:**
- "Nature-inspired robotics: what a fly's brain can teach us about drone obstacle avoidance"
- "Connectome computing: reverse engineering 377 neurons for autonomous flight"
- "The 24-neuron breakthrough: learned sparsification in biological-inspired controllers"
- "From simulation to reality: the Validation Ladder approach in robotics research"
- "Why failsafe matters: "
- "Open science in robotics: the FlyDrone 

---

## 📊 Quick Comparison

| Project | Stars | Language | Focus | Latest Activity |
|---------|-------|----------|-------|-----------------|
| Open AD Kit | 11 | Shell | Containerized Autoware / SOAFEE | Dual-distro pipeline, manifest CLI, R-Car X5H integration |
| DIAMANTS | 0 | JavaScript | Swarm Robotics / Neurosymbolic AI | BYO model contract, wildfire demo films, live browser demo |
| FlyDrone | 0 | Python | Connectome-inspired UAV avoidance | Learned sparse connectome, PX4/Gazebo validation, MIT license |

---

## 📋 Tracking Checklist

See the open issue **[Projects to Revisit & Upcoming Releases](https://github.com/bro26man-hash/robotics-oss-radar/issues/22)** for a detailed tracking checklist of these 3 projects.

## 🎙️ About This Project

This repo is a companion to our podcast on open-source robotics and autonomous systems. We track the most active GitHub projects, analyze their latest commits, and develop episode ideas — so listeners can follow along and contribute.

---

*Generated for the Robotics OSS Radar podcast. Stay curious, stay open-source.*
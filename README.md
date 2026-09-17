# 🤖 Robotics OSS Radar

> A living research hub tracking the most active open-source robotics & autonomous systems projects — curated for our podcast.

---

## Top 3 Most Recently Active Repos

### 1. [comma.ai/openpilot](https://github.com/commaai/openpilot) — *63,671 ⭐*
**Language:** Python | **Topic:** `robotics`  
**Tagline:** *openpilot is an operating system for robotics. Currently, it upgrades the driver assistance system on 300+ supported cars.*

#### 🔬 Latest Development Highlights (Sept 2026)
- **AGNOS 19.8** released — the latest superbike/vehicle integration stack
- **Precompiled eGPU driving model** — pushing inference to external GPUs for higher-performance setups
- **tinygrad generic ONNX compiler artifacts** — switching to a more portable, lightweight ML compiler for driving models
- **UI polish** — removing question marks, adding "not paired" bookmark alerts for better user experience

#### 🎙️ Potential Episode Topics
- On-device vs. cloud ML compilation for autonomous driving (tinygrad story)
- The "300+ supported cars" question — how does openpilot handle such fragmentation?
- eGPU licensing & the future of modular autonomous driving hardware
- AGNOS releases: what's inside the latest vehicle integration stack?

---

### 2. [ApolloAuto/apollo](https://github.com/ApolloAuto/apollo) — *26,828 ⭐*
**Language:** C++ | **Topic:** `autonomous-vehicles`  
**Tagline:** *An open autonomous driving platform.*

#### 🔬 Latest Development Highlights (Early 2026)
- **Apollo 11.0 — BEV+OCC** — the latest feature release combining Bird's-Eye-View perception with Occupancy Network predictions
- **Seyond LiDAR driver updates** — new configuration and documentation for the Seyond sensor ecosystem
- Ongoing maintenance & documentation cleanup after the Apollo 11.0 milestone

#### 🎙️ Potential Episode Topics
- Apollo 11.0's BEV+OCC architecture — how perception and prediction are merging
- The LiDAR sensor war: Apollo's support for niche players like Seyond vs. Velodyne/Ouster
- C++ vs. Python in autonomous driving stacks — Apollo's engineering choices
- Apollo's industry partnerships and the open-source vs. proprietary tension in robotaxi

---

### 3. [microsoft/AirSim](https://github.com/microsoft/AirSim) — *18,487 ⭐*
**Language:** C++ | **Topic:** `autonomous-vehicles`  
**Tagline:** *Open source simulator for autonomous vehicles built on Unreal Engine / Unity, from Microsoft AI & Research.*

#### 🔬 Latest Development Highlights (2025–2026)
- **GitHub Actions pinned to full-length commit SHAs** — improved CI security & reproducibility traceability
- **README updates & maintenance** — ongoing documentation refresh
- Unreal Engine / Unity simulator integration continues to evolve for autonomous driving research

#### 🎙️ Potential Episode Topics
- Simulation-first development: why AirSim (and its Unreal Engine roots) still matters for AV research
- The cost of simulation fidelity — Unreal vs. Unity vs. CARLA: tradeoffs for robotics teams
- CI/CD in sim: how pinning GitHub Actions to SHAs improves reproducibility
- Microsoft's commitment to open-source AV tooling — what's next for AirSim?

---

## 📊 Comparison Matrix

| Project | Stars | Language | Focus Area | Activity Level |
|---------|-------|----------|------------|---------------|
| [openpilot](https://github.com/commaai/openpilot) | 63,671 | Python | On-device ADAS | 🔥 Daily commits |
| [Apollo](https://github.com/ApolloAuto/apollo) | 26,828 | C++ | Full-stack autonomy | 📅 Bi-weekly updates |
| [AirSim](https://github.com/microsoft/AirSim) | 18,487 | C++ | Simulation & training | 📅 Monthly updates |

---

## 🎧 Podcast Episode Ideas (Bundled)

1. **"The Stack Wars"** — Comparing openpilot, Apollo, and AirSim: what each one owns and where they overlap
2. **"From Python to C++"** — Language choices in autonomous systems and why it matters
3. **"Sim or Real?"** — The role of simulation (AirSim) vs. on-vehicle deployment (openpilot/Apollo)
4. **"Hardware & the Open-Source Tension"** — Can open software keep up with proprietary sensor/hardware?
5. **"Compiling Autonomy"** — How ML compilers like tinygrad change the AV deployment landscape

---

_🔄 Last updated: September 2026 · Radar refreshed weekly_

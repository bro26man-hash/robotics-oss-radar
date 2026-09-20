# 🤖 Robotics OSS Radar

> A living research hub tracking the most active open-source robotics & autonomous systems projects — curated for the podcast

This repo is the companion to the **Robotics OSS Radar** podcast, where we deep-dive into the most compelling open-source projects shaping the future of robotics and autonomous driving. Each episode spotlights a project — what's under the hood, what's changed recently, and what it means for the field.

---

## 📡 This Week's Radar

### 1. [Isaac Lab](https://github.com/isaac-sim/IsaacLab)
**⭐ 8,170 stars | 🍴 3,904 forks | 🐍 Python | 📄 BSD-3-Clause**

NVIDIA's GPU-accelerated simulation framework for robot learning. Built on Isaac Sim, it unifies reinforcement learning, imitation learning, and motion planning with multi-physics and RTX-based sensor simulation. Supports 16+ robot models and 30+ ready-to-train environments.

**Recent Development Highlights:**
- 🔧 **CI speed-ups** for contributed environments — faster test pipelines for community submissions
- 🔄 **PyTorch bumped to 2.12** — staying current with the ML ecosystem
- 🚧 **IO descriptors deprecated** — API cleanup in preparation for the v3.0 release
- 🛠️ **Near-singular operational-space control** — numerical robustness fix for arm kinematics
- 📦 **One-removal deprecation notice** — actively pruning legacy APIs before the next major release

**🎙️ Potential Episode Topics:**
- "Sim-to-Real Transfer at Scale — How GPU Acceleration Changes Robot Training"
- "From Orbit to Isaac Lab: The Evolution of NVIDIA's Robotics Stack"
- "Reinforcement Learning in the Wild — What 30+ Ready-Made Environments Teach Us"

---

### 2. [openpilot](https://github.com/commaai/openpilot)
**⭐ 63,682 stars | 🍴 11,373 forks | 🐍 Python | 📄 MIT**

The open-source operating system for robotics — currently upgrading the driver assistance system on **300+ supported cars**. A raising-the-bar project for assisted driving, with a strong safety model (ISO 26262) and a vibrant community.

**Recent Development Highlights:**
- 📡 **Cabana: DBC file generation during builds** — automating signal database creation for car-specific integrations
- 🎨 **Signal heatmap grid refined** — improved visualization of CAN signal activity in the Cabana UI
- 💡 **Activity preservation with brighter baseline** — UI improvements for better signal readability
- 🌙 **Quiet signal brightness clamp reverted** — restoring contrast for low-activity signals in dark mode
- ✨ **Brighter quiet signals in dark mode** — further UI polish for the Cabana diagnostic tool

**🎙️ Potential Episode Topics:**
- "63,000 Stars and Counting — The Community Engine Behind openpilot"
- "Cabana and the Art of CAN Signal Visualization"
- "From 0 to 300+ Cars — How openpilot Scales Across Vehicle Platforms"
- "ISO 26262 in Practice: How openpilot Takes Safety Seriously"

---

### 3. [CARLA](https://github.com/carla-simulator/carla)
**⭐ 14,410 stars | 🍴 4,699 forks | 🛠️ C++ | 📄 MIT**

The open-source urban driving simulator built from the ground up for autonomous driving research. Used by academia and industry alike for training, validating, and benchmarking ADAS and autonomous driving stacks. Now powered by Unreal Engine 5.5.

**Recent Development Highlights:**
- ☁️ **UE5 nightly deployed to Cloudflare R2** — streamlined nightly distribution for the UE5 branch
- 🔦 **Lidar smoke helper signature fixed** — sensor rendering bug squashed
- 🚦 **Null traffic light guard in WalkerManager** — crash prevention for pedestrian scenarios
- 📡 **V2X sensor family added** — CAM service, path-loss, CustomV2X, and V2I sensors for vehicle-to-everything communication research
- 🗺️ **CARLA_MAPS_TO_COOK CMake option** — selectable packaged maps for leaner builds

**🎙️ Potential Episode Topics:**
- "Urban Simulation at Scale — What CARLA Does That Other Tools Don't"
- "V2X in simulation: The New Sensor Frontier"
- "From UE4 to UE5 — The CARLA Rendering Upgrade Journey"
- "Benchmarking Autonomous Driving: How CARLA's Leaderboard Works"

---

## 🎙️ About This Podcast

**Robotics OSS Radar** explores the open-source projects that are driving the next revolution in robotics and autonomous systems. We look at what's being built, who's building it, and what it means for the future of machines that move.

---

## 🗂️ Repo Structure

```
robotics-oss-radar/
├── README.md          ← You are here — project summaries & highlights
├── episodes/          ← Show notes per episode (TBD)
├── data/              ← Structured project tracking data (TBD)
└── charts/            ← Radar charts & visualizations (TBD)
```

## 🤝 Contributing

Found a great project we should cover? Found a bug in our tracking? Open an issue or PR — all contributions welcome!

## 📜 License

Data curated in this repo is licensed under the MIT License. Project licenses vary — check each project's own license for usage terms.

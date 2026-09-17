# 🤖 Robotics OSS Radar

> Open-source robotics & autonomous systems radar — tracking the most active projects, recent commits, and podcast episode opportunities.

This repo is a companion to the **Robotics OSS Radar** podcast — a show dedicated to the people, projects, and technologies powering the future of autonomous systems.

---

## 📡 Tracked Projects

### 1. [commaai/openpilot](https://github.com/commaai/openpilot)
**⭐ 63,671 | Language: Python | The open-source robotics operating system**

openpilot is an operating system for robotics that currently upgrades the driver assistance system on 300+ supported cars. It encompasses everything from vision-based driving models to UI/UX, vehicle interface, and model compilation pipelines.

**Recent Development Highlights (Sept 2026):**
- **AGNOS 19.8 release** — Daniel Koepping shipped the latest AGNOS (Apollo General Neighborhood Operations System) update, the on-device firmware layer that ties the model pipeline to the vehicle.
- **Precompiled eGPU driving model** — Harald Schäfer added a precompiled external GPU driving model, making deployment on edge hardware with eGPUs significantly easier and more accessible.
- **tinygrad generic ONNX compiler artifacts** — Integration with tinygrad's ONNX compiler for more flexible and efficient model artifact generation, widening the hardware support surface.
- **UI polish** — Removed stray question marks and added a "not paired" bookmark alert for improved driver-facing UX and safety feedback.

**🎙️ Potential Episode Topics:**
- "From Model to Road: How openpilot Compiles and Deploys Driving Models on Edge Hardware"
- "The AGNOS Pipeline: What Happens Between a Model Commit and a Car Update"
- "Open- versus Closed-Source ADAS: What Does the 300-Car Ecosystem Teach Us?"
- "tinygrad & ONNX: How Open-Source Model Compilers Are Reshaping Autonomous Stacks"

---

### 2. [ApolloAuto/apollo](https://github.com/ApolloAuto/apollo)
**⭐ 26,829 | Language: C++ | An open autonomous driving platform**

Apollo is Baidu's full-stack open-source autonomous driving platform, covering perception, planning, control, simulation, and cloud services. It targets L4/L5 autonomy and is widely used in research and industrial pilots across China and beyond.

**Recent Development Highlights (2026):**
- **Apollo 11.0 — BEV + OCC** — Added Bird's-Eye-View perception and Occupancy Grid prediction, a major architectural step toward end-to-end neural driving stacks. This positions Apollo alongside Tesla's occupied-space approach and Waymo's geometric perception.
- **Seyond LiDAR Driver** — Integrated support for the Seyond solid-state LiDAR, confirmed working via new configuration and documentation updates. Expands Apollo's hardware compatibility for perception pipelines.
- **Beyond LiDAR Recovery** — Merged PR #15762 to recover the "Beyond" LiDAR driver, keeping hardware support broad and ensuring legacy sensor configurations remain functional.
- **Documentation & Maintenance** — README cleanup and build status badge fixes indicate a focus on onboarding quality and community health.

**🎙️ Potential Episode Topics:**
- "BEV + OCC: How Apollo 11.0 Is Reshaping the Perception Stack"
- "LiDAR Diversity in Open-Source stacks: What Apollo Supports and Why It Matters"
- "From Apollo to Rider: The Journey of Baidu's Open-Source Autonomy"
- "Occupancy Networks in Autonomous Driving: The Trend That Links Apollo, Tesla, and Waymo"

---

### 3. [AtsushiSakai/PythonRobotics](https://github.com/AtsushiSakai/PythonRobotics)
**⭐ 30,533 | Language: Python | Python sample codes and textbook for robotics algorithms**

PythonRobotics is a widely-cited educational collection of robotics algorithms implemented in Python — covering localization, mapping, SLAM, path planning, and control. It's the go-to reference for students and practitioners learning the fundamentals of autonomous systems.

**Recent Development Highlights (Aug–Sept 2026):**
- **Dependency Maintenance** — Regular dependabot bumps for ruff, scipy, and GitHub CodeQL, keeping the project secure, modern, and reproducible. Recent bumps include ruff 0.16.x and scipy 1.18.x.
- **Stable Educational Content** — No major new algorithm additions recently, but the codebase remains a gold standard for clean, readable robotics implementations. The maintenance activity signals long-term sustainability.
- **Code Quality Tools** — Active linter and security scanning via ruff and CodeQL ensures the educational examples remain best-practice templates.

**🎙️ Potential Episode Topics:**
- "Why Python Robotics Education Still Matters in the Age of LLMs and Foundation Models"
- "From Textbook to Deployment: Bridging the Gap Between Algorithmic Learning and Real Systems"
- "The Role of Educational Open-Source in Building the Robotics Workforce"
- "AETS, RSL, and the Chronopolitans: Counter-Path Planning and Decision-Making in Deep Mode"

---

## 🎙️ About the Podcast

**Robotics OSS Radio** explores the open-source projects that are making autonomous systems real — from perception and planning to deployment and UX. Each episode dives into a tracked project, interviews maintainers, and discusses where the field is headed next.

---

## 📊 Quick Comparison

| Project | Stars | Language | Focus | Latest Activity |
|---|---|---|---|---|
| commaai/openpilot | 63.6K | Python | ADAS / Autonomous Driving OS | Daily — model compilation, UI, firmware |
| ApolloAuto/apollo | 26.8K | C++ | Full-stack Autonomous Driving | Monthly — BEV+OCC, LiDAR drivers |
| PythonRobotics | 30.5K | Python | Educational Algorithms | Ongoing — dependency maintenance |

---

## 📋 Tracking Checklist

See the open issue **[Projects to Revisit & Upcoming Releases](https://github.com/bro26man-hash/robotics-oss-radar/issues)** for a detailed tracking checklist of all 3 projects, review dates, and episode outreach status.

## 🤝 Contributing

Have a project you think we should track? Found a major release or PR worth highlighting? Open an issue or submit a PR — this radar is community-driven!

## 📜 License

MIT — use it, remix it, track your own radar.
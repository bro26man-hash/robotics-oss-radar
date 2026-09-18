# 🤖 Robotics OSS Radar

> Tracking the most active open-source robotics & autonomous vehicle projects — for our podcast.

## 📡 Top 3 Projects Under the Lens

---

### 1. [commaai/openpilot](https://github.com/commaai/openpilot)
**⭐ 63,675 stars | Language: Python | License: GPLv3 | Last updated: Sept 17, 2026**

*openpilot is an operating system for robotics. Currently, it upgrades the driver assistance system on 300+ supported cars — turning every commodity sensor setup into an advanced driver-assistance system (ADAS).*

**Recent Development Highlights:**
- **Model chunking removed & LFS adopted for Chestnut releases** (`1328ace`, Sep 17, 2026, PR #38941) — by Harald Schäfer; streamlines model storage and release management using Git LFS, making CI faster and more reliable
- **Chestnut power test removed** (`7db7735`, Sep 17, 2026, PR #38943) — by Daniel Koepping; cleanup of deprecated power testing infrastructure for the new Chestnut hardware generation
- **modeld: 2× faster Chestnut build** (`cd1490a`, Sep 17, 2026, PR #38656) — by Adeeb Shihadeh; major performance optimization cutting model compilation time in half for the upcoming Chestnut release
- **UI: question marks removed** (`bd176cb`, Sep 17, 2026, PR #38938) — by Shane Smiskol; UI polish removing ambiguous placeholder icons
- **UI: not-paired bookmark alert** (`4d9d1bc`, Sep 17, 2026, PR #38936) — by stef; new user-facing alert when a phone isn't paired, improving onboarding experience

**Key Architecture:** modeld (deep learning model runner), managerc (process manager), controls (actuator & state management), ui (React Native dashboard), boardd (CAN bus interface), panda (hardware security & CAN bridge), Chestnut hardware support, RAML-based release pipeline.

**🎙️ Potential Episode Topics:**
- "63K stars and 300+ cars: inside commaai's openpilot"
- "Chestnut is coming: 2× faster builds and LFS-based releases"
- "Why modeld matters: how openpilot runs neural nets on the edge"
- "panda and boardd: the hardware backbone of open-source ADAS"
- "From comma one to commodity hardware: the openpilot hardware saga"
- "UI polish as a feature: how small UX fixes move open-source forward"

---

### 2. [NVIDIA/cosmos](https://github.com/NVIDIA/cosmos)
**⭐ 11,843 stars | Language: Jupyter Notebook | License: Apache-2.0 | Last updated: Sept 17, 2026**

*NVIDIA Cosmos is an open platform of world models, datasets, and tools that enables developers to build Physical AI for robots, autonomous vehicles, and synthetic data pipelines — from text-to-video world generation to certifiable NIM deployment.*

**Recent Development Highlights:**
- **Cosmos3-Super distilled examples fixed for vllm-omni** (`b0e54e8`, Sep 14, 2026, PR #350) — by MaciejBalaNV; bug fix ensuring distilled checkpoint examples work correctly with the vLLM-OMNI inference server, unblocking researchers using quantized models
- **Cookbook: reasoner user guide for sglang added** (`5a68d9d`, Sep 12, 2026, PR #322) — by Kedi Wu; comprehensive documentation for serving Cosmos world models with SGLang, lowering the barrier to production deployment
- **Cookbook (action): RoboCasa mobile-manipulation post-training recipe** (`a9aa3bc`, Sep 10, 2026, PR #318) — by hyzhou-nv; new actionable recipe for post-training robots in mobile manipulation tasks using Cosmos simulation
- **Docs: issue templates & security policy added** (`c92f947`, Sep 10, 2026, PR #348) — by Rickz; professional open-source governance improvements
- **Cookbooks: Cosmos3 Certified NIM added to environment setup guide** (`18d0542`, Sep 4, 2026, PR #345) — by Rickz; streamlined path from research to certified NVIDIA NIM deployment

**Key Architecture:** Cosmos World Foundation Models (text-to-video, image-to-video), Cosmos Transfer (real-to-synthetic domain transfer), Cosmos Predict (video prediction), SGLang & vLLM-OMNI serving, Certified NIM containers, RoboCasa integration, Cookbook recipes.

**🎙️ Potential Episode Topics:**
- "NVIDIA Cosmos: world models that generate reality for AI training"
- "From text to video: how Cosmos world models train robots"
- "Cosmos3-Super distilled: running world models on a single GPU"
- "RoboCasa + Cosmos: the path from simulation to real-world manipulation"
- "Certified NIM: how NVIDIA ships world models to production"
- "SGLang vs vLLM-OMNI: serving world models at scale"

---

### 3. [NVlabs/alpasim](https://github.com/NVlabs/alpasim)
**⭐ 1,238 stars | Language: Python | License: Apache-2.0 | Last updated: Sept 17, 2026**

*AlpaSim is an open-source autonomous vehicle simulation platform designed for development and testing of end-to-end AV policies — built for reproducibility, high-fidelity sensor simulation, and seamless integration with the Apollo planning stack.*

**Recent Development Highlights:**
- **CI: avoid LFS downloads while replaying GitHub changes to GitLab** (`affc2ea`, Aug 18, 2026, PR #154) — by jarcherNV; CI pipeline optimization that avoids heavy Git LFS downloads during cross-platform sync, cutting build times significantly
- **Runtime: rollout seeds selectable & reproducible via RolloutSpec** (`9a3832b`, Aug 17, 2026, PR #149) — by Alba María Téllez Fernández; major reproducibility improvement letting researchers pin random seeds for exact scenario replay — critical for scientific rigor
- **Controller: linear MPC speed bound increased to 40 m/s** (`1e801ca`, Aug 12, 2026, PR #144) — by Ding-ray; MPC controller now supports speeds up to 144 km/h, enabling highway-speed scenario testing
- **GitLab sync (2026-08-11)** (`6870924`, Aug 11, 2026, PR #145) — by mwatson-nvidia; regular cross-platform repository synchronization
- **Fix uv install in self-hosted build jobs** (`0d0f522`, Aug 11, 2026, PR #146) — by jarcherNV; build infrastructure fix for self-hosted runners

**Key Architecture:** RolloutSpec (reproducible scenario specification), Linear MPC controller (with 40 m/s speed support), Sensor simulation (camera, LiDAR, radar), Apollo planning integration, GitLab↔GitHub sync pipeline, uv-based Python environment management.

**🎙️ Potential Episode Topics:**
- "AlpaSim: the simulator built for end-to-end AV policy testing"
- "Reproducibility is everything: why rollout seeds matter in AV research"
- "From 0 to 40 m/s: how AlpaSim is pushing highway-speed simulation"
- "GitLab meets GitHub: the cross-platform CI challenge in open-source AV"
- "AlpaSim + Apollo: a full-stack simulation-to-planning pipeline"
- "uv, LFS, and CI pain: the infrastructure story behind AV simulators"

---

## 📊 Quick Comparison

| Project | Stars | Language | Focus | Latest Activity |
|---------|-------|----------|-------|-----------------|
| openpilot | 63,675 | Python | Open-source ADAS OS for 300+ cars | Chestnut build optimization, LFS migration, UI fixes |
| NVIDIA Cosmos | 11,843 | Jupyter | World models & Physical AI platform | Distilled model fixes, SGLang guide, RoboCasa recipes |
| AlpaSim | 1,238 | Python | End-to-end AV simulation platform | Reproducible rollouts, 40 m/s MPC, CI optimization |

---

## 📋 Tracking Checklist

See the open issue **[Projects to Revisit & Upcoming Releases](https://github.com/bro26man-hash/robotics-oss-radar/issues/31)** for a detailed tracking checklist of these 3 projects.

## 🎙️ About This Project

This repo is a companion to our podcast on open-source robotics and autonomous systems. We track the most active GitHub projects, analyze their latest commits, and develop episode ideas — so listeners can follow along and contribute.

---

*Generated for the Robotics OSS Radar podcast. Stay curious, stay open-source.*
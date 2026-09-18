# 🤖 Robotics OSS Radar

> Tracking the most active open-source robotics & autonomous vehicle projects — for our podcast.

## 📡 Top 3 Projects Under the Lens

---

### 1. [carla-simulator/carla](https://github.com/carla-simulator/carla)
**⭐ 14,405 stars | Language: C++ | License: MIT | Last updated: Sept 2026**

*CARLA is an open-source simulator for autonomous driving research. It provides a flexible, reliable, and realistic environment for development, training, and validation of autonomous driving systems — with support for sensors, traffic, and weather conditions.*

**Recent Development Highlights:**
- **Deploy UE5 nightly to Cloudflare R2** (`1360bb9`, Sep 2, 2026, PR #9859) — by germanros1987; UE5 simulator builds now deployed to Cloudflare R2 for faster global distribution, reducing download times for researchers worldwide
- **Fix lidar smoke helper signature** (`0a5ce0d`, Jul 14, 2026, PR #9791) — by Yin Li; bug fix ensuring LiDAR sensor helpers receive correct signatures, improving sensor simulation accuracy
- **Guard against null traffic light in WalkerManager** (`39c4fda`, Jul 14, 2026, PR #9758) — by Jesus Armando Anaya; critical null-safety fix in pedestrian traffic light logic, preventing crashes in WalkerManager scenarios

**Key Architecture:** UE5-based rendering, ROS/ROS2 bridge, sensor suite (LiDAR, camera, radar, IMU), traffic manager, WalkerManager for pedestrians, Cloudflare R2 deployment pipeline, Python & C++ API.

**🎙️ Potential Episode Topics:**
- "14k stars and a UE5 engine: inside the CARLA driving simulator"
- "From local to Cloudflare R2: how CARLA ships nightly builds globally"
- "NullTrafficLight and LiDAR fixes: the bugs that matter in AV simulation"
- "ROS bridge deep dive: connecting CARLA to the robot ecosystem"
- "WalkerManager: simulating pedestrians for safer autonomous driving"
- "Why simulators are the secret weapon of AV research"

---

### 2. [autowarefoundation/autoware](https://github.com/autowarefoundation/autoware)
**⭐ 12,067 stars | Language: Dockerfile | License: Apache-2.0 | Last updated: Sept 2026**

*Autoware is the world's leading open-source software project for autonomous driving. It provides a complete stack from perception and planning to control, running on ROS 2 — backed by the Autoware Foundation and a global community of contributors.*

**Recent Development Highlights:**
- **Update managed_transform_buffer to 0.3.0** (`a45f9ba`, Sep 16, 2026, PR #7316) — by awf-autoware-bot; dependency bump for transform buffer library, improving coordinate-frame management across the autonomy stack
- **Add CARLA 0.10 Town10HD_Opt map to demo artifacts** (`79446c0`, Sep 9, 2026, PR #7308) — by Masaya Kataoka; new high-definition map integration for demos, enabling more realistic urban scenario testing
- **Fix Docker build for simple planning simulator with core** (`87f7b60`, Sep 8, 2026, PR #7311) — by Mete Fatih Cırıt; Docker build fix unblocking the planning simulator toolchain, critical for CI/CD and developer onboarding

**Key Architecture:** ROS 2-based perception (lidar, camera fusion), planning & decision-making, vehicle control adapters, Autoware.launch badging system, managed_transform_buffer for coordinate management, Docker-based deployment, CARLA integration for simulation.

**🎙️ Potential Episode Topics:**
- "12k stars and the Autoware Foundation: how open-source builds an AV stack"
- "From ROS 2 to Docker: how Autoware ships to production"
- "Town10HD_Opt: HD maps meet simulation in Autoware demos"
- "Transform buffers and coordinate frames: the hidden complexity of AV stacks"
- "The Autoware Foundation: governance, community, and the road ahead"
- "Planning simulator Docker fixes: why CI matters for autonomous driving"

---

### 3. [strands-labs/robots](https://github.com/strands-labs/robots)
**⭐ 159 stars | Language: Python | License: Apache-2.0 | Last updated: Sept 2026**

*Strands Robots enables controlling physical robots and hardware with natural language through Strands Agents. It bridges LLM-based reasoning with real-world robot manipulation, making it possible to command robots conversationally.*

**Recent Development Highlights:**
- **Fix image_keys scoping for camera resize in async policies** (`c684449`, Sep 17, 2026, PR #3849) — by ./c²; critical fix ensuring image_keys properly scopes which cameras the server resizes, preventing incorrect image feeds in multi-camera setups
- **Fix humanoid head camera mount documentation for Unitree G1** (`2eb1576`, Sep 17, 2026, PR #3848) — by ship; documentation correction for the head camera mount on the torso_link of Unitree G1 humanoid, improving hardware setup accuracy
- **Refactor: path sandbox lives below every layer that writes a file** (`11f9c0f`, Sep 17, 2026, PR #3847) — by ./c²; core architectural refactor isolating file-write paths into a sandbox layer, improving security and separation of concerns in policy execution

**Key Architecture:** Strands Agents (LLM-based task planning), natural-language robot command interface, async policy execution with camera scoping, path sandbox for secure file operations, Unitree G1 humanoid support, ROS 2 integration.

**🎙️ Potential Episode Topics:**
- "159 stars, huge ambition: commanding robots with natural language"
- "The path sandbox refactor: security architecture for robot policy execution"
- "Camera scoping bugs and humanoid docs: the small fixes that save big experiments"
- "From LLM to actuator: how Strands bridges language and motion"
- "Unitree G1 meets Strands: a humanoid robot you can talk to"
- "Async policies and multi-camera setups: the hard parts of LLM robot control"

---

## 📊 Quick Comparison

| Project | Stars | Language | Focus | Latest Activity |
|---------|-------|----------|-------|-----------------|
| CARLA | 14,405 | C++ | Autonomous driving simulator (UE5) | UE5 nightly R2 deployment, LiDAR fixes, WalkerManager null-safety |
| Autoware | 12,067 | Dockerfile | Full open-source AV stack on ROS 2 | Dependency bumps, HD map integration, Docker build fixes |
| Strands Robots | 159 | Python | Natural-language robot control via LLMs | Camera scoping fixes, path sandbox refactor, hardware docs |

---

## 📋 Tracking Checklist

See the open issue **[Projects to Revisit & Upcoming Releases](#)** for a detailed tracking checklist of these 3 projects.

## 🎙️ About This Project

This repo is a companion to our podcast on open-source robotics and autonomous systems. We track the most active GitHub projects, analyze their latest commits, and develop episode ideas — so listeners can follow along and contribute.

---

*Generated for the Robotics OSS Radar podcast. Stay curious, stay open-source.*
# 🤖 Robotics OSS Radar

**Tracking the most active open-source robotics & autonomous vehicle repos on GitHub — with recent commits, development highlights, and podcast episode ideas.**

*Last updated: September 2026*

---

## 🔭 Tracked Projects

### 1. NVIDIA Elements — `NVIDIA/elements` ⭐ 85 | 🟢 TypeScript

> **NVIDIA Design System and UI Agent Harness for AI/ML Factories, Robotics, and Autonomous Vehicles**

**What it is:** NVIDIA's unified design system and UI component library purpose-built for robotics, autonomous vehicle tooling, and AI/ML infrastructure dashboards. Framework-agnostic Web Components that work across React, Angular, Vue, Svelte, and Lit.

**Recent Development Highlights:**
- **v2.7.3 released** (Sep 3, 2026) — semantic-release automated the latest version bump
- **CI dependency updates** — Chore commit keeping the monorepo build pipeline current
- **Core icon fixes** — Aspect ratio corrections in the core UI component library
- Active agent-ready tooling: CLI + MCP (Model Context Protocol) expose component APIs, tokens, and validation to AI assistants

**Why it matters for your podcast:** NVIDIA is the heavyweight in autonomous vehicle hardware, and now they're building the *software interface layer* — design systems and agent harnesses that make it possible for AV operators and robotics engineers to interact with AI infrastructure through consistent, toolable UIs. This is the bridge between raw autonomy stacks and the human-in-the-loop dashboards that operators actually use.

**🎙️ Episode Topic Ideas:**
- "How NVIDIA is building the UI layer for autonomous vehicle fleets"
- "Web Components for robotics: framework-agnostic UI in a polyglot world"
- "Agent-ready design systems: when your UI needs to be machine-readable too"

---

### 2. Flight Core — `mingley/flight-core`

> **Strongly typed Rust SDK for autonomous vehicle control: typestate APIs, units/frames, PX4 SITL, deterministic sim/replay, and verified state machines**

**What it is:** A groundbreaking Rust control boundary for autonomous vehicles that makes physically invalid or unsafe control software *impossible to express*. Uses typestate patterns, revocable actuation permits, typed units/frames, and formal verification (Kani, Creusot) to prove safety invariants at compile time.

**Recent Development Highlights:**
- **Agent-executable civilization plan** (Sep 3, 2026) — New commit adding the control-boundary end-state spec for agentic autonomy systems
- **Takeoff state machine fixes** — Leftover state handling refined: Takeoff can no longer declare airborne after revoke; climb-complete after revoke is properly refused
- **Active Kani verification pipeline** — 45 proof harnesses running in CI covering actuators, drive, thrust, contact, drag, buoyancy, HITL miss, position-hold restore, and permit epoch invariants
- **Creusot 0.5.0 integration** — 81 libraries discharged via formal verification for discrete machine contracts
- PX4 SITL, ArduPilot GUIDED, ROS 2 Jazzy, and HITL rack backends all actively maintained
- New scenario workloads: GPS-loss, heartbeat-stale, hitl-miss, imu-loss, revoke-table, motor-efficiency, imu-delay

**Why it matters for your podcast:** This is the bleeding edge of *verified autonomy*. While most robotics codebases rely on conventions and runtime checks, flight-core puts physical safety invariants into the type system itself. If a drone isn't armed, the code literally won't compile to send motor commands. This is the kind of work that could redefine safety standards for autonomous vehicles.

**🎙️ Episode Topic Ideas:**
- "What if your drone firmware had a type error? Compile-time safety for autonomous vehicles"
- "Kani and Creusot: formal verification meets robotics control"
- "Typestate machines in Rust: the future of safe autonomy?"
- "From PX4 SITL to verified world simulation: the new testing paradigm"

---

### 3. MOOS-IvP CC — `HeroCC/moos-ivp-cc` ⭐ 16 | ⚫ C++

> **A collection of MOOS-IvP tools and utilities used in MIT 2.680, Aquaticus, and containerized missions**

**What it is:** Community-maintained extensions and utilities for the MOOS-IvP autonomy framework, heavily used in MIT's autonomous marine vehicles course (2.680) and the Aquaticus underwater robotics project. Docker-first deployment with pre-built images on DockerHub.

**Recent Development Highlights:**
- **Docker image updated** (Sep 4, 2026) — Latest container build with current dependencies
- **Home directory discovery fixed** (Jul 29, 2026) — Resolve MOOS-IvP path detection in containerized environments
- **macOS socket bind fix** (Jul 29, 2026) — Socket resolution corrected for macOS deployment
- Active mission packs for MIT 2.680 coursework and custom aquatic missions

**Why it matters for your podcast:** MOOS-IvP is one of the oldest and most battle-tested marine autonomy frameworks in the world. It powers real ocean-going AUVs and is the backbone of MIT's hands-on autonomy curriculum. The ongoing Docker modernization and cross-platform fixes show a project that's bridging 20+ years of legacy C++ robotics with modern containerized deployment workflows.

**🎙️ Episode Topic Ideas:**
- "MOOS-IvP at 20: how MIT teaches autonomous ocean robots"
- "From Docker containers to ocean-going AUVs: modernizing legacy robotics frameworks"
- "The Aquaticus project and the future of underwater autonomy"

---

## 📋 Quick Stats

| Project | Language | Stars | Last Active | Focus Area |
|---------|----------|-------|-------------|------------|
| NVIDIA Elements | TypeScript | 85 | Sep 4, 2026 | AV UI / Agent Harness |
| Flight Core | Rust | 0 | Sep 4, 2026 | Verified AV Control |
| MOOS-IvP CC | C++ | 16 | Sep 4, 2026 | Marine Autonomy |

---

## 🎙️ About This Radar

This repository is curated for the **Robotics OSS Podcast** — a show exploring the people, tools, and ideas shaping open-source robotics and autonomous systems. Every tracked project represents a different facet of the autonomy ecosystem: from the UI layer that operators touch, to the formally-verified control plane that keeps vehicles safe, to the decades-old frameworks still powering real ocean missions.

*Want to suggest a project for the radar? Open an issue!*
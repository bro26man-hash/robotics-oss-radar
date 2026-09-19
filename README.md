# 🤖 Robotics OSS Radar

> **Podcast companion for open-source robotics & autonomous systems**
> Tracking the most active GitHub projects, recent development highlights, and episode opportunities.

---

## 📡 What Is This?

**Robotics OSS Radar** is a podcast companion that monitors the most recently active open-source repositories in the robotics and autonomous-vehicles ecosystem. We track recent commits, highlight development trends, and generate episode ideas — so you never miss a story worth telling.

---

## 🔍 Current Radar: Top 3 Recently Active Projects

---

### 1. 🏭 sim-foundry — Virtual Industrial Simulation for Robotics & IoT Testing

| Field | Detail |
|-------|--------|
| **Repo** | [`wailhoud/sim-foundry`](https://github.com/wailhoud/sim-foundry) |
| **Tag** | `autonomous-vehicles` (industrial automation) |
| **Language** | Python |
| **License** | MIT |
| **Latest Commit** | `24a4b81` — *Update README.md* — **Sep 19, 2026** |

**What it does:** sim-foundry creates a **complete virtual industrial environment** on your computer — simulating PLCs, cameras, sensors, robotic arms, conveyor belts, and more. It lets developers test HMI, SCADA, IoT gateway, and data-collection software without waiting for physical hardware to ship. Think of it as a "factory in a box."

#### 📊 Recent Commit Activity

| Date | SHA | Change | Why It Matters |
|------|-----|--------|-----------------|
| Sep 19, 2026 | `24a4b81` | README refreshed | Documentation keeps pace with feature growth |
| Sep 18, 2026 | `88a953b` | Initial commit | Project bootstrapped |
| Sep 17, 2026 | `87005ae` | Init commit | Early scaffolding |

#### 🔑 Key Architecture Highlights
- **Device Library:** 100+ virtual industrial components (PLC brands, cameras, temperature/humidity/pressure sensors, robotic arms, packaging machines)
- **Multi-Protocol Support:** Modbus, OPC-UA, MQTT, EtherCAT — connects to any modern industrial stack
- **Integration-Ready:** Works with SCADA, HMI, gateways, cloud platforms, MES, and data historians
- **Custom Device Profiles:** Advanced users can define new virtual devices via JavaScript
- **Docker / K8s Native:** Multiple `docker-compose` configs, Helm charts, and migration scripts for cloud deployments
- **Grafana Dashboards:** Pre-built monitoring dashboards for live telemetry visualization

#### 🎙️ Potential Episode Topics
- "Testing Your Robot Without a Robot: Inside sim-foundry's Virtual Factory"
- "Why Hardware Delays Kill Robotics Startups (and How to Simulate First)"
- "From PLC to Cloud: How sim-foundry Bridges OT and IT"
- "Digital Twins for Everyone: Industrial Simulation Goes Open-Source"
- "Modbus, OPC-UA, MQTT — Protocol Wars in the Factory of the Future"

---

### 2. 🌐 Air-Lingjing — Open Simulation Stack for LLM-Driven Embodied Agents

| Field | Detail |
|-------|--------|
| **Repo** | [`glenuptoherneck646/Air-Lingjing`](https://github.com/glenuptoherneck646/Air-Lingjing) |
| **Tag** | `autonomous-vehicles` (embodied AI) |
| **Language** | Python |
| **License** | Not specified |
| **Latest Commit** | `5cdc1ea` — *Update README.md* — **Sep 19, 2026** |

**What it does:** Air-Lingjing is an **open simulation stack** that connects LLM-driven AI agents to large 3D environments built in Unreal Engine. It enables **multi-agent orchestration** — multiple virtual characters, robots, or digital assistants can share a space, coordinate tasks, communicate, and react to each other and their surroundings in real time. It's essentially a brain for virtual worlds.

#### 📊 Recent Commit Activity

| Date | SHA | Change | Why It Matters |
|------|-----|--------|-----------------|
| Sep 19, 2026 | `5cdc1ea` | README updated | Docs refreshed after plugin work |
| Aug 20, 2026 | `cb8ede7` | **Unreal plugin integration updated** | Core feature development — improving the Unreal Engine bridge |
| Aug 20, 2026 | `a224cc3` | Unreal plugin integration updated (second pass) | Iterative refinement of the Unreal plugin — signals active dev |

#### 🔑 Key Architecture Highlights
- **Multi-Agent Orchestration:** Coordinates multiple AI agents simultaneously — they share information, plan tasks, and cooperate
- **Seamless Unreal Engine Integration:** Purpose-built for UE — stunning visuals + realistic physics
- **Real-Time Performance:** Optimized for live processing; agents react instantly to environmental changes
- **Flexible & Extensible:** Customizable agent behavior, new capabilities, and external tool connections
- **Embodied Intelligence Focus:** Designed for research in group behavior, intelligent NPCs, and industrial workflow simulation

#### 🎙️ Potential Episode Topics
- "Giving Virtual Worlds a Brain: Inside Air-Lingjing's Multi-Agent Engine"
- "LLMs Meet Unreal Engine: What Happens When AI Agents Inhabit 3D Worlds"
- "From Game NPCs to Warehouse Robots: The Shared Tech Stack"
- "Multi-Agent Coordination: How AI Entities Learn to Cooperate (or Compete)"
- "Embodied AI Goes Open-Source: Air-Lingjing's Ambition"

---

### 3. 🔧 robopartpicker — Open Robotics Project Discovery, BOM Compilation & Parts Sourcing

| Field | Detail |
|-------|--------|
| **Repo** | [`brainbook0/robopartpicker`](https://github.com/brainbook0/robopartpicker) |
| **Tag** | `robotics` |
| **Language** | TypeScript (React + Cloudflare Workers) |
| **License** | Not specified (source published for transparency) |
| **Latest Commit** | `732febd` — *Link project pages to their related projects in the crawler view* — **Sep 19, 2026** |

**What it does:** RoboPartPicker is the **PCPartPicker of robotics** — it discovers open-source robotics projects, compiles their bills of materials (BOMs) from the project's own artifacts (CSV, URDF, KiCad, Markdown, JSON, etc.), normalizes component identities, and shows real pricing with sourcing estimates. It currently indexes **2,445 robotics projects, 34,760 components, and 1,653 normalized BOM lines**. Every BOM line keeps its evidence source — unresolved items are never silently guessed.

#### 📊 Recent Commit Activity (All on Sep 19!)

| Date | SHA | Change | Why It Matters |
|------|-----|--------|-----------------|
| Sep 19, 2026 | `732febd` | **Crawler view now links related projects** | Knowledge graph enhances — users can discover connected designs |
| Sep 19, 2026 | `4e71d6f` | Complete favicon set for search visibility | SEO polish — the site is maturing as a public platform |
| Sep 19, 2026 | `f2ae3cf` | Server-render component specs & files on part pages | Performance + SEO — parts pages now render on the server |

#### 🔑 Key Architecture Highlights
- **Evidence-First BOMs:** Every BOM line keeps a source locator (file path, section, URDF element) — nothing is guessed
- **Canonical Component Normalization:** Aggregates only on exact manufacturer + part-number matches
- **Public HTTP API + MCP Server:** Robots can query the catalog directly — `search_projects`, `get_project`, `search_components`, `compare_components`, `validate_rpcs`
- **MCP Registered:** Published to the official Model Context Protocol registry as `com.robopartpicker/robopartpicker`
- **Data Honesty:** Observed prices are labeled as observations, not quotes; unresolved lines stay visible; no synthetic activity
- **RPPS Draft Standard:** Vendor-neutral robotics parts data standard (0.1) published in-repo
- **677 Unit Tests + 72 Integration Tests:** CI-enforced quality with `npm run check`

#### 🎙️ Potential Episode Topics
- "PCPartPicker for Robots: How robopartpicker Turned BOMs into a Public Good"
- "Can a Bot Source Your Next Build? Inside the MCP-Powered Parts Catalog"
- "2,445 Open Robotics Projects — What Did We Learn? (Data Deep-Dive)"
- "Evidence Over Guesswork: Why Robotics BOMs Must Stay Honest"
- "From URDF to Shopping Cart: The Pipeline That Turns Designs into Build Plans"
- "RPPS: A Vendor-Neutral Standard for Robotics Parts Data — Is It Sticking?"

---

## 📊 Radar Summary

| # | Project | Domain | Stars | Commit Cadence | Vibe |
|---|---------|--------|-------|-----------------|------|
| 1 | **sim-foundry** | Industrial Simulation / IoT | New (MIT) | Active (3 commits in 3 days) | 🏭 Factory floor virtualization |
| 2 | **Air-Lingjing** | Embodied AI / 3D Simulation | New | Active (Unreal plugin dev) | 🌐 Virtual worlds with AI brains |
| 3 | **robopartpicker** | Robotics Discovery / BOM Sourcing | New | Active (3 commits in 1 day) | 🔧 PCPartPicker for robots |

---

## 🎙️ Episode Pipeline

| Priority | Project | Suggested Angle | Status |
|----------|---------|-------------------|--------|
| 🔴 **High** | sim-foundry | Industrial simulation — testing robots without hardware | In progress |
| 🟡 **Medium** | Air-Lingjing | Embodied AI — LLM agents in 3D worlds | TBD |
| 🟡 **Medium** | robopartpicker | Robotics discovery & sourcing — turning designs into build plans | TBD |

---

## 📋 How to Contribute

This is a **living document**. To suggest a project or submit an episode idea:

1. Fork this repo
2. Add your candidate to the radar (follow the format above)
3. Open a PR with your suggestions
4. Or open an **Issue** with the `episode-suggestion` label

---

## 🔗 Useful Links

- [sim-foundry](https://github.com/wailhoud/sim-foundry) — Virtual industrial simulation
- [Air-Lingjing](https://github.com/glenuptoherneck646/Air-Lingjing) — LLM-driven 3D agent simulation
- [robopartpicker.com](https://robopartpicker.com) — Live robotics parts catalog & BOM tool
- [robopartpicker MCP](https://registry.modelcontextprotocol.io/v0/servers?search=com.robopartpicker) — Model Context Protocol server

---

*Built for the open-source robotics community. Licensed under MIT.*
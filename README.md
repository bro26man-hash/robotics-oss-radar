# 🤖 Robotics OSS Radar

> Tracking the most active open-source robotics & autonomous-systems projects — with development highlights and podcast episode ideas.

---

## 📡 Projects Under the Lens

### 1. [Air-Lingjing](https://github.com/glenuptoherneck646/Air-Lingjing)
**Tag:** `autonomous-vehicles` · **Language:** Python · **Stars:** 0

**What it is:** An open simulation stack for LLM-driven embodied agents in large 3D environments. Air-Lingjing bridges AI to realistic Unreal Engine scenes, letting multiple intelligent agents coordinate tasks, communicate, and react to their surroundings in real time.

**Recent development highlights:**
- 🗓️ **Sep 19, 2026** — README overhaul (5cdc1ea): major documentation refresh covering system requirements, performance tiers, and usage guides.
- 🗓️ **Aug 20, 2026** — Unreal plugin integration updated (cb8ede7, a224cc3): two commits in one day signalling active iteration on the Unreal Engine bridge.

**🎙️ Potential episode topics:**
- *"LLMs Meet Simulated Worlds"* — How large language models are being orchestrated as multi-agent systems inside virtual environments.
- *"Building a Digital Twin for Free"* — Walkthrough of Air-Lingjing's free simulation stack and how researchers can use it for embodied-AI experiments.
- *"Unreal Engine as a Robotics Testbed"* — Why game engines are becoming the go-to simulator for autonomous-system training.

---

### 2. [RoboPartPicker](https://github.com/brainbook0/robopartpicker)
**Tag:** `robotics` · **Language:** TypeScript · **Stars:** 0

**What it is:** Open robotics project discovery, bill-of-materials compilation, and parts sourcing — think PCPartPicker for robot builds. It currently indexes **2,445 published robotics projects**, **34,760 components**, and **1,653 normalized BOM lines** across open hardware, robotics software, and manufacturer showcases.

**Recent development highlights:**
- 🗓️ **Sep 19, 2026** — Linked project pages to related projects in the crawler view (732febd): improves discovery by connecting designs that share components or design patterns.
- 🗓️ **Sep 19, 2026** — Complete favicon set deployed (4e71d6f): brand polish for search & browser tabs.
- 🗓️ **Sep 19, 2026** — Server-rendered component specs & files on part pages (f2ae3cf): faster loads and better SEO for the 34k+ component catalog.

**🎙️ Potential episode topics:**
- *"PCPartPicker for Robots"* — How RoboPartPicker is solving the "where do I even start?" problem for open-source robot builds.
- *"The Honesty Gap in Robotics Catalogs"* — Why showing unresolved BOM lines and partial prices is more useful than fake certainty.
- *"MCP Servers for Robotics"* — How RoboPartPicker's Model Context Protocol server lets AI agents query real robotics data.

---

### 3. [Navigraph — Scenario Sketchpad](https://github.com/DuvanCardenas/scenario-sketchpad)
**Tag:** `autonomous-vehicles` · **Language:** HTML · **Stars:** 1

**What it is:** An AI whiteboard for 2026 autonomous driving design. Navigraph is a visual orchestration platform for designing, simulating, and validating complex operational scenarios for self-driving cars, robotic fleets, and intelligent systems. Exports to OpenSCENARIO, ROS 2 world files, and CARLA JSON.

**Recent development highlights:**
- 🗓️ **Sep 19, 2026** — Format update (58080d1): ongoing refinement of the scenario file format via automated CI (third automated commit in quick succession).
- 🗓️ **Sep 19, 2026** — Merge & decrypt automation (087b53f): CI-driven merge and encryption workflows, suggesting active work on secure collaborative editing.
- 🗓️ **Sep 19, 2026** — Hotfix notify (2d94385): push notification infrastructure for real-time collaboration alerts.

**🎙️ Potential episode topics:**
- *"Visual Scenario Design for Self-Driving Cars"* — How tools like Navigraph are turning edge-case scenario planning into an interactive, collaborative canvas.
- *"From Whiteboard to CARLA"* — The pipeline from hand-drawn scenarios to simulation-ready OpenSCENARIO and ROS 2 files.
- *"AI as a Co-Pilot for Safety Analysis"* — Using GPT-4 and Claude to review scenario graphs for logical paradoxes and edge cases before deployment.

---

## 🎙️ About This Radar

This repo is the companion data source for the **Robotics OSS Radar** podcast — a show exploring the open-source projects shaping the future of autonomous systems and robotics. Each episode dives deep into one project, interviewing maintainers, walking through the code, and discussing what's coming next.

**Suggested episode cadence:**
| Week | Project | Theme |
|------|---------|-------|
| 1 | Air-Lingjing | LLMs Meet Simulated Worlds |
| 2 | RoboPartPicker | The Hardware Discovery Layer |
| 3 | Navigraph | Visual Scenario Design for AVs |

---

## 🔧 How to Contribute

- Found a stale project? Open an issue with the repo URL and what you expected to see.
- Want your project featured? Submit a link and a 2-line description.
- Episode ideas? The issue tracker is the place.

---

## 📊 Radar Dashboard

| Project | Last Push | Activity | Stars | Language |
|---------|-----------|----------|-------|----------|
| Air-Lingjing | Sep 19, 2026 | 🟢 Active (README refresh + Unreal plugin) | 0 | Python |
| RoboPartPicker | Sep 19, 2026 | 🟢 Active (crawler + favicon + SSR) | 0 | TypeScript |
| Navigraph | Sep 19, 2026 | 🟢 Active (CI automation + hotfixes) | 1 | HTML |

---

*Built with 💡 and a lot of open-source love.*

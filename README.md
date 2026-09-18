# 📡 Robotics OSS Radar

> Tracking the most active open-source robotics & autonomous-vehicle projects. Weekly progress snapshots, development highlights, and podcast episode ideas.

---

## 🔍 Why This Project?

Open-source robotics and autonomous systems are evolving at breakneck speed. This repo is the backbone of our podcast **"Robotics OSS Radar"** — a weekly deep-dive into the projects shaping the future of autonomous machines. We track commits, highlight development trends, and translate technical progress into compelling episodes.

---

## 🏆 Top 3 Projects Under the Microphone

These are the three most relevant and active repositories discovered via GitHub's `robotics` and `autonomous-vehicles` topics, with latest commit analysis as of September 18, 2026.

---

### 1. 🟢 [commaai/openpilot](https://github.com/commaai/openpilot)

| | |
|---|---|
| **Stars** | ⭐ 63,680 |
| **Language** | Python |
| **Focus** | Open-source driver assistance system — an operating system for robotics that upgrades the DAC on 300+ supported cars |
| **Last Activity** | September 18, 2026 (5 commits same day — extremely active!) |

**What it does:** openpilot is a community-developed, open-source driver assistance system that replaces factory ADAS with a more capable, continuously improving alternative. It's part operating system, part perception stack, and part control engine — running real-time neural networks on embedded hardware to deliver adaptive cruise control, lane centering, and automated driving across a massive fleet of 300+ supported vehicles.

**Recent Development Highlights (as of Sep 18, 2026):**
- 🚗 **Cinque v3 Hardware Support** — Major new release (`Cinque v3`, PR #38932) bringing support for comma's latest hardware platform, enabling more vehicles with newer chip architecture for improved performance and power efficiency (Harald Schäfer)
- 📡 **Replay: Fix Ranges with Omitted Start** — Critical bugfix in the replay tooling ensuring time-range queries work correctly when the start timestamp is omitted, improving debugging reliability for developers analyzing driving logs (Trey Moen)
- 🖥️ **UI: Prime Menu Redesign** — New prime menu interface in the car UI, refreshing the user experience for swiping between passages, map, and settings (stef)
- 🔧 **Cabana: Fix Stale Message Size Warnings** — Resolved incorrect warning messages in Cabana (the CAN bus analysis tool) when message sizes were reported incorrectly, cleaning up the diagnostic experience (Trey Moen)
- 📊 **Cabana: Filter Multiplexed Signals in Binary Grid** — New filtering capability for multiplexed CAN signals in the binary grid view, making it far easier to analyze complex vehicle networks with overlapping signal protocols (Trey Moen)

**🎙️ Potential Episode Topics:**
- "Cinque v3: What's Inside comma's Newest Hardware — and Why It Matters for Open-Source ADAS"
- "Inside Cabana: Reverse-Engineering CAN Bus Networks One Signal at a Time"
- "From 300 Cars to 2000: How openpilot Built the Largest Real-World Driving Dataset"
- "Replay-ability Is Everything: How openpilot's Logging Stack Enables Scientific Driving Analysis"
- "UI/UX in a Moving Vehicle: Designing interfaces Drivers Actually Trust"

---

### 2. 🔵 [ApolloAuto/apollo](https://github.com/ApolloAuto/apollo)

| | |
|---|---|
| **Stars** | ⭐ 26,828 |
| **Language** | C++ |
| **License** | Apache-2.0 |
| **Focus** | Open autonomous driving platform — modular AV stack from Baidu |
| **Last Activity** | April 16, 2026 (latest commit); periodic updates with major feature drops |

**What it does:** Apollo is one of the most comprehensive open-source autonomous driving platforms ever created. It provides a full modular stack — perception, planning, control, simulation, and cloud services — enabling researchers and companies to build complete self-driving systems. It powers Baidu's Robotaxi service in China and is used by academic labs and industrial R&D teams worldwide.

**Recent Development Highlights:**
- 🚀 **Apollo 11.0: BEV + OCC (Bird's Eye View + Occupancy)** — Major architectural leap with native Bird's Eye View perception and Occupancy Grid-based 3D scene understanding (`feat: add Apollo 11.0 bev+occ`, PR by yuxin). This brings Apollo into the BEV+OCC paradigm that dominates current top-tier AV research (CourtesyNUSCENE, OccNet), enabling holistic 3D scene representation from multi-camera inputs.
- 🔧 **Seyond Lidar Driver Recovery** — Full merge of the Seyond lidar driver (`recover_seyond_lidar_driver`, PR #15762), restoring support for Seyond's 3D lidar sensors with updated configuration files and documentation. This expands Apollo's hardware compatibility for researchers using newer lidar setups.
- 📋 **README Build Status Badge Cleanup** — Removed invalid CI badges from the README, signaling a focus on documentation accuracy and maintainer hygiene (xiaoxinyu).
- 📖 **Seyond Lidar Driver Configuration & Readme Updates** — Comprehensive documentation for the newly restored lidar driver, including calibration parameters and integration guides (Yuechao.Gu).

**🎙️ Potential Episode Topics:**
- "Apollo 11.0 and the BEV Revolution: Why Every AV Stack Is Going Bird's Eye View"
- "Occupancy Networks Meet Autonomous Driving: What Apollo 11.0's OCC Module Means for 3D Perception"
- "The Modular Stack Debate: Is Apollo's Architecture Still State-of-the-Art in the Age of End-to-End Learning?"
- "Lidar Driver Wars: Why Hardware Compatibility Is the Unsung Hero of Open-Source AV"
- "From Baidu's Robotaxis to Your Garage: The Global Reach of Apollo"

---

### 3. 🟣 [AtsushiSakai/PythonRobotics](https://github.com/AtsushiSakai/PythonRobotics)

| | |
|---|---|
| **Stars** | ⭐ 30,536 |
| **Language** | Python |
| **License** | MIT |
| **Focus** | Python sample codes and textbook for robotics algorithms — the "learn-by-doing" reference |
| **Last Activity** | September 2, 2026 (dependabot updates); repository is well-maintained with steady hygiene |

**What it does:** PythonRobotics is the go-to open-source textbook-turned-codebase for robotics algorithms. It covers everything from localization (Kalman filters, particle filters, SLAM) to motion planning (RRT*, A*, D*), control (PID, LQR, MPC), and kinematics — all implemented in clean, readable Python with equations and diagrams. It's used in university courses worldwide and is the first stop for anyone learning robotics programming.

**Recent Development Highlights (as of Sep 2, 2026):**
- 🐍 **Scipy 1.18.1 Bump** — Updated to the latest SciPy release, ensuring compatibility with the newest sparse matrix operations and spatial transform functions that many algorithms depend on (dependabot)
- 🧹 **Ruff 0.16.5 Linter Update** — Upgraded to the latest Ruff release for faster, more accurate Python linting, keeping the codebase clean and consistent with modern Python style standards (dependabot)
- 🔒 **GitHub CodeQL Action 4.37.9** — Updated security scanning to the latest version, ensuring continuous vulnerability detection across the entire dependency tree (dependabot)
- 🔒 **Ongoing Dependency Hygiene** — Regular dependabot PRs for codeql-action (4.37.4 → 4.37.9) and ruff (0.15.16 → 0.16.1 → 0.16.5) show a healthy, security-conscious maintenance posture

**🎙️ Potential Episode Topics:**
- "PythonRobotics: The Textbook That Teaches 100,000 Engineers to Code Robots"
- "From Equations to Execution: How PythonRobotics Bridges Theory and Practice"
- "Kalman Filters to RRT*: The 8 Algorithms Every Robotics Engineer Should Know Inside-Out"
- "Why Clean Code Matters in Robotics: Lessons from 30,000 Stars and Zero Hype"
- "Teaching Robots to Think: A Conversation with PythonRobotics Creator Atsushi Sakai"

---

## 📊 Activity Snapshot (as of September 18, 2026)

| Project | Stars | Language | Latest Commit | Key Theme |
|---------|-------|----------|---------------|-------------------------------|
| openpilot | 63,680 | Python | Sep 18, 2026 — Cinque v3 + Cabana improvements + UI redesign | Fleet-scale ADAS hardware & tooling |
| Apollo | 26,828 | C++ | Apr 16, 2026 — Apollo 11.0 BEV+OCC + Seyond lidar | Modularity, BEV perception, sensor I/O |
| PythonRobotics | 30,536 | Python | Sep 2, 2026 — SciPy/Ruff/CodeQL updates | Algorithm education & dependency hygiene |

---

## 🎙️ Podcast Alignment

Each project maps to a natural episode arc:

1. **Fleet Episode** → openpilot: "What happens when 300 cars run open-source ADAS every day?"
2. **Architecture Episode** → Apollo: "Is the modular stack dead? Apollo 11.0 bets on BEV+OCC"
3. **Education Episode** → PythonRobotics: "How do you teach a robot to think — in Python?"

---

## 📋 Tracking

See the open issue **[Projects to Revisit & Upcoming Releases](https://github.com/bro26man-hash/robotics-oss-radar/issues/53)** for the running checklist of items to revisit before the next episode cycle.

---

## 🤝 Contributing

Pull requests and suggestions are welcome! To propose a new project or episode topic:
1. Open an issue describing the project and why it matters
2. Tag it with `proposal` and `episode-topic`
3. The maintainers will review and add to the radar

## 📄 License

This project is open-source under the [MIT License](LICENSE).
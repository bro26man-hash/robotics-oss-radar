# 🤖 Robotics & Autonomous Systems — Open-Source Radar

> A living radar for the most active open-source robotics and autonomous-vehicle repos, with commit summaries distilled from live `git log` inspection and podcast episode ideas for the **Robotics OSS** podcast.

_Last scan: 2026-09-17 · Sources: GitHub topic/keyword search on `robotics` & `autonomous-vehicles`, sorted by recent activity, followed by per-repo latest-commit inspection._

---

## 🔥 Top 3 Most Recently Active Repos

### 1. [carla-simulator / carla](https://github.com/carla-simulator/carla)
⭐ 14,403 ⭐ · 🏎️ C++ · 🏷️ `autonomous-vehicles`

**About:** Open-source simulator for autonomous driving research. Industry-standard reference simulator used by academia and industry worldwide for AV perception, planning, and control research.

**Latest Commits (Sep 2026):**
- `1360bb9` — **Deploy UE5 nightly to Cloudflare R2** *(9/2)* — Automating Unreal Engine 5 nightly builds to edge CDN, reducing simulator download friction for global users.
- `dd3a9d7` — **Add V2X sensor family (CAM service, path-loss, CustomV2X, V2I)** *(7/13)* — Major feature: full Vehicle-to-Everything communication layer with custom channel models and V2I messaging.
- `39c4fda` — Guard against null traffic light in WalkerManager *(7/14)* — Robustness fix for pedestrian/npc edge cases.
- `6279162` — Add `CARLA_MAPS_TO_COOK` cmake option for packaged maps *(7/10)* — Streamlined map distribution via Unreal Engine's Cook pipeline.

**What's Cooking:** CARLA is pushing hard on **V2X connectivity** — a rare and important feature in open-source AV simulators. Combined with the UE5 nightly-to-CDN deployment, the team is removing every friction point that keeps researchers from running large-scale multi-agent experiments. The V2X sensor family (CAM service, path-loss modeling, CustomV2X, V2I) is a standout: very few open-source simulators model vehicle-to-everything communication with realistic channel effects.

**🎙️ Episode Ideas:**
- *"When Cars Talk to Everything: V2X Simulation Goes Open-Source"* — CARLA's new V2X sensor family and why it matters for AV safety validation.
- *"Shipping UE5 Nightlies to 190 Countries"* — Cloudflare R2 deployment patterns for heavy-duty research simulators.
- *"The Map-Pipeline Problem: CARLA's Cook Strategy"* — how simulator teams solve map distribution at scale.

---

### 2. [autowarefoundation / autoware](https://github.com/autowarefoundation/autoware)
⭐ 12,065 ⭐ · 🐧 Dockerfile/YAML · 🏷️ `autonomous-vehicles`

**About:** Autoware — the world's leading open-source software project for autonomous driving. Full-stack AV software: perception, planning, control, localization, and HD map integration.

**Latest Commits (Sep 2026):**
- `a45f9ba` — Minor update to `managed_transform_buffer` to v0.3.0 *(9/16)* — Internal dependency bump improving TF2 management for real-time AV transforms.
- `79446c0` — Add CARLA 0.10 Town10HD_Opt map to demo_artifacts *(9/9)* — New simulation map for end-to-end demo validation.
- `87f7b60` — Fix simple-planning-simulator Docker build with core packages *(9/8)* — CI/Docker packaging fix, ensuring the built-in simulator always works.
- `3354a27` — Pin CasADi to 3.7.2 for Humble ARM64 *(9/7)* — Cross-platform stability fix for ARM64/Ubuntu systems (critical for in-vehicle deployment).
- `c0a32e8` — Trim CI health-check PR matrix to amd64 main legs *(9/7)* — CI optimization to reduce CI resource waste.

**What's Cooking:** Autoware's recent work is all about **reliability and reproducibility** — dependency pinning, Docker build fixes, ARM64 compatibility, and CI optimization. The CasADi pin for ARM64 Humble is especially significant: it signals the project is maturing for on-vehicle (edge) deployment, not just cloud-based validation. The Town10HD_Opt map addition keeps the demo pipeline fresh.

**🎙️ Episode Ideas:**
- *"Reasoning on the Edge: Autoware's ARM64 Journey"* — why pinning math libraries for ARM64 matters for in-vehicle autonomy.
- *"The Dockerfiles Behind an Autonomous Vehicle"* — how Autoware's CI/CD pipeline keeps a 12,000-star AV stack reproducible.
- *"Town10HD_Opt & the Demo Pipeline Problem"* — keeping reference simulations current in open-source autonomy.

---

### 3. [rpng / open_vins](https://github.com/rpng/open_vins)
⭐ 3,104 ⭐ · 🔬 C++ · 🏷️ `robotics`

**About:** An open-source platform for visual-inertial navigation research. Provides modular, publishable algorithms for camera + IMU fusion — used in UAVs, ground robots, and AR/VR.

**Latest Commits (Nov 2025):**
- `6948812` — Merge PR #530: Android support *(11/30)* — Full Android logging and build integration, extending VINS-Mono to mobile platforms.
- `6cf212d` — Merge PR #520: Android feature branch *(11/30)* — Additional Android feature consolidation.
- `6b4abfd` — Merge branch 'master' into Android *(11/16)* — Branch sync for Android port stability.
- `77ec88d` — Add Android logging support *(11/16)* — Logcat integration for on-device debugging.

**What's Cooking:** Open-VINS has shipped **full Android support** — a significant milestone that moves visual-inertial navigation from the research lab onto commodity mobile hardware. The Android logging and build integration means researchers can now run VINS on phones, which opens doors for consumer robotics, AR/VR, and edge-based SLAM. The 6-month gap between the last set of commits suggests the team is in a stabilization/catch-up phase.

**🎙️ Episode Ideas:**
- *"VINS on Your Phone: Visual-Inertial Navigation Goes Mobile"* — the implications of Android support for consumer robotics and AR.
- *"Why Visual-Inertial Fusion Matters for Edge Robots"* — camera + IMU complementarity on resource-constrained hardware.
- *"From Research Paper to Android APK: Shipping VINS for Everyone"* — the engineering journey to mobile deployment.

---

## 📊 Radar Summary

| # | Repo | Stars | Language | Domain | Key Trend |
|---|------|-------|----------|--------|-----------|
| 1 | carla-simulator/carla | 14,403 | C++ | AV Simulator | V2X connectivity & UE5 deployment automation |
| 2 | autowarefoundation/autoware | 12,065 | Docker/YAML | AV Stack | ARM64 edge deployment & CI hardening |
| 3 | rpng/open_vins | 3,104 | C++ | Visual-Inertial Nav | Android/mobile platform expansion |

---

## 🎙️ About This Radar

Curated for the **Robotics OSS** podcast and refreshed periodically. Selection priorities:
- Genuine open-source robotics / autonomous-vehicle projects
- Active recent commit cadence (truly "being worked on")
- Strong narrative potential for podcast episodes

See the companion issue **[Projects to Revisit & Upcoming Releases](../../issues/15)** for the tracking checklist.

---

## 🔎 How to Use

1. Scan the **Top 3** above for current development highlights.
2. Pick an episode idea that resonates.
3. Check the companion issue for follow-up items (revisit dates, upcoming releases to watch).

---

_Licensed as part of the open-source robotics podcast ecosystem. Contributions and episode suggestions welcome._

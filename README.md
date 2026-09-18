# 🤖 Robotics OSS Radar

> Open-source robotics & autonomous systems radar — tracking the most active repos, recent development highlights, and podcast episode ideas.

---

## 📡 Tracked Projects

### 1. [MuJoCo](https://github.com/google-deepmind/mujoco) — `google-deepmind/mujoco`
**Stars:** ⭐ 15,214 &nbsp;|&nbsp; **Language:** C++ &nbsp;|&nbsp; **Topic:** `robotics`

> Multi-Joint dynamics with Contact. A general-purpose physics simulator for robotics and biomechanics research.

#### Recent Development Highlights (as of Sep 2026)
| Date | Commit | What's Happening |
|------|--------|-----------------|
| Sep 18 | `54be9cc` — Yuval Tassa | **Error handling upgrade** — `mjd_transitionFD` and `mjd_inverseFD` now raise explicit errors when sleeping is enabled, preventing silent failures in simulation pipelines. |
| Sep 18 | `2fec922` — Sam Haves | **Archive resource providers** — New abstraction for loading resources from archives, enabling portable, self-contained simulation bundles. |
| Sep 17 | `6297987` — Alessio Quaglino | **Contact fidelity fix** — Spring and damper disable flags are now correctly honored in the discrete metric's fluid and passive contact terms. |
| Sep 17 | `9c6dd2b` — Alessio Quaglino | **Flex stretch forces** — Flexible body stretch forces are now computed from edge tensions, improving soft-body and cable simulation accuracy. |
| Sep 17 | `af2c2ba` — Sam Haves | **GIL release in filament renderer** — The Global Interpreter Lock is released during filament rendering, enabling true parallelism for multi-threaded rendering workloads. |

#### 🎙️ Potential Podcast Episodes
- _"Why MuJoCo is Fixing Its Own Sleeping Bugs — and Why It Matters for Your Sim"_
- _"Archive Resource Providers: The Missing Piece for Reproducible Robotics Research"_
- _"Releasing the GIL: How MuJoCo is Unlocking Multi-Threaded Rendering"_
- _"From Rigid to Soft: MuJoCo's New Flex Stretch Force Model"_

---

### 2. [Rerun](https://github.com/rerun-io/rerun) — `rerun-io/rerun`
**Stars:** ⭐ 11,472 &nbsp;|&nbsp; **Language:** Rust &nbsp;|&nbsp; **Topic:** `robotics`

> Visualize, query, and stream multimodal robotics data. The open-source observability platform for roboticists.

#### Recent Development Highlights (as of Sep 2026)
| Date | Commit | What's Happening |
|------|--------|-----------------|
| Sep 18 | `64df84f` — Andreas Reich | **Opt-out of update checks** — JS API now supports disabling startup update checks, critical for air-gapped and production deployments. |
| Sep 18 | `00d6407` — Jochen Görtler | **New `misc` changeset type** — A dedicated changeset category for miscellaneous improvements, improving changelog clarity. |
| Sep 18 | `a9dcf2c` — Eric Leijonmarck | **LeRobot import diagnostics** — `re_lerobot` now collects and categorizes import warnings, making it easier to debug data pipeline issues when bringing in robot datasets. |
| Sep 18 | `94372cf` — Gábor Gyebnár | **Volume raymarcher** — A new volume raymarching renderer component, enabling high-fidelity 3D reconstruction and volumetric visualization of sensor data. |
| Sep 18 | `45d4e39` — Antoine Beyeler | **Log message refactor** — `LogMsg`, `ArrowMsg`, and related types have been lifted out of `re_log_types` into a dedicated `re_log_msg` module, improving API organization and reducing coupling. |

#### 🎙️ Potential Podcast Episodes
- _"Air-Gapped Robotics: Rerun's New Opt-Out for Update Checks"_
- _"Debugging LeRobot Imports: What Rerun's New Diagnostics Tell Us"_
- _"Volume Raymarching: The Next Frontier in Robotics Data Visualization"_
- _"Rust in Robotics: How Rerun Is Structuring its Message API"_

---

### 3. [Physicar DeepRacer for Cloud](https://github.com/PoetAndPoem4Hu/physicar-deepracer-for-cloud) — `PoetAndPoem4Hu/physicar-deepracer-for-cloud`
**Stars:** — &nbsp;|&nbsp; **Language:** Java &nbsp;|&nbsp; **Topic:** `autonomous-vehicles`

> Train your DeepRacer models in the cloud with Physicar, a platform from PhysiCar AI for easy, effective reinforcement learning.

#### Recent Development Highlights (as of Sep 2026)
| Date | Commit | What's Happening |
|------|--------|-----------------|
| Sep 18 | `6080ca4` — PoetAndPoem4Hu | **README refresh** — Project documentation updated, signaling renewed community interest and potential roadmap activity. |
| Sep 28 (2025) | `124fc4b` — PoetAndPoem4Hu | **README update** — Prior documentation study pass; the project has seen periodic maintenance. |
| Mar 2019 | `52375ae` — PoetAndPoem4Hu | **v1.2 release** — Last feature release; the core cloud-based DeepRacer training pipeline remains stable. |

#### 🎙️ Potential Podcast Episodes
- _"Cloud-Native RL: Training DeepRacer Models at Scale with Physicar"_
- _"From 2019 to 2026: What Held Back Open-Source Autonomous Vehicle Training Tools?"_
- _"Reinforcement Learning for Autonomous Racing — Is the Cloud the Right Place?"_
- _"Physicar's Resurgence: A Community-Driven Comeback Story"_

---

## 📋 Episode Planning Template

For each episode, consider the following structure:

1. **Cold Open** — 30-second hook from the latest commit
2. **What's Changed** — Walk through the 3–5 most recent commits
3. **Why It Matters** — Connect the code change to real-world robotics impact
4. **Deep Dive** — Technical breakdown of one key change
5. **OSS Watch** — Community health, contribution trends, fork activity
6. **Roundtable** — Invite a contributor or user for 15 min

---

## 🔗 Useful Links

- [MuJoCo Docs](https://mujoco.readthedocs.io/)
- [Rerun Docs](https://rerun.io/docs/)
- [Physicar README](https://github.com/PoetAndPoem4Hu/physicar-deepracer-for-cloud/blob/main/README.md)

---

*Generated by the Robotics OSS Radar project. Stay curious, stay open-source.* 🦾
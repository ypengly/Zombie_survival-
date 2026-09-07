# 🧟 Zombie Survival

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Made with JavaScript](https://img.shields.io/badge/Made%20with-JavaScript-F7DF1E?logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Platform: Web](https://img.shields.io/badge/Platform-Web-4285F4?logo=googlechrome&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web)
[![Status: Production Ready](https://img.shields.io/badge/Status-Production%20Ready-00C853?logo=vercel&logoColor=white)](https://github.com)
[![Single File](https://img.shields.io/badge/Single%20File-Yes-6C5CE7?logo=html5&logoColor=white)](https://github.com)
[![PRs Welcome](https://img.shields.io/badge/PRs-Welcome-brightgreen.svg)](https://github.com/yourusername/zombie-survival/pulls)

> **Survive the apocalypse in this action-packed 2D top-down arcade game.** Fight endless waves of zombies, level up with powerful upgrades, and see how long you can last in a destroyed city — all in a single HTML file.

**[Play Now](https://yourusername.github.io/zombie-survival)** · **[Report Bug](https://github.com/yourusername/zombie-survival/issues)** · **[Request Feature](https://github.com/yourusername/zombie-survival/issues)**

---

## ✨ Features at a Glance

<table>
<tr>
<td>

### 🧟 **Intense Combat**
- 7 unique zombie types with distinct AI
- 4 epic boss battles every 5th wave
- 5 unlockable weapons from crates
- Combo system with multi-kill callouts

</td>
<td>

### ⬆️ **Deep Progression**
- XP & leveling system with 3-card upgrades
- 12 upgrade options with stacking effects
- 3 playable characters with unique stats
- Persistent coin economy

</td>
</tr>
<tr>
<td>

### ⚡ **Power-Ups & Abilities**
- 7 temporary power-ups
- Chargeable special ability (area nuke)
- Critical hits & damage numbers
- Screen shake for impact feedback

</td>
<td>

### 📱 **Full Mobile Support**
- Dual virtual joysticks
- Touch-safe layout
- Responsive design
- Vibration & motion options

</td>
</tr>
</table>

---

## 📋 Table of Contents

- [Features](#-features)
- [Gameplay](#-gameplay)
- [Controls](#-controls)
- [Weapons](#-weapons)
- [Zombies](#-zombies)
- [Bosses](#-bosses)
- [Power-Ups](#-power-ups)
- [Leveling & Upgrades](#-leveling--upgrades)
- [Installation](#-installation)
- [Project Structure](#-project-structure)
- [Technologies](#-technologies)
- [Saving & Storage](#-saving--storage)
- [Development](#-development)
- [Browser Support](#-browser-support)
- [Contributing](#-contributing)
- [Credits](#-credits)
- [License](#-license)

---

## 🎯 Gameplay


**Survive the Arena:** You start in the middle of a large, destroyed city arena. Zombies spawn around you in waves that grow larger and harder over time — more zombies, faster zombies, tougher zombies, and eventually ranged and exploding variants.

**Fight & Adapt:** Use your weapon to fend off the horde. Each kill drops XP (levels you up), coins (banked at the end of the run), and occasionally power-ups or weapon crates.

**Build Your Power:** Chain kills quickly to build a combo, which boosts your score and coin gain. Level up to choose from 3 random upgrades that permanently enhance your abilities.

**Survive the Boss:** Every 5th wave ends with a boss fight instead of a normal spawn. Each boss has unique attack patterns and telegraphs their special attacks with red warning circles.

**The Run Ends:** When your health hits zero, the run ends. Your coins are banked, and your best stats are saved. How far can you survive?

---
🎮 Play Now
**[Play Zombie_survival in your browser →](https://ypengly.github.io/Zombie_survival-/)**

*No downloads, no installations, no sign-ups — just open and play!*


## 🎮 Controls

### ⌨️ **Desktop**

| Action | Key |
|--------|-----|
| Move | `W A S D` or Arrow Keys |
| Aim | Mouse |
| Fire (hold) | Left Click |
| Special Ability | `Space` |
| Pause | `Esc` |

### 📱 **Mobile**

| Action | Control |
|--------|---------|
| Move | Left Virtual Joystick |
| Aim & Fire (hold) | Right Virtual Joystick |
| Special Ability | Gold Circular Button |
| Pause | Button at Top of Screen |

---

## 🔫 Weapons

<table>
<tr>
<td align="center">

### 🔫 Pistol
*Balanced, reliable*
**Starting weapon**

</td>
<td align="center">

### 💥 Shotgun
*Heavy damage, wide spread, short range*
**Unlocks: Wave 6**

</td>
</tr>
<tr>
<td align="center">

### ⚡ SMG
*Very fast fire rate, lower damage*
**Unlocks: Wave 3**

</td>
<td align="center">

### 🎯 Sniper
*Slow, extremely high damage, pierces multiple zombies*
**Unlocks: Wave 9**

</td>
</tr>
<tr>
<td align="center" colspan="2">

### 🚀 Rocket Launcher
*Explosive area damage*
**Unlocks: Wave 13**

</td>
</tr>
</table>

> **Crate System:** New weapons appear as crates near the player at their unlock wave. Walk over them to switch. Your current weapon and ammo are displayed in the bottom-right HUD.

---

## 🧟 Zombies

| Type | Behavior | Difficulty |
|------|----------|------------|
| **Normal** | Slow, low health, appears in large numbers | ⭐ |
| **Runner** | Fast, low health, rushes the player | ⭐⭐ |
| **Tank** | Very slow, very high health, hits hard | ⭐⭐⭐ |
| **Spitter** | Keeps distance, fires acid projectiles | ⭐⭐⭐ |
| **Exploder** | Rushes in and detonates on contact | ⭐⭐⭐⭐ |
| **Swarm** | Tiny, fast, appears in groups | ⭐⭐⭐ |
| **Armored** | Takes reduced damage from all sources | ⭐⭐⭐⭐ |

---

## 👹 Bosses

A boss replaces the normal spawn every 5th wave, scaling in strength as waves climb. Each has a large health bar at the top of the screen and telegraphs its special attack with a red warning circle before it lands.

| Boss | Attack Style | Difficulty |
|------|--------------|------------|
| **The Brute** | Massive health, ground-slam AOE attack | ⭐⭐⭐ |
| **The Mutant** | Fast, charges the player in a straight dash | ⭐⭐⭐⭐ |
| **The Necromancer** | Summons additional normal zombies | ⭐⭐⭐⭐ |
| **The Abomination** | Cycles randomly through all three attack types | ⭐⭐⭐⭐⭐ |

---

## ⚡ Power-Ups

| Power-Up | Effect |
|----------|--------|
| ❤️ **Health Pack** | Restores health instantly |
| 🔥 **Rapid Fire** | Greatly increases fire rate for a short time |
| 💪 **Damage Boost** | Increases weapon damage for a short time |
| 🛡️ **Shield** | Temporary full invulnerability |
| 🧲 **XP Magnet** | Massively increases pickup radius for a short time |
| ❄️ **Freeze** | Slows nearby zombies for a short time |
| 💀 **Nuke** | Heavily damages every zombie currently on screen |

---

## ⬆️ Leveling & Upgrades

### How It Works
- Kills drop XP orbs
- Filling the XP bar levels you up
- The action pauses, and you choose from **3 upgrade cards**
- Each upgrade can be picked multiple times up to a cap
- Upgrades stack with each other

### Upgrade Pool (12 Options)

| Upgrade | Effect |
|---------|--------|
| 💥 Damage | Increases weapon damage |
| ⚡ Attack Speed | Increases fire rate |
| 🎯 Critical Chance | Chance to deal critical hits |
| 💀 Critical Damage | Bonus damage on critical hits |
| 🛡️ Armor | Reduces incoming damage |
| ❤️ Max Health | Increases maximum health |
| 🏃 Move Speed | Increases movement speed |
| 🧲 Pickup Radius | Increases pickup range |
| 🔄 Magazine Size | Increases ammo capacity |
| 💣 Explosive Rounds | Adds explosive splash damage |
| 🔱 Multishot | Fires additional projectiles |
| 💚 Health Regen | Regenerates health over time |

---

## 📦 Installation

### Single File — Zero Setup

The game is a single self-contained HTML file. No installation, no dependencies, no backend.

#### Option 1: Download & Play
1. Download `zombie-survival.html`
2. Double-click it or drag it into a browser window
3. **Play immediately**

#### Option 2: Clone & Serve (Optional)
```bash
git clone https://github.com/yourusername/zombie-survival.git
cd zombie-survival
python3 -m http.server 8000
# Visit http://localhost:8000
```

#### Option 3: Offline Play
Once downloaded, the game works completely offline — no internet connection required.

---

## 📁 Project Structure

The game ships as one file:

```
zombie-survival.html
└── All markup, styling, and game logic
```

### Internal Organization
The script is organized into clearly commented sections:

1. **Constants & Storage** — Configuration, defaults, localStorage wrapper
2. **Audio** — Web Audio synthesizer (no external files)
3. **Canvas Setup** — Rendering context, scaling
4. **Entity Definitions** — Characters, weapons, zombies, bosses, upgrades, power-ups, achievements
5. **Game State** — Core game objects and variables
6. **Obstacles** — Arena walls and environmental elements
7. **Run & Wave Setup** — Wave generation, spawning logic
8. **Input Handling** — Keyboard, mouse, touch controls
9. **Combat** — Damage, bullets, collision detection
10. **Zombie & Boss AI** — Behavior patterns and pathfinding
11. **Player Update** — Movement, health, leveling
12. **Bullets, Pickups & Particles** — Projectiles, drops, effects
13. **HUD Sync** — UI updates
14. **Render Loop** — Main game loop
15. **Menu & Flow Wiring** — Screen management, event listeners

---

## 🛠️ Technologies

- **HTML5 Canvas** — All rendering, sprites, and effects
- **Vanilla JavaScript** — No frameworks, no build step, no external libraries
- **CSS3** — Responsive layout, styling, and animations
- **Web Audio API** — Synthesized sound effects (no audio files)
- **localStorage** — Persistent save data
- **Google Fonts** — Bebas Neue, JetBrains Mono, Inter (CDN; fallback fonts work offline)

---

## 💾 Saving & Storage

All progress is saved automatically:

| Saved Data | Description |
|------------|-------------|
| 🏆 Best Score | Highest score achieved |
| 🌊 Best Wave | Farthest wave reached |
| 💀 Best Kills | Most kills in a single run |
| ⏱️ Best Survival Time | Longest survival time |
| 🪙 Banked Coins | Coins earned and saved across runs |
| ⚙️ Settings | Music, SFX, vibration, motion preferences |

**How It Works:**
- Saved automatically at the end of each run
- Settings saved whenever changed
- **Reset progress** option in Settings (with confirmation)
- Graceful fallback if `localStorage` is unavailable

---

## ⚡ Performance

- **Optimized Rendering:** Efficient Canvas 2D rendering with culling
- **Entity Management:** Off-screen entities filtered regularly
- **Particle System:** Efficient particle pooling and lifetime management
- **Audio Synthesis:** Lightweight Web Audio with no external files
- **Frame Rate:** Target 60 FPS with delta-time compensation
- **Mobile Optimized:** Touch input optimized for performance

---

## 🌐 Browser Support

| Browser | Version | Status |
|---------|---------|--------|
| Chrome | Latest | ✅ Fully Supported |
| Firefox | Latest | ✅ Fully Supported |
| Safari | Latest | ✅ Fully Supported |
| Edge | Latest | ✅ Fully Supported |
| Android | Latest | ✅ Fully Supported |
| iOS/iPadOS | Latest | ✅ Fully Supported |

Requires: Canvas, `requestAnimationFrame`, and Web Audio API support.

---

## 👨‍💻 Development

### Tuning Everything

All game balance is controlled through objects near the top of the script:

#### 🧟 Zombie Stats — `ZOMBIE_DEFS`
```javascript
{
  normal: { health: 30, speed: 1.2, damage: 10, radius: 16, xpVal: 10, coinVal: 2 },
  runner: { health: 15, speed: 2.8, damage: 8, radius: 14, xpVal: 12, coinVal: 3 },
  // ...
}
```

#### 👹 Boss Stats — `BOSS_DEFS`
```javascript
{
  brute: { health: 500, damage: 30, speed: 1.0, attackPattern: 'slam' },
  mutant: { health: 350, damage: 20, speed: 2.5, attackPattern: 'dash' },
  // ...
}
```

#### 🌊 Wave Difficulty — `difficultyForWave(n)`
```javascript
function difficultyForWave(n) {
  return {
    healthMultiplier: 1 + n * 0.1,
    speedMultiplier: 1 + n * 0.05,
    damageMultiplier: 1 + n * 0.08,
    zombiesPerWave: 5 + n * 1.5,
    spawnInterval: Math.max(200, 800 - n * 10)
  };
}
```

#### 🔫 Weapon Stats — `WEAPONS`
```javascript
{
  pistol: { damage: 15, fireRate: 300, spread: 0.05, magazine: 12, reload: 800 },
  shotgun: { damage: 8, fireRate: 600, spread: 0.3, magazine: 6, reload: 1200, pellets: 5 },
  // ...
}
```

#### ⬆️ Upgrade Values — `UPGRADE_POOL`
```javascript
{ id: 'damage', label: '💥 Damage', effect: () => { /* ... */ }, maxPicks: 5 },
{ id: 'attackSpeed', label: '⚡ Attack Speed', effect: () => { /* ... */ }, maxPicks: 5 }
```

### Adding New Content

- **New Zombie Type:** Add entry to `ZOMBIE_DEFS` and `zombieSpawnWeights`
- **New Boss:** Add entry to `BOSS_DEFS` and update boss selection logic
- **New Weapon:** Add entry to `WEAPONS` and `WEAPON_UNLOCK_WAVES`
- **New Upgrade:** Add entry to `UPGRADE_POOL`
- **New Power-Up:** Add entry to `POWERUP_DEFS` and implement effect

---

## 🤝 Contributing

We welcome contributions! Here's how you can help:

### 🐛 Report Bugs
- Check existing issues first
- Include steps to reproduce, expected vs actual behavior
- Add screenshots if applicable

### 💡 Suggest Features
- Open an issue with the "enhancement" label
- Describe the feature and why it would be valuable

### 🔧 Submit PRs
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

### 📝 Coding Standards
- Keep it Vanilla JS — no frameworks or build tools
- Comment your code (JSDoc style preferred)
- Follow the existing single-file structure
- Test on both desktop and mobile

---

## 🙏 Credits

- **Game Design & Development:** [Your Name]
- **Fonts:** Bebas Neue, JetBrains Mono, Inter from Google Fonts (Open Font License)
- **Sound:** All sound effects synthesized at runtime via Web Audio API
- **Art:** All visuals drawn procedurally on Canvas

**No third-party assets** — everything is pure HTML5, CSS3, and JavaScript in a single file.

---

## 📄 License

Provided as-is for personal use, learning, and modification.

```
MIT License — Copyright (c) 2026

Permission is hereby granted, free of charge, to any person obtaining a
copy of this software and associated documentation files, to deal in the
software without restriction, including without limitation the rights to
use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the software, subject to the standard MIT conditions.
```

---

## ⭐ Support

If you enjoyed this project, please consider:
- **Starring** the repository on GitHub
- **Forking** to build your own version
- **Sharing** with friends and fellow gamers
- **Contributing** improvements and bug fixes

---

<div align="center">

**[Play Now](https://yourusername.github.io/zombie-survival)** · **[Report Bug](https://github.com/yourusername/zombie-survival/issues)** · **[Request Feature](https://github.com/yourusername/zombie-survival/issues)**

**Built with ❤️ for the love of gaming and open source**

</div>

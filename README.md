# Zombie Survival

A 2D top-down arcade survival game. Move, shoot, level up, and hold out against endless waves of zombies in a destroyed city — playable directly in the browser, no install, no account, no backend.

## Features

- Arena survival with a camera that follows the player and a destroyed-city backdrop
- 7 zombie types, each with distinct movement and attack behavior
- 4 boss zombies with telegraphed special attacks, cycling in every 5th wave
- 5 unlockable weapons, found as crate drops as waves progress
- XP and leveling with a 3-card upgrade choice on every level-up
- 7 temporary power-ups
- Combo system, damage numbers, critical hits, multi-kill callouts, screen shake
- A chargeable special ability (area nuke)
- 3 playable characters with different stats
- Full mobile support: dual virtual joysticks, ability button, touch-safe layout
- Saved best score, best wave, best kills, and banked coins between sessions
- Settings for music, sound effects, vibration, and reduced motion
- Synthesized audio (no external sound files) — silently continues if audio is blocked

## Gameplay

You start in the middle of a large arena. Zombies spawn around you in waves that get larger and harder over time — more zombies, faster zombies, tougher zombies, and eventually zombies that come at you from range or explode on contact. Every 5th wave ends with a boss fight instead of a normal spawn.

Killing zombies drops XP (levels you up), coins (banked at the end of the run), and occasionally power-ups or weapon crates. Chain kills quickly to build a combo, which boosts your score and coin gain. Survive as long as you can — the run ends when your health hits zero.

## Controls

**Desktop**
| Action | Key |
|---|---|
| Move | `W A S D` or arrow keys |
| Aim | Mouse |
| Fire | Left click (hold) |
| Special ability | `Space` |
| Pause | `Esc` |

**Mobile**
| Action | Control |
|---|---|
| Move | Left virtual joystick |
| Aim & fire | Right virtual joystick (hold) |
| Special ability | Gold circular button |
| Pause | Button at top of screen |

## Weapons

| Weapon | Style | Unlocks |
|---|---|---|
| Pistol | Balanced, reliable | Starting weapon |
| Shotgun | Heavy damage, wide spread, short range | Starting choice / wave 6 |
| SMG | Very fast fire rate, lower damage | Starting choice / wave 3 |
| Sniper | Slow, extremely high damage, pierces multiple zombies | Wave 9 |
| Rocket Launcher | Explosive area damage | Wave 13 |

New weapons appear as a crate near the player at their unlock wave. Walk over it to switch — your current weapon and ammo are shown in the bottom-right HUD.

## Zombies

| Type | Behavior |
|---|---|
| Normal | Slow, low health, shows up in large numbers |
| Runner | Fast, low health |
| Tank | Very slow, very high health, hits hard |
| Spitter | Keeps its distance and fires acid projectiles |
| Exploder | Rushes in and detonates on contact |
| Swarm | Tiny, fast, appears in groups |
| Armored | Takes reduced damage from all sources |

## Bosses

A boss replaces the normal spawn every 5th wave, scaling in strength as waves climb. Each has a large health bar at the top of the screen and telegraphs its special attack with a red warning circle before it lands.

- **The Brute** — massive health, ground-slam AOE attack
- **The Mutant** — fast, charges the player in a straight dash
- **The Necromancer** — summons additional normal zombies
- **The Abomination** — cycles randomly through all three attack types

## Power-Ups

| Power-up | Effect |
|---|---|
| Health Pack | Restores health instantly |
| Rapid Fire | Greatly increases fire rate for a short time |
| Damage Boost | Increases weapon damage for a short time |
| Shield | Temporary full invulnerability |
| XP Magnet | Massively increases pickup radius for a short time |
| Freeze | Slows nearby zombies for a short time |
| Nuke | Heavily damages every zombie currently on screen |

## Leveling

Kills drop XP orbs. Filling the XP bar levels you up, pauses the action, and offers a choice of 3 upgrade cards drawn from a pool of 12 (damage, attack speed, critical chance and damage, armor, max health, move speed, pickup radius, magazine size, explosive rounds, multishot, and health regen). Each upgrade can be picked multiple times up to a cap, and stacks with the others.

## Installation

No installation needed.

1. Download `zombie-survival.html`
2. Open it in any modern browser (double-click it, or drag it into a browser window)
3. Play

It's a single self-contained file — everything (styling, game logic, and sound) is embedded, so it works offline once downloaded.

## Project Structure

The game ships as one file:

```
zombie-survival.html   All markup, styling, and game logic
```

Internally, the script is organized into clearly commented sections in this order: constants/storage, audio, canvas setup, entity definitions (characters, weapons, zombies, bosses, upgrades, power-ups, achievements), game state, obstacles, run/wave setup, input handling, combat, zombie/boss AI, player update, bullets/pickups/particles, HUD sync, the render loop, and menu/flow wiring.

## Technologies

- Vanilla JavaScript (no build step, no frameworks, no external libraries)
- HTML5 Canvas for rendering
- Web Audio API for synthesized sound effects (no audio files)
- `localStorage` for saved progress
- Google Fonts (Bebas Neue, JetBrains Mono, Inter) loaded via CDN link — the game still runs offline without them, just with fallback fonts

## Saving

Best score, best wave, best kill count, best survival time, banked coins, and your settings are saved to `localStorage` automatically at the end of each run and whenever a setting changes. Use **Reset progress** in Settings to clear everything (this asks for confirmation first). If `localStorage` is unavailable, the game still runs — progress just won't persist between sessions.

## Development

Everything is tuned through a handful of objects near the top of the script:

- **Zombie stats** — `ZOMBIE_DEFS` (health, speed, damage, radius, XP/coin value per type)
- **Boss stats** — `BOSS_DEFS` (health, damage, speed, attack pattern per boss)
- **Wave difficulty & spawn rate** — `difficultyForWave(n)` (health/damage/speed multipliers, zombies per wave, spawn interval, all as functions of wave number)
- **Weapon stats** — `WEAPONS` (damage, fire rate, spread, magazine, reload, pellets, range)
- **Weapon unlock schedule** — `WEAPON_UNLOCK_WAVES`
- **XP values** — `xpVal` field in `ZOMBIE_DEFS`, level curve in `gainXP()`
- **Upgrade values** — `UPGRADE_POOL` (effect and per-upgrade pick cap)
- **Boss frequency** — the `wave.n % 5 === 0` check in `nextWave()`

## Browser Support

Any modern desktop or mobile browser with Canvas, `requestAnimationFrame`, and Web Audio support: current Chrome, Firefox, Safari, and Edge. Runs on Android, iOS/iPadOS, and desktop.

## Credits

All visuals are drawn procedurally on canvas, and all sound is synthesized at runtime — no third-party art, audio, or font files are bundled. Fonts (Bebas Neue, JetBrains Mono, Inter) are loaded from Google Fonts under their respective open licenses.

## License

Provided as-is for personal use, learning, and modification.

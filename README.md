# 🏎️ NEON DRIFT — Cyberpunk Arcade Combat Racer

A high-speed, single-file cyberpunk arcade combat racer built with HTML5 Canvas, Vanilla JavaScript, Tailwind CSS, and procedural Web Audio synthesis. Thread your vector interceptor through 5 lanes of neon traffic, trigger electric **Near-Miss ("Graze")** combos, arm **Twin Railguns**, unleash **Full Overdrive**, and obliterate colossal **OMEGA JUGGERNAUT** war-rigs every 1,500 meters!

---

## ✨ Key Features

* **60 FPS Dual-Pass Vector Neon Engine:** Additive outer neon glows (`lighter` blend mode) paired with razor-sharp inner vector cores, dynamic vehicle banking tilt, neon tire-drift skid trails, pulsing shoulder equalizer pylons, pooled particle sparks, and capped `devicePixelRatio` (`<= 2`).
* **Near-Miss ("Graze") & 10X Combo System:** Threading within `26px` of enemy vehicles or laser barriers arcs live electricity between your hulls, awards `"NEAR MISS! +150"`, builds up to a **10X Score Multiplier** (with a `3.4s` combo decay bar), and charges **+15%** of your Overdrive gauge.
* **Full Overdrive (2X Rampage):** Reach `100%` Overdrive charge to trigger **6.0 seconds** of rainbow-neon invulnerability, **1.55x top speed**, **5-lane magnetic shard/capsule pull**, a **2X score multiplier**, and vehicle-smashing ramming power (`+300` base points per hit).
* **Hull Integrity & Anti-Double-Hit Defense:** Start with **3 Hull Hearts**; taking damage triggers `1.2s` of invulnerability flicker and a **230px clearing shockwave** that wipes nearby hazards and projectiles so you are never unfairly double-hit.
* **Procedural Web Audio Synth:** Real-time pitch-modulated engine hum, bandpass-filtered tire-drift screech, escalating near-miss chimes, railgun blasts, boss sirens, and explosions—with zero external audio assets required.
* **Adaptive Desktop & Touch Controls:** Seamless keyboard steering on desktop, plus both direct horizontal touch-drag steering on the highway and tactile bottom steering/Overdrive pads on mobile devices.

---

## ⚡ 6 Highway Power-Up Capsules

| Badge | Power-Up | Duration | Effect & Combat Bonus |
| :--- | :--- | :--- | :--- |
| **⚡** | **Hyper Nitro** | `6.0s` | Invulnerable high-speed smash rampage (`+300` base points per vehicle smashed). |
| **🔫** | **Twin Railguns** | `8.0s` | Wing-mounted plasma cannons auto-fire rapid bolts that shred traffic, mines, and Bosses. |
| **🛡** | **Aegis Shield** | `12.0s` | Repairs **+1 Hull** immediately on pickup and absorbs a crash with an Aegis Bash (`+250` base points). |
| **🧲** | **Mag-Field** | `9.0s` | Activates a 5-lane electromagnetic vacuum that pulls in Data Shards and Power-Up Capsules. |
| **❄** | **Chrono Slow** | `7.0s` | Slows enemy traffic, Hunter lane lunges, and Boss hazards by **50%** for precision dodging. |
| **💥** | **EMP Nova** | `Instant` | Detonates a screen-wide shockwave that clears all traffic/projectiles (`+120` pts each) and deals **450 damage** to Bosses. |

---

## 🚓 Highway Hazards & Mega Bosses

* **Cyber Traffic Cruisers:** High-speed neon cruisers patrolling the 5-lane superhighway (wave generation always guarantees at least 2 open lanes).
* **Pulsing Laser Barriers:** Horizontal plasma emitters spanning a lane that must be dodged, blasted with Twin Railguns, or smashed with Hyper Nitro/Overdrive.
* **Hunter Police Interceptors (Sector 2+):** Flashing red-and-blue interceptors that lock onto your lane with a **telegraphed red laser sightline** before lunging sideways to cut you off.
* **OMEGA JUGGERNAUT Mega Bosses (Every 1,500m):** Colossal 3-lane armored war-rigs (`MK-1`, `MK-2`, and beyond) featuring:
  * A dedicated **Boss Health Bar** and lateral lane-patrol AI.
  * **Telegraphed Twin Laser Cannons** and **Pulsing Plasma Mines**.
  * Open-lane **Weapon Overcharge Pods** (`Railgun`, `OD+`, `EMP`) spawned throughout the battle so you can blast or Overdrive-ram the Juggernaut to advance to the next Sector.

---

## 🎮 Controls

### Desktop
| Action | Keys |
| :--- | :--- |
| **Steer Left / Right** | `A` / `D` or `Left` / `Right` Arrow Keys |
| **Surge Speed / Brake** | `W` / `S` or `Up` / `Down` Arrow Keys |
| **Activate Full Overdrive** | `Space` (or click the HUD Overdrive Gauge) |
| **Pause / Resume** | `P` or `Esc` |
| **Mute / Unmute Audio** | `M` |

### Mobile & Touch Devices
* **Highway Touch-Drag:** Drag your finger horizontally anywhere on the highway canvas for smooth 1:1 steering.
* **Tactile Bottom Pads:** Use the bottom-left `◀` and bottom-right `▶` buttons to steer, and tap the center `⚡ OVERDRIVE` button when charged to `100%`.

---


## 🛠️ Tech Stack

* **HTML5 Canvas (2D Context):** Dual-pass additive vector rendering, 5-lane scrolling perspective grid, tire-drift trail ring buffer, and pooled particle systems.
* **Vanilla JavaScript (ES6+):** Real-time delta-time physics and collision engine, Near-Miss graze detection, multi-phase Boss AI, and `localStorage` high-score persistence.
* **Web Audio API:** Procedural continuous engine/drift synthesis and polyphonic sound effects.
* **Tailwind CSS (CDN) & Orbitron Typography:** High-contrast cyberpunk HUD telemetry, active power-up timers, Boss Health Bar, and responsive modal overlays.

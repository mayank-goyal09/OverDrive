# 🏎️ OverDrive — Quantum Drift

[![Play Game](https://img.shields.io/badge/🎮_PLAY_LIVE-ONLINE-00ff66?style=for-the-badge&logo=googlechrome&logoColor=black)](https://mayank-goyal09.github.io/OverDrive/)
[![WebGL](https://img.shields.io/badge/WebGL-Three.js_r128-00ff66?style=for-the-badge&logo=webgl&logoColor=black)](https://threejs.org/)
[![FPS](https://img.shields.io/badge/Performance-60%2B_FPS_Locked-00ff66?style=for-the-badge)](https://github.com/mayank-goyal09/OverDrive)
[![Audio](https://img.shields.io/badge/Web_Audio-Procedural_Synth-00ff66?style=for-the-badge)](https://github.com/mayank-goyal09/OverDrive)
[![License](https://img.shields.io/badge/License-MIT-00ff66?style=for-the-badge)](LICENSE)

> 🌐 **Live Game URL**: [https://mayank-goyal09.github.io/OverDrive/](https://mayank-goyal09.github.io/OverDrive/)

An adrenaline-fueled, arcade-simulation 3D supercar driving game built with **Three.js** and procedural **Web Audio**. Featuring fixed-timestep 60Hz physics, chrono bullet-time drifting, mid-air stunt acrobatics, highway civilian traffic, hazard obstacles, and a sleek gamer-grade neon HUD.

---

## 🌟 Key Features

### 🏎️ Vehicle Dynamics & Roster
- **Phantom GT**: Aerodynamic high-speed hypercar tuned for top-end velocity (160+ MPH, 240+ MPH with Nitro) and precision cornering.
- **Vortex Drift**: Aggressive widebody drift tuner with rapid steering response, 1.5x combo multiplier, and rapid Chrono recharge.
- **Titan Brawler**: Heavy armored combat truck equipped with a reinforced battering ram that smashes through highway traffic and barriers.

### ⏳ Chrono Bullet-Time Drifting
- Tap or hold **`Space`** to initiate a high-angle drift.
- Engages **0.38x Bullet Time (Chrono slow-motion)**, dropping game speed while dynamically pitching audio down with cinematic resonance.
- Accumulates drift points and builds up combo multipliers for high-score domination.

### 🛫 Aerial Stunts & Mid-Air Physics
- Hit yellow stunt launch ramps to become airborne.
- Full mid-air rotational freedom:
  - **`A` / `D`**: 360° Barrel Rolls
  - **`W` / `S`**: Backflips and Frontflips
- Stick clean landings to trigger **`BARREL STUNT LANDED! +1500`** bonuses and instant Quantum Nitro refills.

### 🚧 Dynamic Highway Obstacles & Traffic
- **Civilian Traffic**: AI-driven convoy of civilian vehicles across all 4 highway lanes with functioning headlights and taillights.
- **Construction Safety Barrels**: Reflective orange/white hazard barrels with blinking amber beacons blocking lanes.
- **Stunt Jump Ramps**: Angled launch pads equipped with neon cyber guide rails.
- **Nitro Crystals**: Floating rotating octahedron crystals that restore Nitro to 100% and reward bonus score.
- **Titan Smash / Overdrive**: Ramming obstacles or traffic in Nitro boost or Titan mode obliterates them with flying spark debris.

### 🔊 100% Procedural Web Audio Synthesizer
- Zero external audio assets or downloads required.
- Synthesizes real-time V8 engine RPM pitch shifts, turbo blowoff hiss, tire friction screech, metal collision impacts, and an arpeggiated retro synthwave soundtrack completely client-side using Web Audio API nodes.

### ⚡ 60+ FPS Performance Architecture
- **Fixed Timestep Physics Loop (1/60s)**: Eliminates display refresh-rate jitter across 60Hz, 120Hz, and 144Hz monitors.
- **Zero GC in Animation Loop**: Scratch vector recycling (`_vCamTarget`, `_vLookTarget`) prevents browser Garbage Collector pauses.
- **Ring-Buffer Chunk Recycling**: Pre-allocated highway chunks leapfrog behind the player, eliminating chunk creation lag spikes.
- **Exponential Spring Damping**: Camera follow and steering interpolation use mathematical exponential decay for butter-smooth movement.

---

## 🎮 Controls

| Action | Keyboard | Mobile / Touch |
| :--- | :--- | :--- |
| **Accelerate** | `W` or `↑` | `▲` Gas Pedal |
| **Brake / Reverse** | `S` or `↓` | `▼` Brake Pedal |
| **Steer Left / Right** | `A` / `D` or `←` / `→` | `◀` / `▶` Buttons |
| **Chrono Drift (Slow-Mo)** | `Spacebar` | `⚡ DRIFT` Button |
| **Nitro Boost** | `Left Shift` | `🌀 NITRO` Button |
| **Cycle Camera (4 Modes)** | `C` | `📷 CAM` Button |
| **Overclock Boost** | `E` or `Q` | Dimension Badge |
| **Reset Vehicle** | `R` | Top Menu |
| **Toggle Audio** | `M` | `🔊 AUDIO` Button |
| **Fullscreen** | `F` | `⛶ FULL` Button |
| **Pause Menu** | `Escape` | `⏸ PAUSE` Button |

### 🎥 4 Selectable Camera Modes
1. **Chase Cam**: Dynamic velocity-responsive third-person camera.
2. **Low Drift Cam**: Low-angle street-level perspective emphasizing drift angles.
3. **Cockpit Dashboard**: Immersive driver POV with functioning dashboard telemetry.
4. **Top-Down Arcade**: Classic overhead birds-eye arcade view.

---

## 🚀 Quick Start

### Option 1: Direct Browser Play
Double-click `play_game.bat` on Windows, or simply open `index.html` in any modern web browser (Chrome, Edge, Firefox, Brave, Safari).

### Option 2: Local HTTP Server
Run a local static server for optimal asset caching:
```bash
# Python
python -m http.server 3000

# Node.js
npx serve -p 3000
```
Then navigate to `http://localhost:3000`.

---

## 📁 Repository Structure

```
OverDrive/
├── index.html        # Complete standalone 3D WebGL game engine & gamer HUD
├── three.min.js      # Three.js 3D library (bundled for full offline capability)
├── favicon.svg       # Custom neon supercar vector favicon
├── play_game.bat     # Windows one-click local server launcher
└── README.md         # Documentation and guide
```

---

## 🛠️ Built With

- **[Three.js (r128)](https://threejs.org/)** — WebGL 3D rendering pipeline
- **HTML5 Canvas** — Procedural procedural asphalt, carbon fiber, and skyline textures
- **Web Audio API** — Real-time polyphonic audio synthesis
- **Vanilla JavaScript (ES6+)** — Zero framework overhead

---

## 📄 License

MIT License — free to play, modify, and build upon.

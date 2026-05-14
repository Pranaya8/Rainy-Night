# ⛈️ Stormbrella (Umbrella Drift)

**Stormbrella** is an atmospheric, physics-based arcade survival game built entirely in a single HTML5 file. Navigate through a turbulent storm, using your umbrella to catch the wind, dodge debris, and master the art of the "Perfect Drift."

---

## 🎮 Game Overview

In **Stormbrella**, you control a character descending through a high-velocity storm. The goal is simple: survive as long as possible. However, the wind is unpredictable, and the air is filled with hazardous debris. By opening your umbrella, you can slow your fall and maneuver, but you also become more susceptible to the wind's power.

### Key Features

* **Dynamic Wind System:** A randomized wind engine that affects both player movement and visual rain patterns.
* **Physics-Based Movement:** Smooth, momentum-based horizontal travel with "Smooth Follow" logic.
* **Risk-Reward Scoring:** Earn massive points by performing "Perfect Drifts"—narrowly missing obstacles to trigger slow-motion effects and score combos.
* **Multi-Input Support:** Optimized for Mouse (Desktop), Touch (Mobile), and Device Tilt/Gyroscope (Mobile fallback).
* **Zero Dependencies:** Built with pure Vanilla JavaScript and HTML5 Canvas.

---

## 🕹️ How to Play

### Controls

| Input | Action |
| --- | --- |
| **Click / Touch (Hold)** | Open Umbrella (Slow descent / Catch wind) |
| **Move Mouse / Drag** | Move Horizontally (Smooth follow) |
| **Tilt Device** | Horizontal Steering (Bonus momentum) |
| **Release** | Close Umbrella (Fast descent / Reduce wind drag) |

### Survival Tips

1. **The Perfect Drift:** If you pass extremely close to an obstacle without hitting it, your combo meter increases and the game briefly enters slow-motion.
2. **Watch the Rain:** The angle of the rain indicates the current wind direction and strength.
3. **Manage Your Lift:** Keeping the umbrella open too long might make you a target for rising debris. Close it to dive quickly past clusters of glass and twigs.

---

## 🛠️ Technical Implementation

The game is a demonstration of efficient Canvas rendering and state management:

* **Entity Management:** Obstacles (leaves, twigs, glass) are generated with randomized spin, drift, and rotation speeds, then filtered out once they leave the viewport to maintain performance.
* **Input Logic:** Uses a hybrid approach, combining `targetX` coordinates for precision with `deviceorientation` for immersive mobile play.
* **Visual Effects:** Features a `RadialGradient` glow effect on the umbrella and a custom particle-style rain system that reacts to the `wind` variable in real-time.

---

## 🚀 Getting Started

Since the game is self-contained, there is no installation required.

1. Download the `Stormbrella.html` file.
2. Open it in any modern web browser (Chrome, Firefox, Safari, or Edge).
3. Click/Tap to start drifting!

---

## 📂 Project Structure

```text
Stormbrella/
└── Stormbrella.html  # Contains HTML structure, CSS styling, and Game Logic (JS)

```

---

## 📜 License

This project is open-source and free to use for educational or personal purposes.

---

*“Stay dry, stay alive.”*

# Island Bound: Momentum

![Unreal Engine](https://img.shields.io/badge/Engine-Unreal--Engine-0E1128?style=flat&logo=unreal-engine)
![Platform](https://img.shields.io/badge/Platform-PC-blue?style=flat)
![Genre](https://img.shields.io/badge/Genre-First--Person--Physics-orange?style=flat)

**Island Bound** is a physics-based first-person obstacle platformer. Navigate through dynamic environments using momentum and timing to reach the ultimate goal: the victory island.

---

## 🎮 Game Description
In this high-stakes platformer, players must master physics-driven mechanics to survive. From swinging across bottomless pits to dodging massive pendulums, every movement is governed by force and velocity. The objective is to navigate the treacherous path and reach the red flag on the island to progress.

---

## 🚀 Core Gameplay Features

### 🪢 Rope Swing Mechanic
* **Implementation:** Utilizes `Attach Actor` with vector-based launch calculations.
* **Physics:** Launch velocity dynamically combines forward momentum and vertical impulse for a natural "slingshot" feel.

### 🔴 Rotating Sweep Bars
* **Feedback:** Rotating cylinders apply a directional impulse upon contact using `Launch Character`.
* **Physics:** Accurately simulates force and momentum transfer, pushing players off course if they mistime their movement.

### 🍭 Pendulum Obstacle
* **Implementation:** Created using `Physics Constraints` for realistic angular motion.
* **Challenge:** Demonstrates gravity-driven physics; getting hit results in a massive kinetic launch.

### 🧱 Breakable Platforms
* **Mechanism:** Stepping on the platform triggers a timed delay before the `Physics Constraint` breaks.
* **Physics:** Gravity activates upon break, causing the platform to fall realistically.

### ⚖️ Seesaw Platform
* **Implementation:** A tilting platform utilizing a Hinge-like `Physics Constraint`.
* **Physics:** Allows rotation along a single axis based on the player’s center of mass.

---

## ⌨️ Controls

| Key | Action |
| :--- | :--- |
| **W / A / S / D** | Move Character |
| **Mouse** | Rotate Camera |
| **Space** | Jump / Grab Rope |

---

## 🎵 Audio Design

* **Persistent Music:** Background tracks loop continuously, managed via `Game Instance` to ensure seamless transitions between levels.
* **Dynamic SFX:** * Tactical feedback for jumping and rope attachment.
    * Impact sounds for pendulums and sweep bars.
    * Satisfying collapse sounds for breakable platforms.
    * **Victory:** A unique fanfare plays upon reaching the final island.

---

## 🗺️ Level Progression

* **Level 1:** Introduction to the Rope Swing mechanic.
* **Level 2:** Introduces the Seesaw and weight-based movement.
* **Level 3:** Increased difficulty with Rotating Sweep Bars and Pendulums.
* **Final Level:** The ultimate gauntlet. Combines all mechanics with added jumping obstacles for a final sprint to the Victory Island.

---

## 🎓 Acknowledgments

### Tutorials & Resources
* [Rope Swing Logic](https://www.youtube.com/watch?v=QndH9DuL_Ao)
* [Physics Constraints in UE](https://www.youtube.com/watch?v=WznFdYWM2c8)
* [Obstacle Course Design](https://www.youtube.com/watch?v=9j-eu4RvHgM&t=903s)

### Assets
* **Hexagon Kit** – [Kenney.nl](https://kenney.nl/assets/hexagon-kit)
* **Tower Defense Kit** – [Kenney.nl](https://kenney.nl/assets/tower-defense-kit)

---
*Developed for academic evaluation in Game Development.*

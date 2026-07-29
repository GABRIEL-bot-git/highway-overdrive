# 🏎️ Highway Overdrive

![HTML5](https://img.shields.io/badge/HTML5-Canvas-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6+-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![CSS3](https://img.shields.io/badge/CSS3-UI%2FUX-1572B6?style=for-the-badge&logo=css3&logoColor=white)

An interactive 2D highway driving simulation built entirely with **HTML5 Canvas** and **Vanilla Object-Oriented JavaScript**. 

This project was developed as a software engineering demonstration of real-time state management, procedural entity generation, mathematical collision detection, and defensive programming techniques within a browser environment.

---

## 🎮 Play the Game
*(Optional: If you deployed using GitHub Pages, replace the `#` below with your actual link)*
**[Play Highway Overdrive Live Here](#)**

## 🚀 Key Engineering Features

* **Synchronized Rendering Engine:** Replaces asynchronous `setInterval` loops with the `requestAnimationFrame` API to anchor rendering to the hardware display cycle, achieving a stable 60 FPS while minimizing CPU overhead.
* **Polymorphic Entity Management:** Utilizes ES6 Object-Oriented Programming (OOP) to manage game entities. A single `Obstacle` class procedurally generates both dynamic traffic and static roadblocks using randomized instantiation logic.
* **Graceful Degradation (Fault Tolerance):** Implements an asynchronous asset pipeline. If external image assets fail to load due to network latency, the system defensively degrades to rendering geometric primitives, preventing runtime crashes.
* **Memory Optimization (Entity Culling):** Actively monitors viewport bounds and splices off-screen entities from memory arrays to prevent memory leaks during extended execution.
* **AABB Collision Engine:** Employs the Axis-Aligned Bounding Box mathematical model for microsecond spatial detection, enhanced with a custom internal tolerance buffer for optimized user experience.

## 🛠️ Installation & Local Setup

Because this system utilizes a zero-dependency client-side architecture, no server-side compilation or package installation (e.g., `npm`) is required.

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/YOUR-USERNAME/highway-overdrive.git](https://github.com/YOUR-USERNAME/highway-overdrive.git)

2. **Navigate to the directory:**
    cd highway-overdrive
3. **Run the simulation:**
Simply double-click the index.html file to open it in any modern web browser (Chrome, Firefox, Edge, Safari).

🕹️ Controls
Left Arrow (←): Steer vehicle left.

Right Arrow (→): Steer vehicle right.


**📂 Project Structure**
Plaintext
highway-overdrive/
├── index.html       # Core game engine, UI overlay, and rendering logic
├── player.png       # Main character vehicle asset
├── enemy.png        # Dynamic traffic vehicle asset
├── barrier.png      # Static roadblock asset
└── README.md        # System documentation

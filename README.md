# 🐦 Flappy Bird - Unity 2D Clone

[![Unity Version](https://img.shields.io/badge/Unity-6000.0%2B-blue.svg?style=for-the-badge&logo=unity&logoColor=white)](https://unity.com/)
[![Render Pipeline](https://img.shields.io/badge/URP-Universal%20Render%20Pipeline-orange.svg?style=for-the-badge)](https://unity.com/srp/Universal-Render-Pipeline)
[![Input System](https://img.shields.io/badge/Input%20System-New-success.svg?style=for-the-badge)](https://docs.unity3d.com/Packages/com.unity.inputsystem@1.7/manual/index.html)
[![License](https://img.shields.io/badge/license-MIT-green.svg?style=for-the-badge)](LICENSE)

A modern, highly optimized, and clean implementation of the classic **Flappy Bird** game built in **Unity** utilizing the **Universal Render Pipeline (URP)** and the new **Input System**. Designed with scalability and clean programming principles in mind, it provides a solid foundation for endless runner and physics-based arcade games.

---

## 🎮 Features

- **Physics-Driven Gameplay:** Tight and responsive bird flapping controls utilizing 2D gravity simulation.
- **Dynamic Obstacle Spawning:** Custom spawning manager that spawns procedurally positioned pipes with random heights at regular intervals.
- **Seamless Parallax Effect:** Infinite background scrolling using texture offsets to simulate high-speed flight.
- **Robust Input Support:** Seamlessly supports multiple input types out of the box (Keyboard Space, Mouse Click, and Mobile Touchscreens).
- **Universal Render Pipeline (URP):** Modern rendering setup ensuring high performance, color grading, and flexibility across platforms.

---

## 🛠️ Project Structure

The project follows a clean, standardized Unity folder structure under `Assets/`:

```
Assets/
├── Materials/         # Material assets for game rendering
├── Prefabs/           # Pre-configured game objects (Pipes, Bird, Spawner, etc.)
├── Scenes/            # Unity scene files (FlappyBird.unity)
├── Scripts/           # Custom GDScript-style C# game logic scripts
├── Settings/          # URP and Renderer configuration files
├── Sprites/           # High-quality graphic assets for the game
```

### 📜 Scripts Breakdown

Our code architecture is modular and highly decoulped:

| Script Name | Purpose | Key Responsibilities |
| :--- | :--- | :--- |
| **`Player.cs`** | Bird control & physics | Listens to inputs, applies upward lift, handles gravity, triggers sprite animations, and detects collisions with pipes (obstacles) or point triggers. |
| **`GameManager.cs`** | Match state & score loop | Tracks the game score, manages UI triggers, and controls standard game-over states. |
| **`Spawner.cs`** | Procedural level generation | Instantiates pipe prefabs at a defined rate and offsets their vertical coordinates randomly. |
| **`Pipes.cs`** | Obstacle behavior | Moves pipes from right to left at a consistent speed and automatically destroys them when they exit the left edge of the viewport. |
| **`Parallex.cs`** | Infinite scrolling effect | Animates background and floor layers by dynamically shifting their materials' texture offsets over time. |

---

## 🕹️ Controls

The game is equipped with **cross-platform controls** powered by Unity's modern Input System:

- **Keyboard:** Press <kbd>Space</kbd> to flap upward.
- **Mouse:** Click <kbd>Left Mouse Button</kbd> to flap upward.
- **Mobile / Touch:** Tap anywhere on the screen to flap upward.

---

## 🚀 Getting Started

Follow these instructions to get the project up and running locally:

### Prerequisites

- **Unity Editor:** Version `2022.3 LTS` or higher (URP & New Input System pre-configured).
- **Git** (for cloning and version control).

### Setup Instructions

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/Habeeb-Rahman-CA/flappy-bird-unity.git
   cd flappy-bird-unity
   ```

2. **Open in Unity Hub:**
   - Launch **Unity Hub**.
   - Click **Add** -> **Add project from disk**.
   - Select the cloned `flappy-bird-unity` project directory.
   - Select your Unity Editor version (recommended: matching target version or newer) and open.

3. **Play the Game:**
   - In the Unity Project window, navigate to `Assets/Scenes/`.
   - Double-click `FlappyBird.unity` to open the main gameplay scene.
   - Click the **Play** (▶) button at the top of the Unity Editor to play the game!

---

## 🔮 Future Roadmap

Here are some potential enhancements to take this prototype to a full release:
- [ ] **Main Menu & UI Overhaul:** Implement title, settings, and high-score screens.
- [ ] **Audio Manager:** Integrate sound effects (flap, score, crash) and background music.
- [ ] **Skins & Personalization:** Allow players to unlock different colors and cosmetic accessories for the bird.
- [ ] **Particle Systems:** Add dynamic wind or feather particles when flapping or crashing.

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

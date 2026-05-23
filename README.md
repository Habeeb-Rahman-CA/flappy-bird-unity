# Flappy Bird Unity 2D

A simple 2D Flappy Bird clone built in Unity using the Universal Render Pipeline (URP) and the new Input System. It features clean, modular code and supports keyboard, mouse, and touch controls out of the box.

## Features
- Physics-based bird movement.
- Randomly spawning pipe obstacles.
- Infinite background parallax scrolling.
- Cross-platform controls (keyboard, mouse, mobile touch).

## How to Play
- Press Spacebar on your keyboard, left-click with your mouse, or tap your mobile screen to flap.

## Project Structure
All the game files are located inside the Assets folder:
- Materials: Render materials for game elements.
- Prefabs: Pre-made game objects (Pipes, Bird, Spawner).
- Scenes: The main game scene (FlappyBird.unity).
- Scripts: C# game logic scripts.
- Settings: Render pipeline configurations.
- Sprites: Game art and visual assets.

## Scripts
- Player.cs: Controls the bird's physics, animation, and collision.
- GameManager.cs: Manages the game state, score tracking, and game over triggers.
- Spawner.cs: Periodically spawns pipe obstacles at random heights.
- Pipes.cs: Moves the pipes left and deletes them when they leave the screen.
- Parallex.cs: Scrolls the background texture to create a movement effect.

## Setup Instructions
1. Clone the repository:
   ```bash
   git clone https://github.com/Habeeb-Rahman-CA/flappy-bird-unity.git
   ```
2. Open the project folder in Unity Hub (using Unity 2022.3 LTS or newer).
3. Open the main game scene in Assets/Scenes/FlappyBird.unity and press the Play button.

## License
This project is licensed under the MIT License.

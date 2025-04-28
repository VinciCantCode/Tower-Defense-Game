# Tower Defense Game

A classic 3D Tower Defense game built with Unity. Defend your base from waves of ground and flying enemies by strategically building and upgrading towers.

## Features

- **Multiple Tower Types:**  
  Arrow Tower, Cannon Tower, Hot Plate, Barricade, and more.  
  Each tower has unique abilities and upgrade paths.
- **Enemy Variety:**  
  Ground enemies follow a path and can be slowed or damaged by different towers.  
  Flying enemies appear every few levels and fly directly to the goal, bypassing ground obstacles.
- **Progressive Difficulty:**  
  Each level increases in difficulty with more and tougher enemies.  
  Flying enemies appear at intervals (default: every 4th level).
- **Resource Management:**  
  Earn gold by defeating enemies and completing levels.  
  Spend gold to build, upgrade, or sell towers.
- **User Interface:**  
  Intuitive UI for building, upgrading, and selling towers.  
  Visual feedback for gold, lives, and game state.

## Getting Started

### Prerequisites

- Unity 2022.3 LTS or newer

### How to Play

1. **Open the Project:**
   - Open the project in Unity Hub or Unity Editor.
   - Open the `Main.unity` scene in the `Assets/Scenes` folder.

2. **Game Controls:**
   - Use the mouse to select and place towers on the map.
   - Use arrow keys or mouse drag to move the camera.
   - Use the scroll wheel to zoom in/out.
   - Click the "Play" button to start a wave.

3. **Objective:**
   - Prevent enemies from reaching the leak point by building towers.
   - If an enemy leaks, you lose a life. The game ends when all lives are lost.

4. **Towers:**
   - **Arrow Tower:** Fast firing, targets both ground and flying enemies.
   - **Cannon Tower:** Deals area damage, effective against groups.
   - **Hot Plate:** Deals continuous damage to ground enemies within range.
   - **Barricade:** Blocks enemy paths, forcing them to take longer routes.

5. **Enemies:**
   - **Ground Enemy:** Follows the path, can be blocked or slowed.
   - **Flying Enemy:** Ignores ground obstacles, appears every 4th level by default.

6. **Level Progression:**
   - Each level spawns a set number of enemies.
   - Every 4th level (configurable), all enemies are flying enemies.

## Project Structure

- `Assets/Scenes/` - Contains the main game scene.
- `Assets/Prefabs/` - Contains prefabs for towers, enemies, and UI elements.
- `Assets/Scripts/` - Core game scripts:
  - `Player.cs` - Main game logic, level management, and enemy spawning.
  - `Enemy.cs`, `GroundEnemy.cs`, `FlyingEnemy.cs` - Enemy behaviors.
  - `Tower.cs`, `FiringTower.cs`, `Hotplate.cs` - Tower behaviors.
  - `Projectile.cs`, `ArcingProjectile.cs`, `SeekingProjectile.cs` - Projectile logic.
  - `Targeter.cs` - Handles enemy targeting for towers.
- `Assets/UI/` - UI prefabs and panels.
- `Assets/Materials/` - Materials for visual effects.

## Customization

- **Adjust enemy spawn rate, flying interval, and level difficulty** in the `Player` script via the Inspector.
- **Add new towers or enemies** by creating new prefabs and scripts based on the existing structure.

## Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss what you would like to change.

## License

This project is for educational purposes. Please check with the project owner for licensing if you plan to use it commercially. 
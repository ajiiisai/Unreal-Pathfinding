# Unreal Pathfinding
Weight based A* pathfinding implemented on Unreal Engine blueprints.

![main image](assets/pathfinding.gif)

## Controls
- Q/E: Rotate Camera
- W/A/S/D: Move Camera
- Mouse Wheel Up/Down: Zoom In/Out Camera

The obstacle base clase can be inherited, allowing the modification of the `Satic Mesh` and the `TileType enum` value.
In the current example the following are implemented:
- None
- Normal -> 1
- Difficult -> Bush -> 2
- Really dificult -> Logs -> 5
- Impossible -> Tree -> 999

The algorithm will follow the most cost effective path to the destination.

The project also implement a basic debuging UI to enable/change some parameters.

## Commands
![commands](https://safe.lyly.moe/oEq68U9yatq1.png)

- **stat fps**: Shows the current FPS
- **stat unit**: Displays performance information for the project's Frame, Game, Draw, GPU, RHIT, and DynRes threads
- **stat ubjects**: Shows performance statistics for UObjects in the game.
- **Static Meshes Flag**: Enables and disables static meshes
- **Wireframe Flag**: Shows and hides the wireframe

## Camera
![camera](https://safe.lyly.moe/fSfhAwVg6FOl.png)

Here you can change some of the camera variables to find the ones that feel the best.

The defaults are some sensible values that are a good starting zone.
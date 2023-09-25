# Unreal Pathfinding
Weight based A* pathfinding implemented on Unreal Engine using Blueprints.

![main image](assets/pathfinding.gif)

## Controls
- Q/E: Rotate Camera
- W/A/S/D: Move Camera
- Mouse Wheel Up/Down: Zoom In/Out Camera

## Functionality

Each tile has a cost, the algorithm will skip to the adjacent tile with the lower cost and repeat the process until it reaches the destination. Since it can take multiple paths at the end it will chose the one with the lower total path cost.
It will try to avoid obstacles with a high tile cost but will cross them if the overall cost is lower than the detour.

The obstacle base class can be inherited, allowing the modification of the `Satic Mesh` and the `TileType enum` value.
In the current example the following are implemented:
- None
- Normal -> 1
- Difficult -> Bush -> 2
- Really dificult -> Logs -> 5
- Impossible -> Tree -> 999

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

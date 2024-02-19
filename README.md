# Visual-Trajectory-Unity
Helper scripts for creating a trajectory visual in Unity

![Trajectory Image 1](https://github.com/Nathan-Carpenter-Git/Visual-Trajectory-Unity/assets/144058518/c5600df3-a341-473c-9dda-6dbba9293b98)
![Trajectory Image 2](https://github.com/Nathan-Carpenter-Git/Visual-Trajectory-Unity/assets/144058518/1226ac86-fe42-41fb-bf3b-3d6e60967776)

## Warning
This package only supports 2D projects

## Scripts
- Trajectory Drawer - Draws trajectory using a custom dot renderer via physics scene.
- Dot Renderer - Component that creates dots in specific positions.
- Physics Scene Manager - Handles hidden physics scene for trajectory physics calculations
- Object Pool - Customized object pool allowing for multiple instanced object pools in the same scene
- Throwable - Simple test object that throws object holding mouse button and is used in tandem with trajectory drawer.

## Setup
- Must have all scripts in scene to function (Throwable is not required if you want to create your own implementation).
- There must be an physics object as the base object. This object requires a Dot Renderer script, Trajectory Drawer script, and Throwable script (if wanted).
- In the scene there must be a singular instance of the scripts: Phyiscs Scene Manager and Object Pool.
- DotRenderer requires a dotPrefab for the dotted line (best case is a game object with a sprite renderer that has a circle or your own design for the dotted line).
- Throwable requires a "trajectory object" prefab. This prefab should be the same as the original throwable prefab without any scripts attached (only sprite renderer and rigid body 2D).

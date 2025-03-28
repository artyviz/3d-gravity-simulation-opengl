# 3D Gravity Simulation

A 3D Gravity simulation program created with GLFW for window management, GLEW for OpenGL extensions, GLM for mathematics, and ImGui for graphical user interface.

### Features

- Real-time rendering of celestial bodies
- Camera controls for navigation
- Pause and resume simulation
- ImGui controls for camera and simulation settings
- Dynamic object creation and manipulation

### Controls

- **Movement**:
  - `W`, `S`: Move the camera forward and backward along the direction it's facing.
  - `A`, `D`: Move the camera left and right, strafing it horizontally.
  - `Q`, `E`: Move the camera up and down, changing its pitch.

- **Rotation**:
  - Hold the right mouse button and move the mouse to rotate the camera around the center point.

- **Zoom**:
  - Scroll the mouse wheel to move the camera closer to or further away from the center of the simulation.

- **Center Camera**:
  - Press `C` to center the camera on the center of mass of the objects in the simulation.

### System Requirements

- OpenGL 3.3 compatible GPU
- GLFW 3.x
- GLEW 2.x
- GLM 0.9.8
- ImGui

#### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/artyviz/3d-gravity-simulation-opengl
    ```
2. Install required libraries (on Ubuntu):
   ```bash
   sudo apt-get update
   sudo apt-get install libglfw3 libglew2 libglm-dev
    ```
3. Build the project:
   ```bash
   cd 3d_simulation
  g+++ -o SpaceSimulation main.cpp imgui/imgui.cpp imgui/imgui_demo.cpp imgui/imgui_draw.cpp imgui/imgui_widgets.cpp imgui/imgui_impl_glfw.cpp imgui/imgui_impl_opengl3.cpp imgui/imgui_tables.cpp -lglfw -lGLEW -lGL -ldlX11 -ldlXext -ldlXrender -ldlGL -ldlglm
   ```
4. Run the simulation:
   ```bash
   ./3dSimulation
   ```

### Usage

- Use the controls listed above to navigate and interact with the simulation.
- Use ImGui to reset the camera, pause/resume the simulation, and adjust settings.

### Contributing

Contributions are welcome! Please submit a pull request with your changes.

### License

This project is licensed under the MIT License - see the LICENSE file for details.
```

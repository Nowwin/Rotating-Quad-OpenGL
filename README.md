# Rotating-Quad-OpenGL
Rendered a Quad in OpenGL
# OpenGL Example with SDL2

## Overview

This project is a simple example that demonstrates the usage of OpenGL in tandem with SDL2 to create a graphical application. It shows how to set up a basic vertex and fragment shader, handle user input for translation and rotation, and also how to draw a shape using the vertex and index buffer.

## Dependencies

- OpenGL
- SDL2
- GLAD for OpenGL loading
- GLM (OpenGL Mathematics)
- C++ Standard Libraries
- Filesystem (C++17 Standard Library)

## File Structure

- `main.cpp` : The main C++ file where the program starts execution.
- `shaders/vert.glsl` : Vertex shader
- `shaders/frag.glsl` : Fragment shader
- `build.py` : Python build script to compile the project into an executable.

## Key Functions

### Initialization

- `InitializeProgram()`: Initializes SDL and sets up the OpenGL context.

### Vertex Specification

- `VertexSpecification()`: Sets up the Vertex Array Object (VAO), Vertex Buffer Object (VBO), and Index Buffer Object (IBO).

### Shader Compilation and Linking

- `CreateGraphicsPipeline()`: Loads and compiles the vertex and fragment shaders and links them into a shader program.

### Main Loop and Cleanup

- `MainLoop()`: The main event loop where user input is polled and drawing occurs.
- `CleanUp()`: Cleans up resources and quits SDL.

## Error Handling

The program uses custom error-checking macros and functions (`GLCheck`, `GLClearAllErrors`, and `GLCheckErrorStatus`) for OpenGL error handling.

## User Input

The program allows the user to translate and rotate a shape using the arrow keys:

- `UP` / `DOWN`: Translate the shape along the Z-axis.
- `LEFT` / `RIGHT`: Rotate the shape around the Y-axis.

## Build Instructions

To build the project, simply run the `build.py` script:

```bash
python build.py
This will compile the project into an executable.
```
## Running the Program
After building, execute the generated binary to start the program. A window should appear displaying a shape that you can translate and rotate using the arrow keys.

For more details on the project structure and functionality, refer to the inline comments within the source code.
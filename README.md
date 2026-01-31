# Minecraft Clone

A simple Minecraft-like voxel game built with Python and the Ursina engine.

## Overview

This is a basic Minecraft clone that allows players to:
- Move around in a first-person perspective
- Place blocks by left-clicking
- Destroy blocks by right-clicking
- Explore a 20x20 block terrain

## Requirements

- Python 3.8 or higher
- ursina module (includes all dependencies)

The ursina module automatically installs the following dependencies:
- panda3d (3D game engine)
- panda3d-gltf
- panda3d-simplepbr
- pillow (image processing)
- pyperclip (clipboard access)
- screeninfo (display information)
- sswg
- typing_extensions

## Installation

### 1. Create a Virtual Environment

It is recommended to use a virtual environment to avoid conflicts with system Python packages.

```bash
python3 -m venv venv
```

### 2. Activate the Virtual Environment

On Linux/macOS:
```bash
source venv/bin/activate
```

On Windows:
```bash
venv\Scripts\activate
```

### 3. Install Dependencies

```bash
pip install ursina
```

## Running the Game

1. Make sure your virtual environment is activated
2. Navigate to the project directory
3. Run the game:

```bash
python minecraft.py
```

## Controls

| Key | Action |
|-----|--------|
| W/A/S/D | Move forward/left/back/right |
| Mouse | Look around |
| Left Click | Place a block |
| Right Click | Destroy a block |
| Space | Jump |
| Shift | Descend (when flying) |
| Ctrl | Sprint |
| Escape | Pause/release mouse |

## Project Structure

```
minecraft/
├── minecraft.py    # Main game file
├── grass.png       # Block texture
└── README.md       # This file
```

## Asset

- `grass.png`: Texture used for the voxel blocks

## Troubleshooting

### Display Issues

If you encounter graphics issues:
1. Ensure your system has OpenGL support
2. Update your graphics drivers
3. Try running with software rendering if needed

### Permission Errors

If you get permission errors when creating the virtual environment:
```bash
python3 -m venv venv --clear
```

### Module Not Found

If Python cannot find the ursina module:
1. Verify your virtual environment is activated
2. Reinstall ursina: `pip install ursina --force-reinstall`

## License

This project is for educational purposes.


# Map Editor

![Map Editor Preview](images/preview.jpg)

A map editor for creating Tanki Online maps written from scratch with C++ and OpenGL.

## Features

- **3D Viewport** with intuitive camera controls
- **Prop Library System** for loading and placing map objects
- **Transform Tools** for moving, rotating, and scaling objects
- **Multi-selection** with rectangle selection and modifier keys
- **Undo/Redo History** for safe editing
- **XML Import/Export** compatible with Tanki map format
- **Texture Management** for props with multiple texture variants

## Quick Start

### Loading Assets

1. **Load Prop Libraries**: Click "Select path" in Library Browser and choose your prop libraries directory
2. **Import Maps**: Go to File → Import Map and select a `.xml` map file

Download prop libraries and maps from:
- [MapMakersAndProgrammers/tanki-prop-libraries](https://github.com/MapMakersAndProgrammers/tanki-prop-libraries)
- [MapMakersAndProgrammers/tanki-xml-maps](https://github.com/MapMakersAndProgrammers/tanki-xml-maps)

### Basic Usage

1. **Place Objects**: Double-click props in Library Browser to add them to the map (placed at origin)
2. **Select Objects**: Right-click objects in viewport or hold Shift for multi-select
3. **Move Objects**: Press `T` for translation mode and use the gizmo
4. **Rotate Objects**: Press `Z`/`X` for 90° Y-axis rotation or `R` for rotation mode
5. **Fine-tune**: Adjust properties in the Properties panel

## Controls

### Camera
- **Rotate**: Left-click + drag
- **Move**: `W` `A` `S` `D` keys
- **Up/Down**: `Q` / `E` keys
- **Speed Boost**: Hold `Shift` while moving

### Editing
- **Select Mode**: `V`
- **Translation Mode**: `T`
- **Rotation Mode**: `R`
- **Quick Rotate**: `Z` / `X` (90° around Y-axis)
- **Duplicate**: `Space`
- **Delete**: `Delete`
- **Deselect**: `Esc`

### Selection
- **Multi-select**: Hold `Shift` while right-clicking
- **Rectangle Select**: `Ctrl` + right-click drag (in Select Mode)
- **Add to Selection**: `Ctrl` + `Shift` + right-click drag (in Select Mode)

### History
- **Undo**: `Ctrl` + `Z`
- **Redo**: `Ctrl` + `Y`

### Transform Gizmo
- **Snap to Grid**: Hold `Ctrl` while dragging (250 units XZ, 300 units Y)
- **Adjust Values**: Click and drag in Properties panel
  - Default increment
  - `Shift`: Larger increment
  - `Alt`: Smaller increment
  - `Ctrl` + click: Enter exact value

### Manual

See the manual in `manual/` for additional hotkeys.

## Skyboxes

The library format is extended to support skyboxes. See `skyboxes/` for an example.

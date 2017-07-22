Tomb Raider SAT Blender plugin
=====

### About

Import all valid geometry from `.SAT` (Sega Saturn version of Tomb Raider).

![Blender](https://raw.githubusercontent.com/ijacquez/trsat/master/.images/level1.sat.png)

### TODO (need help)
 1. Document .SAT format completely
 2. Import calculated normals
 3. Import textures and map them to each face
 4. Import lighting

### Disassembly

Here is a list of functions inside the main binary (`0MAIN.BIN`)

- `0x060347A8` - Parses .SAT/.SPR files
- `0x06033C90` - Loads actual file `"data\\level3a.sat"` before parsing
- `0x060478A0` - String compare
- `0x060436E8` - Prints to console
- `0x06043A18` - Possibly loads files from CD
- `0x06043A70` - Possibly loads files from CD
- `0x0602C5AC` - HUGE function

### Installation

#### Windows
 1. Copy `io_import_trsat.py` to `%APPDATA%\Blender Foundation\Blender\2.XX\scripts\addons\` where `XX` is your version of Blender.

#### Unix
 1. Copy `io_import_trsat.py` to `~/.blender/scripts/addons/` where `XX` is your version of Blender.

 1. Open Blender, and press *Ctrl+Alt+U* to open the _Blender User Preferences_ window.
 2. Select the _Add-ons_ tab and search for _israel_
 3. Enable all addons
 4. Click on _Save User Settings_ button

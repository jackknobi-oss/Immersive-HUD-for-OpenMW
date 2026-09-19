# Immersive HUDHider for OpenMW

An OpenMW HUD modification that provides multiple HUD visibility modes while keeping important gameplay information available.

This mod is designed for OpenMW 0.51.0 and currently requires the included/custom OpenMW engine build.

## Features

Press **H** to cycle between three HUD modes:

1. **Full HUD**
   - Standard HUD elements are visible.

2. **Immersive HUD**
   - Most normal HUD elements are hidden.
   - The native OpenMW crosshair remains available.
   - Important contextual and scripted information remains visible.

3. **Hidden HUD**
   - Normal HUD elements are hidden for a cleaner and more cinematic view.
   - Important information messages and interactive message boxes remain available.

The mod is designed to preserve important gameplay information such as:

- World object tooltips
- Scripted notifications and message boxes
- Quest and gameplay messages
- Interactive message boxes

## Requirements

- Morrowind
- OpenMW 0.51.0
- The provided **Living Tamriel  OpenMW Engine Build**

The standard OpenMW 0.51.0 executable does not currently provide all engine-side functionality required by this mod.

**Mod Organizer 2 is NOT required.**

The mod can be installed with MO2 or manually.

---

# Installation

## Option 1 - Mod Organizer 2 (Recommended)

### 1. Install the mod

Install the `Immersive HUDHider for OpenMW - Main` mod archive through Mod Organizer 2 like a normal OpenMW mod.

The installed mod should contain approximately:

Living Tamriel - HUD Modes/
├── LivingTamrielHUDModes.omwscripts
├── scripts/
│   └── livingtamrielhudmodes/
│       └── player.lua
├── README.md
└── LICENSE

Do not move the Lua scripts into the OpenMW installation directory.

### 2. Install the custom OpenMW build

Extract the provided **Immersive HUDHider for OpenMW Engine Build** to its own folder.

For example:

C:\Games\OpenMW - Immersive HUDHider for OpenMW\

Do NOT copy individual files from the custom build into your normal OpenMW installation.

Keeping both OpenMW installations separate makes it much easier to return to the standard version.

### 3. Add the custom OpenMW executable to MO2

In Mod Organizer 2, add:

Binary:
C:\Games\OpenMW - Immersive HUDHider for OpenMW\openmw.exe

Start in:
C:\Games\OpenMW - Immersive HUDHider for OpenMW\

No special command-line arguments should be required.

Launch the game through this executable.

### 4. Enable the mod in OpenMW

Make sure the mod is present in your OpenMW data paths and that:

LivingTamrielHUDModes.omwscripts

is enabled as a content file.

---

# Manual Installation

You do NOT need Mod Organizer 2.

Do not copy the mod directly into `Morrowind\Data Files`.

Instead, create a separate mod directory.

Example:

C:\Games\OpenMW Mods\Immersive HUDHider for OpenMW\

Place the files so that the folder contains:

Immersive HUDHider for OpenMW/
├── LivingTamrielHUDModes.omwscripts
├── scripts/
│   └── livingtamrielhudmodes/
│       └── player.lua
├── README.md
└── LICENSE

Then add the mod directory to your OpenMW configuration.

On Windows, the default OpenMW configuration directory is usually:

Documents\My Games\OpenMW\

Open:

openmw.cfg

and add a data entry pointing to the mod folder:

data="C:\Games\OpenMW Mods\Immersive HUDHider for OpenMW"

Then enable the OpenMW Lua content file:

content=LivingTamrielHUDModes.omwscripts

The exact position of these entries may matter if you use a large mod setup with conflicting files.

## Install the custom engine

Extract the supplied OpenMW engine build into its own directory, for example:

Immersive HUDHider for OpenMW\

Run:

openmw.exe

from this folder.

Do not overwrite your existing OpenMW installation unless you specifically know what you are doing.

---

# Vortex

Vortex is not currently the primary supported installation method.

The mod itself does not require MO2, but OpenMW uses its own system of `data=` paths and content files rather than relying on the original Morrowind `Data Files` directory alone.

If using Vortex, make sure that the final mod folder is added to OpenMW as a data directory and that:

LivingTamrielHUDModes.omwscripts

is enabled as an OpenMW content file.

Do not assume that deploying the files into `Morrowind\Data Files` is sufficient.

More streamlined compatibility and installation options for other mod managers are planned.

---

# Usage

Press:

H

to cycle through the available HUD modes.

The current mode should change immediately.

The mod intentionally keeps important contextual and scripted information available even when the normal HUD is hidden.

---

# F11 / Toggle HUD

OpenMW's native **Toggle HUD** function is separate from the HUD mode system provided by this mod.

The current release has a known limitation:

When the native OpenMW HUD toggle is used to hide the HUD, some information elements that this mod deliberately keeps persistent may remain visible.

This behavior is planned to be improved in an upcoming update.

---

# Compatibility

This mod changes HUD behavior at both the Lua and OpenMW engine level.

Simple compatibility patches and additional compatibility options are planned for future releases.

HUD mods that modify the same visibility behavior may conflict with Immersive HUDHider for OpenMW.

Mods that only change textures, icons, fonts, HUD positioning or visual styling may work normally, depending on what they modify.

Compatibility testing will be expanded over time.

If you find a conflict, please report:

- The conflicting mod
- Your OpenMW version
- Your mod manager
- What HUD mode was active
- What you expected to happen
- What actually happened

---

# Planned Updates

This is an early release and active development is continuing.

Planned updates include:

- Improved interaction with OpenMW's native F11 / Toggle HUD function
- Easier installation
- Additional compatibility options
- Simple compatibility patches for popular HUD and interface mods
- Further testing with larger OpenMW mod lists
- Documentation improvements

The current release is intended to provide a functional foundation rather than the final version of the HUD system.

---

# Uninstallation

Remove or disable:

LivingTamrielHUDModes.omwscripts

and remove the mod's data directory from your OpenMW configuration.

If you installed the custom OpenMW build in a separate directory, simply switch back to your normal OpenMW executable.

The mod does not require replacing your original Morrowind files.

---

# AI Assistance

Parts of the development, documentation and build process for Immersive HUDHider for OpenMW were created with AI assistance.

The mod has been manually tested in-game.

---

# Credits

Immersive HUDHider for OpenMW

Built for OpenMW 0.51.0.

OpenMW is a separate open-source project and is not affiliated with this mod.

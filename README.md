<p align="center"><img src="assets/images/SwarmConstructionLogo.png" width="600" >
<br>
<br>

</div>

[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/XenonLab-Studio/TerraCraft/graphs/commit-activity)
[![GPLv3 license](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0.en.html)

---

# Swarm Construction Blueprint Creator

This code is used to create a simple means to create new blueprints for Swarm Construction. A Minecraft-like environment is displayed wherein users can add or remove smart blocks to create blueprints. These blueprints, saved as numpy .npy files (by hitting P on the keyboard) can be read by the Swarm Construction simulator to be simulated with. Follow the instructions below for learning the controls to use the Blueprint Creator.

A large portion of this code was created for gaming purposes and made by Xenon Lab Studios (Michael Fogleman and Stefano Peris). All credit belongs to them for all borrowed code. Please see their [README](https://github.com/XenonLab-Studio/TerraCraft/blob/master/README.md) and repo for their intentions with this project. All code in this project is used for educational purposes under their GNU General Public License.

### How to Run

First, edit the file_config.py file to change the parameter location_to_save. This is the location that the numpy blueprint files will be saved to. This is provided to easily move the files to the correct location.

Once the config file has been set, run the following commands:

```shell
pip install requirements.txt
python main.py
```

### Mac

On Mac OS X, you may have an issue with running Pyglet in 64-bit mode. Try running Python in 32-bit mode first:

```shell
arch -i386 python3 main.py
```

If that doesn't work, set Python to run in 32-bit mode by default:

```shell
defaults write com.apple.versioner.python Prefer-32-Bit -bool yes
```

This assumes you are using the OS X default Python. Works on Lion 10.7 with the default Python 3.5+, and may work on other versions too. Please raise an issue if not.
<br/>

## Controls:

### Moving

- P: Save current blueprint
- H: Show a help menu with all of the commands
- W: forward
- S: back
- A: strafe left
- D: strafe right
- Mouse: look around
- Space: Move up

- ESC: release mouse, then close window

### Building

- Selecting type of block to create:
  - 0-9: Select color of block to be used
  - Mouse left-click: remove block
  - Mouse right-click: create block

**Warning! By pressing F12, the previous screenshot is automatically overwritten.**

### Quitting

- ESC: release mouse, then close window

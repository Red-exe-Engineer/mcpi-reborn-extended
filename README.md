# MCPI++ (mcpi-reborn-extended)
This is a fork of [mcpi-reborn](https://gitea.thebrokenrail.com/TheBrokenRail/minecraft-pi-reborn), with custom features added by community members. The apt packages and repo info are stored in the [debs](debs/) folder. The project is UNOFFICIAL from mcpi-reborn. If you like MCPI or MCPI-Reborn, you'll probably like this too!

[![Discord](https://badgen.net/badge/icon/discord?icon=discord&label=Get%20support%20on)](https://discord.gg/XJJNG9jTuh)

![image](screenshot.png)

Source code and documentation is in the [source](https://github.com/NoozSBC/mcpi-reborn-extended/tree/source) branch.

## Installation ([compatibility list](https://github.com/NoozSBC/mcpi-reborn-extended#compatibility))

### Method 1 - Install Script
This method only supports debian-based distros with APT. This method will also add sound support. 
```bash
wget -qO- https://raw.githubusercontent.com/mobilegmYT/mcpi-reborn-extended/main/install.sh | bash
```

#### Uninstall (if you used the script)
```bash
wget -qO- https://raw.githubusercontent.com/mobilegmYT/mcpi-reborn-extended/main/uninstall.sh | bash
```

### Method 2 - DEB Install
This script only supports debian-based distros with APT. This method will also add sound support. 
Download and install the appropiate DEB for your architecture with the `client` tag from [here](https://github.com/mobilegmYT/mcpi-reborn-extended/tree/main/debs)

### Method 3 - AppImage
Download and run the appropiate AppImage for your architecture with the `client` tag from [here](https://github.com/mobilegmYT/mcpi-reborn-extended/releases/). This is the only method that works on non-debian distros like arch or fedora.

## Feature List (in order of awesomeness)
- Supports all distros with glibc (most major distros except musl-based ones like Alpine)
- Working sound
- Add missing items in creative inventory
- Sprinting via `CTRL` key
- Modern textures
- Custom skins
- Longer chat message length limit (512 characters)
- Longer username length limit (32 characters)
- Add item names for some hidden items (like the camera)
- Sneaking via both the `Shift` and `Alt` keys
- A custom "[Cursed Chest](https://media.discordapp.net/attachments/761048906242981948/903080546182242344/2021-10-27_20.39.05.png)" block for debugging
- Ability to look around via arrow keys instead of mouse (useful if mouse is glitched)
- [Colored](https://upww.screenrec.com/images/f_PX5iWMcfs6KLjEyqvmtU10Ozwogl4r3C.png) terminal output
- Use basic Vim keybindings for movement (hjkl)

## Compatibility
MCPI++ has been tested with the following:
- Raspberry Pi 3/4 running RPI OS Buster/Bullseye
- Windows 10/11 via WSL2 and GWSL (instructions [here](https://www.youtube.com/watch?v=3l-m8O13LYk))
- x64 PC running Debian/Ubuntu

## User guide
### Starting the game
If you didn't choose to install the launcher, launch with `minecraft-pi-reborn-client` and configure your features. Otherwise, type `planet-launcher` into terminal or find `Planet Launcher` from your start menu. You will be greeted with the launcher, from which you can configure settings like username, control which mods are enabled, and add servers. Once you are done, hit "Launch" and start the game!

### Controls
Once you are in a world, you will be able to move with WASD and Space.  
You can look around with the mouse or arrow keys.  
To look in your inventory use the "E" and to scroll use the mouse to drag.  
To pause the game press Esc.  
To sneak press Shift or Alt.  
To sprint hold Ctrl and move.  

### Entering a game
Press "Start Game", then click "Create new" to make a new world. Once you load in, you can play around and do whatever. Pause the game with ESC and you can mute sounds or return to the main menu. To enter that world again, click "Start Game" and click on the picture for that world. 

#### Joining a server
Press "Join Game", and you will be greeted with a list of available servers. Click on one and it will connect. Playing on servers is the exact same as playing on multiplayer, except pausing won't pause the game for other people online and of course, there will be other players online who will all have the same skin as you.

### Installing extra mods.
MCPI mods are compiled into shared objects (also called "so files") to add them move them to `~/.minecraft-pi/mods/lib<modname>.so`.
If you are interested in making your own mods, documentation can be found [here](https://github.com/mobilegmYT/mcpi-reborn-extended/blob/source/docs/MODDING.md).

## Troubleshooting
- My mouse sensetivity is really high
- - If on WSL --> Follow this [tutorial](https://www.youtube.com/watch?v=3l-m8O13LYk)
- - If on bare metal Linux --> Uncheck `Disable Raw Mouse Motion` launch flag

## Credits
- Maintained by [mobilegmYT](https://github.com/mobilegmYT).
- Patches/mods by [Bigjango13](https://github.com/bigjango13) and [TheBrokenRail](https://github.com/TheBrokenRail).
- Vanilla Reborn by [TheBrokenRail](https://github.com/TheBrokenRail).
- Minecraft: Pi Edition by Mojang AB.

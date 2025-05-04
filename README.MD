# X360CE - Xbox 360 Controller Emulator

[![Build Status](https://img.shields.io/github/workflow/status/X-android-pixel/x360ce/build/main)](https://github.com/X-android-pixel/x360ce/actions)
[![Latest Release](https://img.shields.io/github/v/release/X-android-pixel/x360ce?include_prereleases)](https://github.com/X-android-pixel/x360ce/releases)
[![License](https://img.shields.io/github/license/x360ce/x360ce)](https://github.com/x360ce/x360ce/blob/master/LICENSE)

## About This Fork

This repository is a fork of the [original X360CE project](https://github.com/x360ce/x360ce). The main purpose of this fork is to **provide automated builds** of the project, making it easier for users to download and use without having to compile the code themselves.

**Key benefits:**
- Automated builds via GitHub Actions
- Regular updates from the upstream repository
- Direct download links for the latest builds
- All the functionality of the original project

## What is X360CE?

"Xbox 360 Controller Emulator" allows your controller (gamepad, joystick, wheel, etc.) to function as an Xbox 360 controller. For example, it lets you play games such as "Grand Theft Auto" (GTA) or "Mafia II" using a Logitech Wheel.

## ⚠️ Important Security Notice

Please download and run **digitally signed files only**! If someone asks you to disable your antivirus or exclude X360CE from anti-virus scanning - **DON'T DO IT!** Report any suspicious behavior in the [Issues](https://github.com/YOUR_USERNAME/x360ce/issues) section.

## Downloads

### Version 4.x (Latest)

Supports all games with Virtual Gamepad Emulation Bus

[⬇️ Download Latest x360ce v4.x](https://github.com/YOUR_USERNAME/x360ce/releases/latest)

### Version 3.x (Legacy)

#### For 32-bit Games
[⬇️ Download x360ce_x86.zip](https://github.com/YOUR_USERNAME/x360ce/releases/latest/download/x360ce_x86.zip)

#### For 64-bit Games
[⬇️ Download x360ce_x64.zip](https://github.com/YOUR_USERNAME/x360ce/releases/latest/download/x360ce_x64.zip)

#### DInput.dll Plugin (required for some games)
- [32-bit Download - dinput_x86.dll](https://github.com/YOUR_USERNAME/x360ce/releases/latest/download/dinput_x86.dll)
- [64-bit Download - dinput_x64.dll](https://github.com/YOUR_USERNAME/x360ce/releases/latest/download/dinput_x64.dll)

## System Requirements

1. Windows Vista or newer
2. [.NET 3.5 (also installs 2.0 and 3.0)](http://www.microsoft.com/en-us/download/details.aspx?id=22) (included in Windows 7)
3. [.NET 4.0 or higher](http://www.microsoft.com/en-us/download/details.aspx?id=48130) (included in Windows 8 and 10)
4. [DirectX End-User Runtime (June 2010)](http://www.microsoft.com/en-us/download/details.aspx?id=8109) (required regardless of OS)
5. [Visual C++ Redistributable for Visual Studio 2013](http://www.microsoft.com/en-us/download/details.aspx?id=40784) (**for x64 systems install both x86 and x64 redistributables**)
6. If you upgraded to Windows 10/11, you must Uninstall and Reinstall the Visual C++ Redistributable

## Quick Installation Guide

1. Download the appropriate version for your game (32-bit or 64-bit)
2. Extract the files to your game's main directory (where the game executable is located)
3. Run x360ce.exe and configure your controller
4. Play your game with your controller

## Detailed Installation

Run this program from the same directory as the game executable. XInput library files exist with several different names, and some games require a change in its name. Known names:

* xinput1_4.dll (Windows 8/10/11 / metro apps)
* xinput1_3.dll
* xinput1_2.dll
* xinput1_1.dll
* xinput9_1_0.dll

Game Database (GDB) and Configuration (INI) files can be stored in:
- Same directory as the game's executable (.EXE)
- `%ALLUSERSPROFILE%\X360CE` on Windows Vista/7/8/10/11
- `%ALLUSERSPROFILE%\Application Data\X360CE` on Windows XP

**Note:** In games based on the Source engine, place the DLL inside the `/Bin/` sub-folder.

## Troubleshooting

### Controller Not Working in Game

**Solution 1: Try setting device as GamePad**
1. Run x360ce.exe
2. Select the [Controller #] tab corresponding to your controller
3. Open [Advanced] tab
4. Set "Device Type" to: GamePad
5. Save and close x360ce.exe
6. Run the game

**Solution 2: Map controller to PAD1**
1. Run x360ce.exe
2. Select the [Controller #] tab for your controller
3. Open [Direct Input Device] tab
4. Set "Map To" to: 1
5. For additional controllers, set them to 2, 3, or 4
6. Save, close x360ce.exe, and run the game

**Solution 3: Adjust Dead Zone settings**
- Some games have control issues when Dead Zone is reduced to 0%
- Try increasing the Anti-Dead Zone value if there's a delay between input and reaction

### Emergency HID Guardian Removal

If you lose access to your Mouse and Keyboard when using X360CE v4.x, follow these instructions:
[HID Guardian Removal Guide](https://github.com/x360ce/x360ce/wiki/HID-Guardian)

## Game Compatibility

For a list of compatible games, see the [Compatibility List](https://github.com/x360ce/x360ce/wiki/Compatibility-List).

## Need Help?

For installation or configuration help, please visit the [X360CE forum on NGemu](http://ngemu.com/forums/x360ce.140).

## Screenshots

![X360CE Interface](http://www.jocys.com/projects/x360ce/Images/x360ce_General.png)

## Credits
* Original X360CE Team
* ThreeDeejay for `build.yml`
* YOUR_USERNAME for maintaining this fork

## License

This project is licensed under the [MIT License](https://github.com/x360ce/x360ce/blob/master/LICENSE).

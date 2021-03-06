![logo](/img/ogMountUp.png)

# Mount Up!
**Mount Up!** is a module for [Foundry VTT](https://foundryvtt.com/  "Foundry VTT") that allows tokens to carry or be carried by other tokens. This is completely system agnostic, and fully customizable to fit right into your game.

![GitHub release (latest by date)](https://img.shields.io/github/v/release/brunhine/mountup?style=flat-square)
![GitHub latest version downloads](https://img.shields.io/github/downloads/brunhine/mountup/latest/total?style=flat-square)

[![Twitter Follow](https://img.shields.io/badge/follow-%40Brunhine-blue.svg?style=flat-square&logo=twitter)](https://twitter.com/brunhine)
[![Become a Patron](https://img.shields.io/badge/support-patreon-orange.svg?style=flat-square&logo=patreon)](https://www.patreon.com/brunhine)
[![Donate via Ko-Fi](https://img.shields.io/badge/support-ko--fi-ff4646?style=flat-square&logo=ko-fi)](https://ko-fi.com/brunhine)

# Installation
It's always better and easier to install modules through in in app browser. Just search for "Mount Up!"

To install this module manually:
1. Inside the Foundry "Configuration and Setup" screen, click "Add-on Modules"
2. Click "Install Module"
3. In the "Manifest URL" field, paste the following url:
`https://raw.githubusercontent.com/Brunhine/MountUp/master/src/module.json`
4. Click 'Install' and wait for installation to complete
5. Don't forget to enable the module in game using the "Manage Module" button

# Localization
Japanese Language support provided by [BrotherSharper](https://github.com/BrotherSharper) ('Brother Sharp#6921' on discord)

*always welcoming more translations*

# Usage
*In this example, we will be using a rider and a mount and rider scenario, but this could be anything like driving or carrying. You can even change the icons used by the module to fit your game.*

## Mounting
To mount a token:
1. Select the "rider" and the "mount" tokens.
2. Right click on the "mount" icon to bring up the token HUD.
3. Click on the horse icon (you can change this in your game).\
![mount example](/examples/mount-example.webm)\
*The rider will now be linked to the mount. Anywhere the mount moves, the rider follows.*

## Dismounting
To dismount a token from a token:
1. Right click on the "mount" to bring up the token HUD.
2. Click on the dismount icon.\
![dismount example](/examples/dismount-example.webm)\
*The rider will now be un-linked from the mount, and is free to move on their own.*

## Macros
Some functionality is exposed to macros for repeatable usage. All macros will either accept a token ID or name (case insensitive).

#### Mounting
You can mount a rider to a mount using the following syntax:
`MountUp.mount('RiderNameOrId', 'MountNameOrId')`

### Dismounting
You can have a rider dismount by passing it's token name or id:
`MountUp.dismount('RiderNameOrId)`

### Drop a rider from a mount
You can have a mount drop its rider by passing the mount's name or id:
`MountUp.dropRider('MountNameOrId')`

# Compatibility
Most recently tested on [Foundry VTT](https://foundryvtt.com/  "Foundry VTT") version `0.6.0`.

# Feedback
All feedback and suggestions are welcome. Please contact me on Discord (Brunhine#2182).

Any issues, bugs, or feature requests are always welcome to be reported directly to the [Issue Tracker]([https://gitlab.com/brunhine/foundry-mountup/-/issues](https://gitlab.com/brunhine/foundry-mountup/-/issues)  "Issue Tracker")

# Licensing
**Mount Up!** is a module for [Foundry VTT](https://foundryvtt.com/  "Foundry VTT") by Jeremiah Altepeter and is licensed under a [Creative Commons Attribution 4.0 International License](http://creativecommons.org/licenses/by/4.0/).

This work is licensed under Foundry Virtual Tabletop [EULA - Limited License Agreement for module development v 0.1.6](https://foundryvtt.com/article/license/).

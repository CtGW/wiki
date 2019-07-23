---
title: Main modding
description: The brunt of the modding, where we focus on adding mods
published: 1
date: 2019-07-23T20:33:49.832Z
tags: 
---

# Main modding
## Choosing ESL or not
> 
> **TLDR**: When given a choice of choosing an ESP or an ESL you should always download the ESP and then manually mark it as an ESL in FO4Edit.
> 
{.is-info}

For an in-depth understanding: https://www.afkmods.com/index.php?/topic/5079-plugin-files-and-you-esmeslesp/
Another nice explanation: https://steamcommunity.com/app/489830/discussions/0/3276824488728505237/

We outline a small summary:

### How ESLs work

Firstly, lets remember that the Bethesda engine allows loading 255 plugins in total.
Each plugin occupies a namespace, `xx`, for its load order, where a general element is represented by: `xx123456`

So, in theory, any plugin can add <code>16<sup>6</sup></code> new items, though in reality the number is a bit smaller.

ESLs work by sharing the `FE` namespace, so that an element in the plugin looks like `FEyyyyyy`.
The first ESL has the plugin FormIDs as: `FE000zzz`, the second ESL has FormIDs as: `FE001zzz`, so on and so forth.

So in theory, you cannot have more than <code>16<sup>3</sup></code> ESL plugins in your modlist, each of which can only introduce another <code>16<sup>3</sup></code> new items/elements.

### ESL vs ESP
.esl plugins are loaded in the master space and is termed as a *light master*, as internally the bethesda engine makes every .esl 
This means that they are loaded before the other files and they can mess up your load order.

On the other hand, if you use an .esp marked as an ESL in FO4Edit, the plugin respects your load order.

So whenever there is an option, always choose the ESP file instead of the ESL file and then you can decide if you want to make it into and ESL or not.

---

## Core mods

##### [F4SE](https://f4se.silverlock.org/) 
Brose install file manually and install only data folder. This way we can more easily
determine if any of the scripts are overwritten by later mods.

##### [PrivateProfileRedirector F4](https://www.nexusmods.com/fallout4/mods/33947)
Speeds up game start by storing INI files in memory instead of opening, parsing and closing the file
each time some value from it is needed.

##### [Unofficial Fallout 4 Patch](https://www.nexusmods.com/fallout4/mods/4598)
Fixes things Bethesda won ́t. Drag esp to just after esm-files.

##### [Mod Configuration Menu](https://www.nexusmods.com/fallout4/mods/21497)

##### [Game Configuration Menu](https://www.nexusmods.com/fallout4/mods/33759)
GCM allows you easily set many game settings, like game difficulty, skills, XP, quests etc,
without the need of additional ESPs or console commands. Install both main file.

##### [Armor and Weapon Keywords Community (AWKCR)](https://www.nexusmods.com/fallout4/mods/6091)
Make sure to ticket the CBBE patch option during the installer

##### [Armorsmith Extended](https://www.nexusmods.com/fallout4/mods/2228)
Install main file

## Minor fixes

##### [CCCleaner](https://www.nexusmods.com/fallout4/mods/26592)

##### [Achievements](https://www.nexusmods.com/fallout4/mods/12465)
Uses F4SE to re-enable achievements while mods are active

##### [RAW INPUT - The Ultimate Mouse Sensitivity Fix](https://www.nexusmods.com/fallout4/mods/27019)
Disabled Mouse Acceleration, Horizontal/Vertical Parity, Scalable ADS Multiplier, Normalized Sensitivity

##### [Simple Trashcan fix](https://www.nexusmods.com/fallout4/mods/14707/)
One of those small fixes you can only truly appreciate if you suffer from OCD...

##### [Wetness shader fix](https://www.nexusmods.com/fallout4/mods/23389)

##### [Eye Normal Map Fix](https://www.nexusmods.com/fallout4/mods/819)

##### [Far Harbor Doctor Dialogue Fix](https://www.nexusmods.com/fallout4/mods/16274)

##### [Search and Destroy Fixed](https://www.nexusmods.com/fallout4/mods/33127)

##### [Lever Action Reload Fix](https://www.nexusmods.com/fallout4/mods/22896)

##### [Overboss Power Armor headlamp fix](https://www.nexusmods.com/fallout4/mods/19295)

##### [Mechanist's Lair - expanded corrected and fixed](https://www.nexusmods.com/fallout4/mods/11490)

##### [Perception Bug Fix](https://www.nexusmods.com/fallout4/mods/35376)

##### [Protectron Subway Steward (fix)](https://www.nexusmods.com/fallout4/mods/22022)

##### [Alex's Male First Person Camera Height Fix](https://www.nexusmods.com/fallout4/mods/27582)
Adjusts the eyeheight in first person if you play as a male character.

##### [Vault 111 Floor Guide Fix](https://www.nexusmods.com/fallout4/mods/28167)

##### [Starlight Drive In LOD Fix with ESL](https://www.nexusmods.com/fallout4/mods/23034)

##### [NukaWorld Transit Center LOD Fix with ESL](https://www.nexusmods.com/fallout4/mods/30925)

##### [Vault111 And Billboard LOD Fix](https://www.nexusmods.com/fallout4/mods/36288)

##### [Sanctuary Bridge LOD Fix](https://www.nexusmods.com/fallout4/mods/36288)

##### [Far Harbor Bed Fix](https://www.nexusmods.com/fallout4/mods/34504)

##### [Hardware Town Key Havok Fix](https://www.nexusmods.com/fallout4/mods/34497)

##### [Nuka Cola Storage Rack](https://www.nexusmods.com/fallout4/mods/24909)

##### [Space Sentry Leg Fix](https://www.nexusmods.com/fallout4/mods/29869)

##### [Vault Door FIXED](https://www.nexusmods.com/fallout4/mods/24954)

##### [Blood Pack Mesh Fix](https://www.nexusmods.com/fallout4/mods/25800)

##### [Fixed Gobo Effects](https://www.nexusmods.com/fallout4/mods/27445)

##### [Plasma Impact Fix](https://www.nexusmods.com/fallout4/mods/25412)

##### [Doorway Endcap Fix](https://www.nexusmods.com/fallout4/mods/35818)

##### [Flicker fixer](https://www.nexusmods.com/fallout4/mods/35720)

##### [BiRaitBec ́s merged Fixes](https://www.nexusmods.com/fallout4/mods/23556)


## Misc tweaks

##### []()

## Camera and UI

##### []()

## Settlements

##### []()

## Cosmetic overhauls

##### []()

## Clothing

##### []()

## Armor

##### []()

## Power armor

##### []()

## Weapons of lore

##### []()

## Gameplay

##### []()

## NPC and creature overhauls

##### []()

## Companion overhauls

##### []()

## New companions

##### []()

## Animations

##### []()

## Vanilla location overhauls

##### []()

## New quests and locations

##### []()

## Weather and environment

##### []()

## Audio overhauls

##### []()

## Cut content restored

##### []()

## Late loaders

##### []()

## Rounding up

##### []()

## Dead last (conflict resolutions)

##### []()

---
title: Main modding
description: The brunt of the modding, where we focus on adding mods
published: 1
date: 2019-07-23T22:06:49.778Z
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

##### [No Quest Autostart - BoS Fire Support](https://www.nexusmods.com/fallout4/mods/31563)

##### [No Quest Autostart - Far Harbor](https://www.nexusmods.com/fallout4/mods/31450)

##### [No Quest Autostart - Nuka World](https://www.nexusmods.com/fallout4/mods/31433)

##### [No Quest Autostart – Automatron](https://www.nexusmods.com/fallout4/mods/31576)

##### [No Quest Autostart – Vault-Tec](https://www.nexusmods.com/fallout4/mods/31454)

##### [Recruiter Radio Freedom](https://www.nexusmods.com/fallout4/mods/14762)

##### [Corpse Collision](https://www.nexusmods.com/fallout4/mods/37133)

##### [Realistic Death Physics - No Animations](https://www.nexusmods.com/fallout4/mods/4371)

##### [Remove Interior Fog](https://www.nexusmods.com/fallout4/mods/2628)

##### [Realistic conversations](https://www.nexusmods.com/fallout4/mods/32514)

##### [Immersive Generic Dialogue](https://www.nexusmods.com/fallout4/mods/14108)

##### [Icebreaker Settlements – Settler Dialogue Overhaul](https://www.nexusmods.com/fallout4/mods/25972)

##### [Icebreaker - Piper - Companion Dialogue Overhaul](https://www.nexusmods.com/fallout4/mods/25525)

##### [Settler Sandbox](https://www.nexusmods.com/fallout4/mods/20442/)

##### [Locky bastard](https://www.nexusmods.com/fallout4/mods/13380/)

##### [First Person messages](https://www.nexusmods.com/fallout4/mods/10870)

##### [Quest Summary by Default](https://www.nexusmods.com/fallout4/mods/2664)

##### [Puddle remover plus](https://www.nexusmods.com/fallout4/mods/34035)

##### [R2K fast pipboy](https://www.nexusmods.com/fallout4/mods/17777)

##### [Not So Bright Pins](https://www.nexusmods.com/fallout4/mods/35097)

##### [Swinging Animated Meat Bags](https://www.nexusmods.com/fallout4/mods/21087)

##### [Tougher Cars Durable Vehicles](https://www.nexusmods.com/fallout4/mods/3680)

##### [Lootable vendors](https://www.nexusmods.com/fallout4/mods/34960)

##### [ExitSave Killer](https://www.nexusmods.com/fallout4/mods/18102)

## Camera and UI

##### [DEF_UI](https://www.nexusmods.com/fallout4/mods/10654)

##### [DEF_UI Iconlibs Rescaled and Fixed](https://www.nexusmods.com/fallout4/mods/31088/)

##### [Extended Dialogue Interface](https://www.nexusmods.com/fallout4/mods/27216)

##### [HUDFramework](https://www.nexusmods.com/fallout4/mods/20309)

##### [Power Armor HoloHUD](https://www.nexusmods.com/fallout4/mods/29969)

##### [HUD Plus Plus](https://www.nexusmods.com/fallout4/mods/27218)

##### [ApeHUD](https://www.nexusmods.com/fallout4/mods/30294)

##### [Immersive HUD](https://www.nexusmods.com/fallout4/mods/20830)

##### [Ruddy88 ́s Simple Sorter](https://www.nexusmods.com/fallout4/mods/33983)

##### [Clock Widget - Show Real Time While Loading](https://www.nexusmods.com/fallout4/mods/26759)

##### [Satellite Color World Map Combo](https://www.nexusmods.com/fallout4/mods/9414)

##### [Crafting Highlight Fix](https://www.nexusmods.com/fallout4/mods/27479)

##### [No more hold v to enter workshop](https://www.nexusmods.com/fallout4/mods/19996)

##### [Loading Screen Spoiler Remover](https://www.nexusmods.com/fallout4/mods/30594)

## Settlements

##### [Workshop Framework](https://www.nexusmods.com/fallout4/mods/35004)

##### [Workshop Plus](https://www.nexusmods.com/fallout4/mods/35005)

##### [All Setlements Extended](https://www.nexusmods.com/fallout4/mods/25316?tab=description)

##### [Uncapped Settlement Surplus](https://www.nexusmods.com/fallout4/mods/12430)

##### [Faster Workshop (Workshop Lag Fix)](https://www.nexusmods.com/fallout4/mods/35382)

##### [Quieter settlements](https://www.nexusmods.com/fallout4/mods/2819)

##### [Locksmith](https://www.nexusmods.com/fallout4/mods/12454)

##### [Basement Living](https://www.nexusmods.com/fallout4/mods/10967)

##### [Basement Living-Immersion Adjustment](https://www.nexusmods.com/fallout4/mods/28942)

##### [The Master Plan](https://www.nexusmods.com/fallout4/mods/16626)

##### [Vanilla Extensions](https://www.nexusmods.com/fallout4/mods/10032)

##### [This is MY Bed](https://www.nexusmods.com/fallout4/mods/7399)

##### [Better Cooking Stations](https://www.nexusmods.com/fallout4/mods/12104)

##### [PWR - Passive Water Resources](https://www.nexusmods.com/fallout4/mods/19871)

##### [CWSS Redux]()

##### [Lore Friendly Posters]()

##### [Workshop Rearranged]()

##### [Master Plan WRA Patch]()

##### [Better Stores]()

##### [Better Vendor Stalls]()

##### [Manufacturing Extended]()

##### [Thematic and Practical]()

##### [Creative clutter]()

##### [Do It Yourshelf]()

##### [Gruffydds Signs and Posters]()

##### [g2m Workshop]()

##### [Organized Workbench Menu]()

##### [JP Guard Towers]()

##### [Woody's Wasteland Stuff]()

##### [Private Area Markers (keep settlers out of your house)]()

##### [Timer Power Switch]()

##### [Weapon Rack Extended]()

##### [Weapon Rack Fixes]()

##### [Settlement Objects Combined]()

##### [Settlement Tidy bot]()

##### [Settlement Menu Manager]()

##### [Sim Settlements]()

##### [Sim Settlements Mega Pack - Year One]()

##### [Sim Settlements Mega Pack - Year Two]()

##### [Sim Settlements – Conqueror]()

##### [Sim Settlements Conqueror Faction Pack - The Forsaken Vaulters]()

##### [Sim Settlements - Building Plan Preview]()

##### [Sim Settlements - IDEK's Logistics Station]()

##### [Wasteland Venturers 2 All-In-One]()

##### [Place Everywhere]()

## Cosmetic overhauls

##### []()

##### []()

##### []()

##### []()

##### []()

##### []()

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

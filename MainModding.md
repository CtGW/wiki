---
title: Main modding
description: The brunt of the modding, where we focus on adding mods
published: 1
date: 2019-07-23T22:34:45.634Z
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

A UI better suited for PC (Hear that Bethesda?)
install both main files in order, use same name for both during manual install and choose
merge.
During Installation of first file select:
- DEF_HUD
- DEF_INV
- Language and Screen Ratio based on your preferences
- Do NOT install component tags and Vanilla Hud
- i already have sorting xml files option
After the second file is merged, use right-click Open in Explorer and delete any Translate_%%.txt
files in the \Interface folder. If $CREATION CLUB appears on the main menu, you've missed this
step.

##### [DEF_UI Iconlibs Rescaled and Fixed](https://www.nexusmods.com/fallout4/mods/31088/)
Based on Updated ICONLIBS2 for DEF_UI by omega9380. Aims to bring consistency in
design and coloring to the icon library. Also fixes various issues with icon sizes, bounding
boxes and scaling.
Install the subtle color main file.
For the colors to work, a couple of changes need to be made to fallout4custom.ini
```
[Pipboy]
bPipboyDisableFX=1
fPAEffectColorR=1
fPAEffectColorG=1
fPAEffectColorB=1

[Interface]
iHUDColorR=255
iHUDColorG=255
iHUDColorB=255

[Display]
fPipboyScreenEmitIntensityPA=1
fPipboyScreenDiffuseIntensityPA=0
```
If those values are already present, override them. Otherwise just add them in the
appropriate section.

##### [Extended Dialogue Interface](https://www.nexusmods.com/fallout4/mods/27216)
Displays full dialogue, and adds engine support for any number of player dialogue options.
Contains and ESM, which MO2 won ́t automatically put in the correct place. Drag manually
up in the right pane to the other ESMs.

##### [HUDFramework](https://www.nexusmods.com/fallout4/mods/20309)
a UI framework that makes it possible for mods to add new UI elements to the HUD
Install main file only

##### [Power Armor HoloHUD](https://www.nexusmods.com/fallout4/mods/29969)
A slicker Powerarmor HUD.

##### [HUD Plus Plus](https://www.nexusmods.com/fallout4/mods/27218)

##### [ApeHUD](https://www.nexusmods.com/fallout4/mods/30294)
In CtGW main archive there are two version:
- standard – some UI elements removed and the rest resized and move towards the edge of the screen
- lean – same as above but also compass, enemy health and notifications turned off

##### [Immersive HUD](https://www.nexusmods.com/fallout4/mods/20830)
A hud that gets out of the way when you don ́t need it.

##### [Ruddy88 ́s Simple Sorter](https://www.nexusmods.com/fallout4/mods/33983)
an alternative to VIS which is less flexible but much easier to work with, as it
patches the whole list for you, without any need for extra patches.
Go to the RSS files and first download R88SimpleSorter_SCRIPT. Extract the file menu
manually into your F04edit folder.
Now download MXPF - Mator's xEdit Patching Framework, and repeat the process from
above.
Next, install in MO2 R88SimpleSorter_XML.
Finally, we will do the actual patching. Note that it ́s recommended that you deactivate all
plugins related to Sim Settlements in the right pane before starting the patching process.

1. Open FO4Edit, and click OK. Holdiing shift while clicking ok will load the program quicker. Wait for thr background loader to finish.
2. Right-click on any of the plugins in the left pane and select "Apply Script".
3. In the Apply Script dialogue, click in the script box and navigate to R88_SimpleSorter. Click OK.
4. In the first dialogue box, check your options as below:
5. Click on New Patch. You can name your sorting file whatever you want, I name it CtGW – simple sorter
6. Let the sorter do it ́s job (which only takes a couple of minutes on my rig. When it ́s done, you will get a popup message saying "Patching Complete".
7. Close FO4Edit, make sure your new plugin is selected.
8. Put your newly created patch last in the right pane of MO2. We ́re done

##### [Clock Widget - Show Real Time While Loading](https://www.nexusmods.com/fallout4/mods/26759)
You can change setting in ClockWidget.ini to toggle on/off 24-hour clock, by changing the
value of iEnable24HourClock=1 to 0.

##### [Satellite Color World Map Combo](https://www.nexusmods.com/fallout4/mods/9414)
During installer choose:

- No Special

Also install maps for Nuka-World and Far harbor and Zoom-out Extended (half-sized
markers) and make sure to merge them with the main mod. I had issues when installing
them as separate mods for some reason.

##### [Crafting Highlight Fix](https://www.nexusmods.com/fallout4/mods/27479)

##### [No more hold v to enter workshop](https://www.nexusmods.com/fallout4/mods/19996)

##### [Loading Screen Spoiler Remover](https://www.nexusmods.com/fallout4/mods/30594)

## Settlements

##### [Workshop Framework](https://www.nexusmods.com/fallout4/mods/35004)

##### [Workshop Plus](https://www.nexusmods.com/fallout4/mods/35005)

##### [All Setlements Extended](https://www.nexusmods.com/fallout4/mods/25316?tab=description)
Download and install No Bunker Hill or Hangman's Alley main version

##### [Uncapped Settlement Surplus](https://www.nexusmods.com/fallout4/mods/12430)

##### [Faster Workshop (Workshop Lag Fix)](https://www.nexusmods.com/fallout4/mods/35382)

##### [Quieter settlements](https://www.nexusmods.com/fallout4/mods/2819)

##### [Locksmith](https://www.nexusmods.com/fallout4/mods/12454)
Allows you to lock any door or container, preventing any of those snoopy settlers to mess with your stuff.
Install Locksmith, then the replacer Locksmith.esp provided in my files.

##### [Basement Living](https://www.nexusmods.com/fallout4/mods/10967)

##### [Basement Living-Immersion Adjustment](https://www.nexusmods.com/fallout4/mods/28942)

##### [The Master Plan](https://www.nexusmods.com/fallout4/mods/16626)

##### [Vanilla Extensions](https://www.nexusmods.com/fallout4/mods/10032)
Improves vanilla snapping and adds a variety of highly functional blocks to the workshop menu. 
Install main file and any update file

##### [This is MY Bed](https://www.nexusmods.com/fallout4/mods/7399)

##### [Better Cooking Stations](https://www.nexusmods.com/fallout4/mods/12104)
Download and install:
- main file
- DLC patches

##### [PWR - Passive Water Resources](https://www.nexusmods.com/fallout4/mods/19871)
Install only main file, not the SKE patch

##### [CWSS Redux](https://www.nexusmods.com/fallout4/mods/14326)
Craftable working showers, baths, toilets, sinks, urinals, bubblers, and kitchens, that
followers, settlers, traders and caravan guards can use automatically. Custom idles, models,
sounds and visual FX. Automatic undressing/dressing. Immersive buffs that taper over time.
Essential to this modlist if you ́ve also installed “Get Dirty”

##### [Lore Friendly Posters](https://www.nexusmods.com/fallout4/mods/7145)
Install mod, and then the Wasteland and Contraptions Workshop and disappearing Mesh Fix
patches

##### [Workshop Rearranged](https://www.nexusmods.com/fallout4/mods/16181)
Install main file and patch pack
during installation of patch file, select:
Required patches

- Lore friendly posters – Replacer (after install, move replacer after WRA)
- Master Plan – Standalone

Optional patches

- Atomic radio – standalone
- Beantown interiors – standalone – DEF_UI

Creation club

- your choice

##### [Master Plan WRA Patch](https://www.nexusmods.com/fallout4/mods/16626)

##### [Better Stores](https://danielgamache.wixsite.com/awarhero/mod-archive)
During installation, select:
- Extra Custom Props
- Far Harbor patch

##### [Better Vendor Stalls](https://www.nexusmods.com/fallout4/mods/9758)

##### [Manufacturing Extended](https://www.nexusmods.com/fallout4/mods/15429)

##### [Thematic and Practical](https://www.nexusmods.com/fallout4/mods/16207)

##### [Creative clutter](https://www.nexusmods.com/fallout4/mods/20782)

##### [Do It Yourshelf](https://www.nexusmods.com/fallout4/mods/14532)

##### [Gruffydds Signs and Posters](https://www.nexusmods.com/fallout4/mods/9711)

##### [g2m Workshop](https://www.nexusmods.com/fallout4/mods/17088)

##### [Organized Workbench Menu](https://www.nexusmods.com/fallout4/mods/32588)

##### [JP Guard Towers](https://www.nexusmods.com/fallout4/mods/36178)

##### [Woody's Wasteland Stuff](https://www.nexusmods.com/fallout4/mods/24951)

##### [Private Area Markers (keep settlers out of your house)](https://www.nexusmods.com/fallout4/mods/26377)

##### [Timer Power Switch](https://www.nexusmods.com/fallout4/mods/10750)

##### [Weapon Rack Extended](https://www.nexusmods.com/fallout4/mods/15729)

##### [Weapon Rack Fixes](https://www.nexusmods.com/fallout4/mods/19324)

##### [Settlement Objects Combined](https://www.nexusmods.com/fallout4/mods/36461)

##### [Settlement Tidy bot](https://www.nexusmods.com/fallout4/mods/33217)

##### [Settlement Menu Manager](https://www.nexusmods.com/fallout4/mods/24204)

##### [Sim Settlements](https://www.nexusmods.com/fallout4/mods/21872)

##### [Sim Settlements Mega Pack - Year One](https://www.nexusmods.com/fallout4/mods/30396)

##### [Sim Settlements Mega Pack - Year Two](https://www.nexusmods.com/fallout4/mods/37983)

##### [Sim Settlements – Conqueror](https://www.nexusmods.com/fallout4/mods/37000)

##### [Sim Settlements Conqueror Faction Pack - The Forsaken Vaulters](https://www.nexusmods.com/fallout4/mods/38425)

##### [Sim Settlements - Building Plan Preview](https://www.nexusmods.com/fallout4/mods/26004)

##### [Sim Settlements - IDEK's Logistics Station](https://www.nexusmods.com/fallout4/mods/28945)

##### [Wasteland Venturers 2 All-In-One](https://www.nexusmods.com/fallout4/mods/30081)

##### [Place Everywhere](https://www.nexusmods.com/fallout4/mods/9424)

## Cosmetic overhauls

##### [BodySlide and Outfit Studio](https://www.nexusmods.com/fallout4/mods/25)

##### [LooksMenu](https://www.nexusmods.com/fallout4/mods/12631)

##### [Looksmenu Customization Compendium](https://www.nexusmods.com/fallout4/mods/24830)

##### [LooksMenu Body Tattoos](https://www.nexusmods.com/fallout4/mods/25000)

##### [FSM Body Textures](https://www.nexusmods.com/fallout4/mods/31965)

##### [Picturesque Presets](https://www.nexusmods.com/fallout4/mods/16788)

##### [Caliente's Beautiful Bodies Enhancer -CBBE-](https://www.nexusmods.com/fallout4/mods/15)

##### [Malestra's CBBE BodySlide Preset Collection](https://www.nexusmods.com/fallout4/mods/35316)


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

---
title: Main modding
description: The brunt of the modding, where we focus on adding mods
published: 1
date: 2019-07-24T00:02:48.636Z
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
During installation, select standalone with clutter

##### [Manufacturing Extended](https://www.nexusmods.com/fallout4/mods/15429)
Install main file and Far Harbor patch

##### [Thematic and Practical](https://www.nexusmods.com/fallout4/mods/16207)
Install main file and DLCpatch

##### [Creative clutter](https://www.nexusmods.com/fallout4/mods/20782)
During installation, select Creative Clutter DLC

##### [Do It Yourshelf](https://www.nexusmods.com/fallout4/mods/14532)
During installation, select extra half-shelf clutter full cost

##### [Gruffydds Signs and Posters](https://www.nexusmods.com/fallout4/mods/9711)
Install main file only

##### [g2m Workshop](https://www.nexusmods.com/fallout4/mods/17088)
During installation, check Main version [default]. If you during the intro sequence (right before the bathroom scene) get a white screen, press enter, downarrow and enter again. It ́s a message box spamming the screen at startup.

##### [Organized Workbench Menu](https://www.nexusmods.com/fallout4/mods/32588)

##### [JP Guard Towers](https://www.nexusmods.com/fallout4/mods/36178)

##### [Woody's Wasteland Stuff](https://www.nexusmods.com/fallout4/mods/24951)

##### [Private Area Markers (keep settlers out of your house)](https://www.nexusmods.com/fallout4/mods/26377)

##### [Timer Power Switch](https://www.nexusmods.com/fallout4/mods/10750)
Allows you to build power switches that automatically power on/off.

##### [Weapon Rack Extended](https://www.nexusmods.com/fallout4/mods/15729)

##### [Weapon Rack Fixes](https://www.nexusmods.com/fallout4/mods/19324)

##### [Settlement Objects Combined](https://www.nexusmods.com/fallout4/mods/36461)
oad esp version 2 (loose files)
If you use the get Dirty mod we will want to make the showers from this mod compatible.
- Open F04Edit. Select both "Get Dirty" and "Settlement Objects Combined" and click ok.
Only those 2 should be selected.
- Once loaded, Right Click on SOC, and click "Add Master" > select "Get Dirty".
- Expand Spells then click on "SShowerBetterEffect"
- Replace the 'DamageradiationWater' Effect with the CS7_DirtTier00 'Clean'" Effect (which
is what is triggered when you swim in the Get Dirty mod, for example).
- Repeat for SShowerBasicEffect
- Close and Save the "Showers" mod, as that is the only mod you've edited.

##### [Settlement Tidy bot](https://www.nexusmods.com/fallout4/mods/33217)

##### [Settlement Menu Manager](https://www.nexusmods.com/fallout4/mods/24204)

##### [Sim Settlements](https://www.nexusmods.com/fallout4/mods/21872)
Install 3 in 1 version
Allows you to build zone objects that tell the settlers what type of buildings to create in
different areas of your settlement and they will do so. Includes a progression system, a more
interesting settler needs system, and rewards to help settlements matter more. This mod aims
to completely change the way you think about settlements. You'll now be able to create
detailed, living places with minimal effort.
The ultimate goal: making every settlement a unique and awesome looking Fallout city, with
perks and rewards that help you at every stage of the game.

##### [Sim Settlements Mega Pack - Year One](https://www.nexusmods.com/fallout4/mods/30396)

##### [Sim Settlements Mega Pack - Year Two](https://www.nexusmods.com/fallout4/mods/37983)

##### [Sim Settlements – Conqueror](https://www.nexusmods.com/fallout4/mods/37000)

##### [Sim Settlements Conqueror Faction Pack - The Forsaken Vaulters](https://www.nexusmods.com/fallout4/mods/38425)

##### [Sim Settlements - Building Plan Preview](https://www.nexusmods.com/fallout4/mods/26004)
Download and install Newest main file, and the Mega pack – year one file.
Apart from the Sim Settlement add-ons we ́ve already installed, this mod also covers
Wasteland Venturers v7.1.1+, Always Free Sim Settlements MrJoseCuervo v1.3.2+ ,
Industrial City v0.9.0+, Junk Town by uituit v9+

##### [Sim Settlements - IDEK's Logistics Station](https://www.nexusmods.com/fallout4/mods/28945)

##### [Wasteland Venturers 2 All-In-One](https://www.nexusmods.com/fallout4/mods/30081)

##### [Place Everywhere](https://www.nexusmods.com/fallout4/mods/9424)

## Cosmetic overhauls

##### [BodySlide and Outfit Studio](https://www.nexusmods.com/fallout4/mods/25)
An easy to use tool for customizing bodies and outfits, creating new bodies and outfits, and
converting outfits between body types.
For a tutorial on how to use, click here. It ́s for NMM but the functionality of the program is
identical for MO2.

##### [LooksMenu](https://www.nexusmods.com/fallout4/mods/12631)
Adds engine modifications to improve character creation.

##### [Looksmenu Customization Compendium](https://www.nexusmods.com/fallout4/mods/24830)

##### [LooksMenu Body Tattoos](https://www.nexusmods.com/fallout4/mods/25000)
Tattoo overlays for LooksMenu. Install only ESP version (flag as ESL instead)

##### [FSM Body Textures](https://www.nexusmods.com/fallout4/mods/31965)
Download the first main file and install it.
During the Installer, click next till on the fourth panel and select Neck and Scalp
Adjustament option only. In the fifth panel select all Valkyr options, then click next and
select finish.

##### [Picturesque Presets](https://www.nexusmods.com/fallout4/mods/16788)
Adds a huge number of Looks Menu presets
Note: a minor bug causes some of the eyes and markings in the presets to be incorrect (crazy
red eyes, etc,)

##### [Caliente's Beautiful Bodies Enhancer -CBBE-](https://www.nexusmods.com/fallout4/mods/15)
Body replacer allowing for body physics and customization
Install first main file
Choose whatever body shape you like best
Tick all boxes under Outfit Options and F4EEMorphs

##### [Malestra's CBBE BodySlide Preset Collection](https://www.nexusmods.com/fallout4/mods/35316)
NSFW! optional This is a collection of 35 very accurate presets based on real people or
erotic fantasy art characters for CBBE/BodySlide. With variations it is ~90 presets total.

## Clothing

##### [Modular Road Leathers](https://www.nexusmods.com/fallout4/mods/29779)

##### [Commonwealth Shorts – CBBE](https://www.nexusmods.com/fallout4/mods/7898)
Install CBBE main file an the tight armors optional file, then install bodyslide from here.

##### [Shade Girl Leather Outfits – CBBE](https://www.nexusmods.com/fallout4/mods/32547)
Install main file and bodyslide hotfix file

##### [Raider Themed Mashups](https://www.nexusmods.com/fallout4/mods/29503)

##### [Badlands Mashups](https://www.nexusmods.com/fallout4/mods/30013)

##### [Commonwealth Mashups](https://www.nexusmods.com/fallout4/mods/27776)

##### [Wasteland Mashups](https://www.nexusmods.com/fallout4/mods/28099?tab=files)

##### [Irradiated Raiments](https://www.nexusmods.com/fallout4/mods/34193)
Install main file and Boston Belle Belt Hotfix for CBBE

##### [Spiff's Wasteland Clothing Pack](https://www.nexusmods.com/fallout4/mods/31129)

## Armor

##### [Eli's Armour Compendium](https://www.nexusmods.com/fallout4/mods/22431)
Download and install CBBE main file

##### [The Mercenary Pack](https://www.nexusmods.com/fallout4/mods/20088)
Download and install:
- The Mercenary - Pack v0.9b – loose files
- The Mercenary - Pack v0.9.c - plugin only update
there are optional, though reportedly a bit buggy, BodySlide files available for those who
intend to use BodySlide to custom fit armor to their characters body.

##### [West Tec Tactical Optics](https://www.nexusmods.com/fallout4/mods/12220)
ad and install:
- West Tek Tactical Optics v2.0.1 (minor update)Revision 2.5.0 alpha 2
- West Tek Tactical Optics v2.0 - AWKCR
- West Tek Tactical Optics v2.0 - Standard Leveled Lists

##### [PreWar Binoculars](https://www.nexusmods.com/fallout4/mods/17819/)
Adds functional binoculars to the game.
During install, select:
- “Binoculars – AWKCR” and 
- “Standard viewfinder”

##### [Crimsomrider's Accessories](https://www.nexusmods.com/fallout4/mods/19563)

##### [Tactical Flashlights](https://www.nexusmods.com/fallout4/mods/16172)
Adds wearable flashlight gear to the wasteland.
During install, select:
- AWKCR+AE
- 100% + shadows

##### [K-9 harness](https://www.nexusmods.com/fallout4/mods/17686)
download:
- K-9 Harness - Tactical Body Armor and Backpack for Dogmeat
- K-9 Harness - Armorsmith Extended plus DEF UI

##### [CROSS Pre-War Cybernetics](https://www.nexusmods.com/fallout4/mods/8609)
download main file only

##### [CROSS Institute Tech Mask](https://www.nexusmods.com/fallout4/mods/11881)

##### [CROSS Brotherhood Recon](https://www.nexusmods.com/fallout4/mods/27418)

##### [CROSS Chosen of Atom](https://www.nexusmods.com/fallout4/mods/37820)

##### [CROSS Courser Strigidae](https://www.nexusmods.com/fallout4/mods/28009)

##### [CROSS Institute Expeditionary suit](https://www.nexusmods.com/fallout4/mods/30857)

##### [CROSS Mojave manhunter](https://www.nexusmods.com/fallout4/mods/32214)

##### [Wearable Backpacks and Pouches](https://www.nexusmods.com/fallout4/mods/3258)
Install main file and the AWKCR Crafting optional patch
These clothes and armors need to be run through Bodyslide if you ́re using a bodyslide preset other
than the CBBE vanilla one. For instructions on how to do this, I will refer to the ever excellent
Gopher on YouTube. I recommend you watch the whole video, but for this step, you can skip to
timestamp 09:53.

## Power armor

##### [Enclave X-02 Power Armor](https://www.nexusmods.com/fallout4/mods/11017)

##### [Hellfire X-03 Power Armor](https://www.nexusmods.com/fallout4/mods/26251)

##### [InstitutePowerArmor](https://www.nexusmods.com/fallout4/mods/18315)

##### [Tribal Power Armor](https://www.nexusmods.com/fallout4/mods/22437)

##### [Standalone Construction Power Armor](https://www.nexusmods.com/fallout4/mods/12096)

##### [Liberty Power Armor](https://www.nexusmods.com/fallout4/mods/16305)

##### [Submersible Power Armor Redux - BioShock Inspired](https://www.nexusmods.com/fallout4/mods/25591)

##### [Some assembly required](https://www.nexusmods.com/fallout4/mods/12050)

##### [Some Assembly Required Patches for X-02 and X-03 Pas](https://www.nexusmods.com/fallout4/mods/26739?tab=files)

##### [Improved Jetpack Flight Model](https://www.nexusmods.com/fallout4/mods/34249)

##### [Restore Power Armor Frames](https://www.nexusmods.com/fallout4/mods/20890)

##### [Power Armor Impact FX](https://www.nexusmods.com/fallout4/mods/34012)

## Weapons of lore

##### []()

## Gameplay

##### [Unbogus Fallout overhaul](https://www.nexusmods.com/fallout4/mods/26026)
A fairly extensive game overhaul that will give you a more consistent, challenging and fun
experience with many neat features.
Install main file only.

##### [BS Defence](https://www.nexusmods.com/fallout4/mods/20137)

##### [More Attackers – Get off my Buildzone](https://www.nexusmods.com/fallout4/mods/27465)
Install main file

##### [Night Of The Creeps](https://www.nexusmods.com/fallout4/mods/23721)

##### [Sleepless Nights](https://www.nexusmods.com/fallout4/mods/33057)

##### [Shaikujin's Better warning for settlements being attacked](https://www.nexusmods.com/fallout4/mods/4106)

##### [Pack Attack NPC Edition - Gangs With Group Combat Tactics](https://www.nexusmods.com/fallout4/mods/30140)
Adds group combat AI to raider gangs, Gunners, and most other NPC groups, based on
individual NPC social awareness and tactical combat evaluation. Now with MCM!
NOTE: this mod is heavy on script resources and might cause game instability, especially if
adding further scripted mods on top of this list.

##### [H.A.R.D.Core - Fusion Generator Overhaul](https://www.nexusmods.com/fallout4/mods/28890/)
isn ́t it amazing how every fusion core you find, regardless of how many hundreds of years
they ́ve been in use, are fully charged?

##### [QuickTrade](https://www.nexusmods.com/fallout4/mods/16229)
Yeah, yeah, I ́m here to trade, not chit-chat.

##### [Auto Eat and Drink in Survival](https://www.nexusmods.com/fallout4/mods/25408)
In the real world you don ́t need a pip-boy to eat and drink, you just do.

##### [Grab and Eat All-in-One](https://www.nexusmods.com/fallout4/mods/17608)
use 1.0 version from old without notereading feature. 1.5 version has issues.

##### [Read Notes from Containers and Corpses](https://www.nexusmods.com/fallout4/mods/18077)

##### [GET DIRTY (take a bath)](https://www.nexusmods.com/fallout4/mods/29171)
Get dirty while exploring the wasteland. Take a bath to get clean again.

##### [GET DIRTY (take a bath) additional effects](https://www.nexusmods.com/fallout4/mods/36880)
This little patch for 7StarC's GET DIRTY mod adds charisma modifiers and some other
minor tweaks to the original mod. I made several flavors to accomodate your preferences.

##### [Canteens of the commonwealth](https://www.nexusmods.com/fallout4/mods/24493)

##### [Fill'em Up Again (Dynamic Bottle Recyclation)](https://www.nexusmods.com/fallout4/mods/12674)
SURVIVAL Ever wondered that you drink a beer for example and the bottle is magically
gone? With the new survival mode you could use the bottle to get some water! But how to
get this bottle!? Fill ́em up again fixes that and gives a bottle in return!
Install loose files version

##### [Intimidation Overhaul](https://www.nexusmods.com/fallout4/mods/23922)

##### [Critical Hits Outside of VATS Revisited](https://www.nexusmods.com/fallout4/mods/25583)
Install main and worse criticals optional files.

##### [Hacking 101](https://www.nexusmods.com/fallout4/mods/15033)
Major rework of the Hacking system.

##### [Salvage Robot Parts](https://www.nexusmods.com/fallout4/mods/25355)

##### [Sofa Surfer - Sleeping on Couches](https://www.nexusmods.com/fallout4/mods/24944)

##### [SKK Combat Stalkers (hostile spawns)](https://www.nexusmods.com/fallout4/mods/30308)

##### [RSE Elements Vol.3 - Karma System feat. Bounty Hunters](https://www.nexusmods.com/fallout4/mods/36020)

##### [Outfit Switcher](https://www.nexusmods.com/fallout4/mods/10282)
Lets you save your entire loadout, including armor pieces! Then equip and swap between
saved loadouts with the press of a button.

##### [I Ain't Drunk (I'm Just Drinking)](https://www.nexusmods.com/fallout4/mods/36888)
Now you can have a beer without getting drunk, and beer quenches thirst.

##### [First Person Death Cam](https://www.nexusmods.com/fallout4/mods/27537)
Die in first person

##### [Survival options](https://www.nexusmods.com/fallout4/mods/14650)
SURVIVAL This is an F4SE plugin which restores some hard-coded features disabled by
the game
Install version 1.6.2, the version before MCM, as it reportedly works better.

## NPC and creature overhauls

##### [Raider Overhaul](https://www.nexusmods.com/fallout4/mods/9103)
Install Raider Overhaul WIP 11.4c optional file only, then install AE replacer Raider
Overhaul 11.4c from the Armorsmith Extended files.

##### [D.E.C.A.Y – Better Ghouls](https://www.nexusmods.com/fallout4/mods/2500)
Install main file only

##### [Deadlier Deathclaws](https://www.nexusmods.com/fallout4/mods/13822)

##### [Unique NPCs - Creatures and Monsters](https://www.nexusmods.com/fallout4/mods/24357?tab=files)
Install main file and any updates/fixes
During installer choose
- DECAY
- Deadlier Deathclaws
- SMR no patch
- Respawnable no patch
- Unique NPCs - C n M – Non-Lore
The Unique NPCs installer will have replaced a couple of earlier installed esps (edited
versions to make them cmpatible with Unique NPCs). Those esps will now need to be
moved below the main Unique NPC esp to work properly. Below is a ist of the esps you
need to move before moving on to the next mod:

D.E.C.A.Y.esp
DeadlierDeathclaws
make sure that this section of your right pane now looks like this:

After installation, open Unique NPCs – Creatures and Monsters.esp in FO4Edit expand:
Worldspace
>0000003c
>Block -1, -1
>Sub-Block -2, -1
>0000E48E
>Temporary
and remove 001D0F96 (breaks precombines)
##### [Less Loot D.E.C.A.Y](https://www.nexusmods.com/fallout4/mods/32938)

##### [Feral Ghouls After Dark](https://www.nexusmods.com/fallout4/mods/22434)

##### [Super Mutant Redux](https://www.nexusmods.com/fallout4/mods/11853/)
Reworks the super mutant faction including Behemoths, FEV Hounds, and of course, Super
Mutants.
Install Super Mutant Redux and any updates. During installer select Armorsmith patch

##### [We are the minutemen](https://www.nexusmods.com/fallout4/mods/6443/)

##### [Far West Minutemen](https://www.nexusmods.com/fallout4/mods/27972)

##### [Militarized Minutemen](https://www.nexusmods.com/fallout4/mods/29853)
During installer:
• WATM compatibility

##### [Synth Overhaul – C.A.S.T](https://www.nexusmods.com/fallout4/mods/9525)
This mods overhauls all the Synths by giving them 70 new armor sets, 77 helmets, 42
uniforms and 2 Synth weapons. From damaged armor to undamaged looking armor sets.Revision 2.5.0 alpha 2
guide updated 2018-07-04, load order list updated 2018-07-04
Install the main ba2 version, and any update
During install select:
- Synth Overhaul – no weapons
- AWKCR + AE
- Remove level requirements (Optional. Synths will be more powerful at lower levels!)

##### [Better Settlers](https://www.nexusmods.com/fallout4/mods/4772)
Better Settlers is a lore friendly mod that adds more than 240 new settlers to the vanilla
settler selections.
Install Better Settlers v2.0 DLC Master FOMOD main file
During install select:
- Bettersettlers.esp
- No Lollygagging!
- Dirty faces
- Better settlers default
- Vanilla
- Community hair and clothing
- Mortal pack

##### [Simple Settlers](https://www.nexusmods.com/fallout4/mods/36074)
Main options
- Mortal settlers
Optional
- None
##### [Unique NPCs - An Overhaul of the Commonwealth](https://www.nexusmods.com/fallout4/mods/21248)
Install any of the two mian files (they ́re identical), and the 2.1 update
FOMOD instructions:
Core
- Unique Npcs Core.esp
- I read this if you don ́t use the HD DLC (which you shouldn ́t anyway)
Better Settlers and it ́s patches
- Better Settlers - No LollyGagging
- Mortal Pack
- No Patch - Standard Mix
No Patch - Standard Armor Mix
Better Settlers - Elis armour compendium - AE
No patches
Special Settlers
- No special settlers
Minutemen options
- Militarized Minutemen
- Far West Minutemen
- WATM 5.x enhanced
- none (we are the far west minutemen merged)
- UniqueNPCs_WATMM_FarWest_MilitarizedMinuetmen.esp
Gunner options
- No patches
3rd party patches and final otpions
- Standard mortality
- Diamond city expansion
- No settlement patches
- Unique NPCs_AE_SuperMutantRedux
- Looks Menu Customization Compendium Replacer
If the FOMOD installer doesn ́t let you install the DCE patch, then I ́ve added the patch to
the CtGW R2 archive. Install separately or merge with Unique NPCs doesn ́t matter as long
as it ́s place after it.
The Unique NPCs installer will have replaced a couple of earlier installed esps (edited
versions to make them cmpatible with Unique NPCs). Those esps will now need to be
moved below the main Unique NPC esp to work properly. Below is a ist of the esps you
need to move before moving on to the next mod:
Looksmenu customization compendium
We are the minutemen
Far west minutemen
Militarized minutemen
Better Settlers
make sure that this section of your right pane now looks like this:

##### [Raider children](https://www.nexusmods.com/fallout4/mods/16586/)
Raiders have been known to abduct children in the commonwealth to replenish their ranks.
Once indoctrinated, those poor children return the world from which they came to pillage
and kill.

##### [FO4 NPCs Travel](https://www.nexusmods.com/fallout4/mods/16987/)
This mod adds 338 new NPCs, travelling across the commonwealth
Install FO4 NPCs Travel main file

##### [Settlers of the Commonwealth](http://3dnpc.com/wiki/fallout-mods/fallout-4/settlers-of-the-commonwealth/)
Adds 30 new recruitable settlers across the commonwealth. From the creator of Tales of the
Commonwealth

##### [Sim Settlements - Settlers of the Commonweath - City Leaders](https://www.nexusmods.com/fallout4/mods/29799)

##### [Immersive Dogmeat](https://www.nexusmods.com/fallout4/mods/34128)
ESP version

##### [Moddable Robot Settlers](https://www.nexusmods.com/fallout4/mods/11976)

##### [Killable Children](https://www.nexusmods.com/fallout4/mods/197)

##### [Less Aggressive Settlers](https://www.nexusmods.com/fallout4/mods/36399)

##### [Grieving Raider - A Most Important Mod](https://www.nexusmods.com/fallout4/mods/32335)

## Companion overhauls

##### [Valentine REBORN](https://www.nexusmods.com/fallout4/mods/9568)

##### [Valentine Noir](https://www.nexusmods.com/fallout4/mods/7551)

##### [Live Action Mr. Handy](https://www.nexusmods.com/fallout4/mods/9571)
Adds spotlights to Codsworth and all Handy models eyes including Gutsy and Nanny.
Spotlights also included in all Automatron eyes added in the Robot Workbench under Handy
Torso.
Install Live Action Handy - With Iris and GlowMap – Repack version

##### [Cait's Corset – Tailored](https://www.nexusmods.com/fallout4/mods/27939)

##### [Just another Piper Outfit](https://www.nexusmods.com/fallout4/mods/21114)

##### [CIO - Companion Inventory Overhaul](https://www.nexusmods.com/fallout4/mods/34977)

## New companions

##### [Tina De Luca Voiced as a Settler (Dependency Revisited)](https://www.nexusmods.com/fallout4/mods/20226)
Allows you to recruit Tina outside Dependency even after the quest was already finished. It
also fixes several bugs with the "good" ending of the Vault 81 quest Dependency.

##### [Heather Casdin](https://www.nexusmods.com/fallout4/mods/23273)
Heather is a story-driven character with over 1200 lines of custom, voiced dialogue, quests,
etc
Custom voiced companion for Fallout 4, boasting over 1200 lines of custom made and
voiced dialogue. Affinity system, supporting DLC. Romance. Custom quest. Vanilla lore-
friendly face and background.
During install choose "Heather with Extended Dialogue Interface" on the first pane, AE on
the second pane.

##### [Heather Casdin - Assorted Patches](https://www.nexusmods.com/fallout4/mods/24314)

##### [Ellen - the cartographer](https://www.nexusmods.com/fallout4/mods/15962)
Custom voiced companion for Fallout 4, boasting over 1200 lines of custom made and
voiced dialogue. Affinity system, supporting DLC. Romance. Custom quest. Vanilla lore-
friendly face and background.

##### [Buttons – Companion](https://www.nexusmods.com/fallout4/mods/31710)

##### [I am Darlene](https://www.nexusmods.com/fallout4/mods/36254)

## Animations

##### [Laser weapons 1st person reposition](https://www.nexusmods.com/fallout4/mods/23102)
Install Institute and standard lasers main file

##### [Automatically Lowered Weapons](https://www.nexusmods.com/fallout4/mods/20093)

##### [New Alternative Animations](https://www.nexusmods.com/fallout4/mods/29857)
Download and install one big pile of animations optional file

##### [Stay Focused Son](https://www.nexusmods.com/fallout4/mods/18619)

##### [Power Armor Animation Changes](https://www.nexusmods.com/fallout4/mods/4408)

## Vanilla location overhauls

##### [Better Goodneighbor](https://www.nexusmods.com/fallout4/mods/16594/)
Download and install main file, update and cleaned esp

##### [Better The Third Rail](https://www.nexusmods.com/fallout4/mods/15388/)
Download and install main file, update and cleaned esp

##### [Better Atom Cats Garage](https://www.nexusmods.com/fallout4/mods/14764/)
Download and install main file and cleaned esp

##### [Vault 88 - Your Vault Your Way - Build Ready](https://www.nexusmods.com/fallout4/mods/35076)

##### [A sensible Prydwen overhaul](https://www.nexusmods.com/fallout4/mods/24198/)

##### [Introducing – Radium-Inc](https://www.nexusmods.com/fallout4/mods/32175)

##### [The Lost Building of Atlantic](https://www.nexusmods.com/fallout4/mods/25401)

##### [Sanctuary Hills - Root Cellar Remade](https://www.nexusmods.com/fallout4/mods/24791)

##### [Virgils LABORATORY - Evil Lab Overhaul](https://www.nexusmods.com/fallout4/mods/29540)

##### [Aloot's Home Plate](https://www.nexusmods.com/fallout4/mods/15300/)

##### [Hotel Rexford](https://www.nexusmods.com/fallout4/mods/36458)
Install main file and optional NPCs outside of the street file

##### [Better Robotics Disposal](https://www.nexusmods.com/fallout4/mods/36077)

## New quests and locations

##### [Fusion City Rising](https://www.nexusmods.com/fallout4/mods/16423/)

##### [Outcasts and Remnants](https://www.nexusmods.com/fallout4/mods/21469/)

##### [Project Valkyrie](https://www.nexusmods.com/fallout4/mods/28085)

##### [Nuka-World Reborn](https://www.nexusmods.com/fallout4/mods/32857)
Install main and optional file, then the AE patch here: https://www.nexusmods.com/fallout4/mods/34260

##### [50 Ways to Die at Dr. Nick's](https://www.nexusmods.com/fallout4/mods/25564/)
10 Connected Quests, Unique Rewards, Custom Player Home, Lore-Friendly Backstory,
Lots of Explosions, and a Twist.

##### [The Secret of Huntress Manor - A Far Harbor Story](https://www.nexusmods.com/fallout4/mods/27311)
Install 1.2 regular main file

##### [Vault 494 - A Vault-Tec Story](https://www.nexusmods.com/fallout4/mods/23651)

##### [David Hunter - A Brotherhood Story](https://www.nexusmods.com/fallout4/mods/16808)

##### [Hilda Hughes - An Institute Story](https://www.nexusmods.com/fallout4/mods/22128)

##### [Tales from the Commonwealth](http://3dnpc.com/)
install Tales and Atomic Radio (optional) from 3Dnpc.com (always update before Nexus
version and contains custom tracks not on Nexus).

##### [Sector 5 – Rise and Fall](https://www.nexusmods.com/fallout4/mods/38457)

## Weather and environment

##### [Vivid Weathers](https://www.nexusmods.com/fallout4/mods/15466)
During install
Alternative addons
- Disable Volumetric Fogs
- Extended Rain Sounds
- Vivid Weathers Quest and Player Home
Visual changes
- Default - No changes
Compatibility patches
- Far Harbor Patch
- Nuka World
Seasons of Vivid Weathers
- NO Season Limitation

##### [WET – Water Enhancement textures](https://www.nexusmods.com/fallout4/mods/20775)
WET enhances all the bodies of water in the game, as well as adding new water and rain
effects.
During Installer select the WET Assets With Rain and the WET Clearer (ESL) options

##### [Darker nights](https://www.nexusmods.com/fallout4/mods/191)
Install both main and optional files, during installer, choose:
- Light (level 4)
- Far harbor and Nuka World DLC patches
- Vivid weathers
- Easiest (level 6)
- Alternative (green tint)
- Weaker night vision
Leave the other options unticked

##### [Vault-Tec Workshop Overhaul](https://www.nexusmods.com/fallout4/mods/17174)

##### [Clarity](https://www.nexusmods.com/fallout4/mods/31991)

##### [Fr4nsson's Light Tweaks](https://www.nexusmods.com/fallout4/mods/2139)

##### [Thaylar's Settlement Lighting Fixes](https://www.nexusmods.com/fallout4/mods/20003)

##### [Pip-Boy Flashlight](https://www.nexusmods.com/fallout4/mods/10840)

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

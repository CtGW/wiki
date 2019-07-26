---
title: Main modding
description: The brunt of the modding, where we focus on adding mods
published: 1
date: 2019-07-26T17:19:35.832Z
tags: 
---

# Main modding
## Choosing ESL or not

> 
> **TLDR**: When given a choice of choosing an ESP or an ESL you should always download the ESP and then manually mark it as an ESL in FO4Edit.
>{.is-danger}

For an in-depth understanding: https://www.afkmods.com/index.php?/topic/5079-plugin-files-and-you-esmeslesp/

<center><details><summary><b>We outline a small summary</b> </summary>
<p>

### How ESLs work

Firstly, lets remember that the Bethesda engine allows loading 255 plugins in total.
Each plugin occupies a namespace, `xx`, for its load order, where a general element is represented by: `xx123456`

So, in theory, any plugin can add <code>16<sup>6</sup></code> new items, though in reality the number is a bit smaller.

ESLs work by sharing the `FE` namespace, so that an element in the plugin looks like `FEyyyyyy`.
The first ESL has the plugin FormIDs as: `FE000zzz`, the second ESL has FormIDs as: `FE001zzz`, so on and so forth.

So in theory, you cannot have more than <code>16<sup>3</sup>=4096</code> ESL plugins in your modlist, each of which can only introduce another <code>16<sup>3</sup></code> new items/elements.

### ESL vs ESP
.esl plugins are loaded in the master space and is termed as a *light master*, as internally the bethesda engine makes every .esl with an ESM tag as well.
This means that they are loaded before the other files and they can mess up your load order.

On the other hand, if you use an .esp marked as an ESL, the plugin respects your load order.

So whenever there is an option, always choose the ESP file instead of the ESL file and then you can decide if you want to make it into and ESL or not.
</p>
</details>
</center>

---

## Mod outline

##### Mod name *version*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span> <span style="background-color:#00aedb; padding:3px;"><font color="white"> Optional </font></span> <span style="background-color:#d11141; padding:3px;"><font color="white"> Clean </font></span> <span style="background-color:#ffc425; padding:3px;"><font color="black"> Extracted </font></span> <span style="background-color:#f37735; padding:3px;"><font color="black"> ESL </font></span> <span style="background-color:#ff8b94; padding:3px;"><font color="black"> HD-HQ </font></span>
Mod description
- File 1
- File 2

> Extra information/explanation
>{.is-success}

> Extra steps

---

## Legend

- <span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>: Mods which are essential to the guide
- <span style="background-color:#00aedb; padding:3px;"><font color="white"> Optional </font></span>: Mods which are optional and can be skipped
- <span style="background-color:#d11141; padding:3px;"><font color="white"> Clean </font></span>: Mods which should be cleaned using Fo4Edit-quickclean
- <span style="background-color:#ffc425; padding:3px;"><font color="black"> Extracted </font></span>: Mods where you should extract the `.bsa` files
- <span style="background-color:#f37735; padding:3px;"><font color="black"> ESL </font></span>: Mods which you can/should manually mark as ESL
- <span style="background-color:#ff8b94; padding:3px;"><font color="black"> HD-HQ </font></span>: Mods which are taxing on the computer and should be installed with caution

---

## Core mods

##### [F4SE](https://f4se.silverlock.org/) *v0.6.17*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
Install only the scripts, by doing a manual install in MO2 and selecting data folder.

> This way we can more easily determine if any of the scripts are overwritten by later mods.
{.is-success}


##### [PrivateProfileRedirector F4](https://www.nexusmods.com/fallout4/mods/33947) *v0.4*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
Speeds up game start by storing INI files in memory instead of opening, parsing and closing the file each time some value from it is needed.

##### [Unofficial Fallout 4 Patch](https://www.nexusmods.com/fallout4/mods/4598) *v2.0.7*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
A comprehensive bugfixing mod for Fallout 4. The goal of the Unofficial Fallout 4 Patch (aka UFO4P) is to eventually fix every bug with Fallout 4 not officially resolved by the developers to the limits of the Creation Kit and community-developed tools, in one easy-to-install package. 

##### [Mod Configuration Menu](https://www.nexusmods.com/fallout4/mods/21497) *v1.37*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
The Mod Configuration Menu is a settings page for mods! It provides a central location for mod configuration, accessible via the Pause menu. 
 
##### [Game Configuration Menu](https://www.nexusmods.com/fallout4/mods/33759) *v0.6*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
GCM allows you easily set many game settings without the need of additional ESPs or console commands. 
 

##### [Armor and Weapon Keywords Community (AWKCR)](https://www.nexusmods.com/fallout4/mods/6091) *v8.51*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
 This is a master file to create a standardize framework for armor so that modders can create and modify armor (like Armorsmith) while making edits compatible with mods that adjust dynamic item naming (like Valdacil's Item Sorting).
 
##### [Armorsmith Extended](https://www.nexusmods.com/fallout4/mods/2228) *v4.6*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
This mod does so much awesome stuff that the description doesn't come anywhere close to fitting here. 

## Minor fixes

##### [CCCleaner](https://www.nexusmods.com/fallout4/mods/26592) *v3.11*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
clean all about CC from ur game interface 
 
##### [Achievements](https://www.nexusmods.com/fallout4/mods/12465) *v1.0.5*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
Uses F4SE to re-enable achievements while mods are active

##### [RAW INPUT - The Ultimate Mouse Sensitivity Fix](https://www.nexusmods.com/fallout4/mods/27019) *v2.4*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
Disabled Mouse Acceleration, Horizontal/Vertical Parity, Scalable ADS Multiplier, Normalized Sensitivity

##### [Simple Trashcan fix](https://www.nexusmods.com/fallout4/mods/14707/) *v1*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
One does not simply "steal" trashes.  

##### [Wetness shader fix](https://www.nexusmods.com/fallout4/mods/23389) *v2.2*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
This small mod fixes the exaggerated shine of specific objects while it's raining. Comes with an installer for different options. 
 
##### [Eye Normal Map Fix](https://www.nexusmods.com/fallout4/mods/819) *v1b*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
Enhanced normal maps for the eyes. 

##### [Far Harbor Doctor Dialogue Fix](https://www.nexusmods.com/fallout4/mods/16274) *v1.0*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
 Far Harbor doctors will now offer doctor services. 

##### [Search and Destroy Fixed](https://www.nexusmods.com/fallout4/mods/33127) *v1.0*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
The Far Harbor Quest "Search and Destroy" is massively bugged in the game, and while the quest can be completed, the Brotherhood doesn't attack as it is supposed to. This mod fixes the reasons they don't arrive at the attack site and several other bugs within the quest that would probably never have been noticed without it being fixed. 

##### [Lever Action Reload Fix](https://www.nexusmods.com/fallout4/mods/22896) *v1.4*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
The most stable lever action reload fix out there with working 3rd person. 

##### [Overboss Power Armor headlamp fix](https://www.nexusmods.com/fallout4/mods/19295) *v1.2*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
Adds better headlamp functionality to the Overboss power armor helmet from Nuka World. 

##### [Mechanist's Lair - expanded corrected and fixed](https://www.nexusmods.com/fallout4/mods/11490) *v0.1*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
This settlement expansion comes in three flavours and with an additional fix added !
You can choose from simply using a fix, that will allow to build in the Lair like in every other settlement, or you can go for one of the three / four expansions, one fullfeatured, a more immersive one and a third/fourth Version, that is really as immersi 

##### [Perception Bug Fix](https://www.nexusmods.com/fallout4/mods/35376) *v1.0.0*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
This mod prevents the "Perception Bug" from affecting the player. 

##### [Protectron Subway Steward (fix)](https://www.nexusmods.com/fallout4/mods/22022) *v*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
Enables the scene for Protectrons when assigned the Subway Steward personality. 
 
##### [Alex's Male First Person Camera Height Fix](https://www.nexusmods.com/fallout4/mods/27582) *v1.0*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
Adjusts the eyeheight in first person if you play as a male character.

##### [Vault 111 Floor Guide Fix](https://www.nexusmods.com/fallout4/mods/28167) *v1.0*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
 This mod fixes the arrows and lines at the entrance in prewar Vault 111. They're disappearing when viewed from certain angles. Now not anymore. 

##### [Starlight Drive In LOD Fix with ESL](https://www.nexusmods.com/fallout4/mods/23034) *v1.0*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
 Was always annoyed with how the Drive In would fade into view when walking up to it. Can now be seen properly from far away. More immersive. ESL Version Available. 

##### [NukaWorld Transit Center LOD Fix with ESL](https://www.nexusmods.com/fallout4/mods/30925) *v1.0*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
 Makes the giant Nuka Bottles at the Transit Center in the Commonwealth visible from far away so they don't pop in when you get close. Purely for immersion. ESL version available. 

##### [Vault111 And Billboard LOD Fix](https://www.nexusmods.com/fallout4/mods/36288) *v1*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
 Makes Vault 111 and the giant Billboard next to it visible from a distance! 

##### [Sanctuary Bridge LOD Fix](https://www.nexusmods.com/fallout4/mods/36288) *v1*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
 Makes Vault 111 and the giant Billboard next to it visible from a distance! 

##### [Far Harbor Bed Fix](https://www.nexusmods.com/fallout4/mods/34504) *v1*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
 Fixes the evil bed at far harbor red rocket. 
 
##### [Hardware Town Key Havok Fix](https://www.nexusmods.com/fallout4/mods/34497) *v1.0*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
 A super simple mod that disables Havok settling on the Hardware Town Storage Key by applying the defaultdisablehavokonload script to it. This prevents it from being knocked off the desk on the second floor should you use frag grenades or mines. 

##### [Nuka Cola Storage Rack](https://www.nexusmods.com/fallout4/mods/24909) *v02.00.00*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
 The constructable object form for the Nuka Cola Storage Rack has an error This fixes that. 

##### [Space Sentry Leg Fix](https://www.nexusmods.com/fallout4/mods/29869) *v1.00*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
 Fixes the wonky wheels on the Space Sentry legs 

##### [Vault Door FIXED](https://www.nexusmods.com/fallout4/mods/24954) *v0.1*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
 Fixed navmesh for Vault-Tec Workshop DLC Vault Door 

##### [Blood Pack Mesh Fix](https://www.nexusmods.com/fallout4/mods/25800) *v1.0*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
 Fixed model of Blood Pack. Now tubes are visible. 

##### [Fixed Gobo Effects](https://www.nexusmods.com/fallout4/mods/27445) *v1.4*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
 This mod fixes artefacts, pixelation and color banding in textures that are used for special light effects. Zero performance loss, little to nothing strain for your VRAM, no esp needed, no reason to not use it. 

##### [Plasma Impact Fix](https://www.nexusmods.com/fallout4/mods/25412) *v1.1*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
 A very simple little mod that fixes the bugged plasma impact sets if you're running EBT. 

##### [Doorway Endcap Fix](https://www.nexusmods.com/fallout4/mods/35818) *v1.0*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
 Fixes the Workshop Vault Domestic Doorway Endcap so that it snaps in the correct place. 

##### [Flicker fixer](https://www.nexusmods.com/fallout4/mods/35720) *v5.0*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
 Fixes most of the exterior flickering aka z fighting in the game, particularly in the Boston and Cambridge areas. 

##### [BiRaitBec ́s merged Fixes](https://www.nexusmods.com/fallout4/mods/23556) *v1.0*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
Merged mod for a lot of fixes that UFO4P still has not gotten around to include yet.


## Misc tweaks

##### [No Quest Autostart - BoS Fire Support](https://www.nexusmods.com/fallout4/mods/31563) *v1.0*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
 Prevents "Fire Support" from beginning without the player listening to Haylen's radio message. 

##### [No Quest Autostart - Far Harbor](https://www.nexusmods.com/fallout4/mods/31450) *v1.0*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
Prevents "Far From Home" from starting without the player either listening to Ellie's radio message or visiting the Nakano residence. 

##### [No Quest Autostart - Nuka World](https://www.nexusmods.com/fallout4/mods/31433) *v1.0*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
 Simple script edit to prevent the Nuka-World main quest from running without either visiting the Nuka-World Transit Station or listening to the radio station. 

##### [No Quest Autostart – Automatron](https://www.nexusmods.com/fallout4/mods/31576) *v1.0*
 <span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
 Prevents the Automatron main quest from automatically starting until the player listens to the Caravan Distress Call. 

##### [No Quest Autostart – Vault-Tec](https://www.nexusmods.com/fallout4/mods/31454) *v1.0*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
This mod prevents the quest 'Vault-Tec Calling' from automatically updating and beginning officially until you either A) listen to the Vault 88 emergency broadcast or B) Enter the Vault 88 cell--as in, go inside. 

##### [Recruiter Radio Freedom](https://www.nexusmods.com/fallout4/mods/14762) *v1*
 Makes Radio Freedom a Recruitment Beacon 

##### [Corpse Collision](https://www.nexusmods.com/fallout4/mods/37133) *v1*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
Run into dead things and they get pushed. 

##### [Realistic Death Physics - No Animations](https://www.nexusmods.com/fallout4/mods/4371) *v1.2*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
10mm bullets knocking raiders into the air? Deathclaws tossing you around like a tennis ball? Dead bodies floating gently to the ground like rose petals? No more! 

##### [Remove Interior Fog](https://www.nexusmods.com/fallout4/mods/2628) *v1.5dlc6*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
This mod will pretty much remove all that ugly fog you see everywhere indoors and will look a million times better. 

##### [Realistic conversations](https://www.nexusmods.com/fallout4/mods/32514) *v1.0*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
Every social logic in Fallout for NPCs is changed, they talk more often to each others. And will less likely greet to you from a distance, they will also greet less often too, making them to not act as much as robots. NPCs are also more clever and will know for example if they talked to a NPC and will therefore talk to another or not talk at all. 

##### [Immersive Generic Dialogue](https://www.nexusmods.com/fallout4/mods/14108) *v1.03c*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
Your reputation will now be determined by your actions and how well you manage your settlements. Earn the respect and trust by helping people and be a good ruler of your settlements, or be shunned for the opposite actions. 

##### [Icebreaker Settlements – Settler Dialogue Overhaul](https://www.nexusmods.com/fallout4/mods/25972) *v1.03*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
400+ new carefully selected lines of settler dialogue to reduce the repetitive sound of the 168 original. All lines in the original actors' voices. Intended to blend in very naturally with the default lines. Settler dialogue lines that insulted the player character were also tweaked. 
 
##### [Icebreaker - Piper - Companion Dialogue Overhaul](https://www.nexusmods.com/fallout4/mods/25525) *v1.0.5*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
Adds more variety to the dialogue companions use the most often. Over 300 new audio files in the companions own voice, with facial expression, and supports Affinity. 

##### [Settler Sandbox](https://www.nexusmods.com/fallout4/mods/20442/) *v4.0*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
Settler Sandbox and AI Expansion 

##### [Locky bastard](https://www.nexusmods.com/fallout4/mods/13380/) *v4.0*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
Tired of lockpicking ? Shoot a bullet at that goddamn lock to open it ! Or do you prefer to blow it up with some explosive ? Oh wait, you just want to kick doors open with your shiny X-01 ? Well, you can do that as well. 

##### [First Person messages](https://www.nexusmods.com/fallout4/mods/10870) *v2.0*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
Changes the messages you get to first person messages. 

##### [Quest Summary by Default](https://www.nexusmods.com/fallout4/mods/2664) *v0.2*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
Show quest summary by default in the quest log instead of showing animation. Useful for avoiding spoilers and preventing excessive toggling of summary display. 

##### [Puddle remover plus](https://www.nexusmods.com/fallout4/mods/34035) *v6.0*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
Options to remove Water Puddles, Blood Puddles, Mud Puddles, Seagull Droppings and the dirt clouds from NPC Footsteps. 

##### [R2K fast pipboy](https://www.nexusmods.com/fallout4/mods/17777) *v1.1*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
A collection of mods and ends. 

##### [Not So Bright Pins](https://www.nexusmods.com/fallout4/mods/35097) *v1.0*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
Reduced the brightness of the pins in the loadingscreens 

##### [Swinging Animated Meat Bags](https://www.nexusmods.com/fallout4/mods/21087) *v1.41*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
This mod adds a new swinging animation to all the hanging meat bags in the game, with swinging sound, dripping blood and swarming flies effect. It also fixes all meat bags so their loot will respawn. Swarming flies are also added to fallen meat bags, including craftable ones. 

##### [Tougher Cars Durable Vehicles](https://www.nexusmods.com/fallout4/mods/3680) *v1.3*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
Increases the durability of destructible vehicles. Three flavors to choose from: multiplied vanilla values, diverse modified values, or indestructible vehicles. 
 
##### [Lootable vendors](https://www.nexusmods.com/fallout4/mods/34960) *v1.01*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
Wipe the vendor's inventory dry with this mod. This mod transfers the items that a vendor is selling to their body when they are killed by the player. 

##### [ExitSave Killer](https://www.nexusmods.com/fallout4/mods/18102) *v0.2*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
This mod stops exit saves from being done by the game. 

## Camera and UI

##### [DEF_UI](https://www.nexusmods.com/fallout4/mods/10654) *v1.5.1*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
Re-release of DEF_HUD and DEF_INV by Neanka with a combined installer package. DEF_HUD is a fully 
customizable HUD. DEF_INV provide many improvements to Pipboy, container, and barter inventory screens. 
- *Main files*: Def_ui 1.5.1
- *Main files*: def_ui_translations 1.10.130

###### Def_ui 1.5.1 (installation options)
- DEF_HUD
- DEF_INV
- Language and Screen Ratio based on your preferences
- Do NOT install component tags and Vanilla Hud
- i already have sorting xml files option

> Delete the following files 
>   `Interface\Translate_**.txt`

##### [DEF_UI Iconlibs Rescaled and Fixed](https://www.nexusmods.com/fallout4/mods/31088/) *v1.5*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
 Based on Updated ICONLIBS2 for DEF_UI by omega9380. Aims to bring consistency in design and coloring to the icon library. Also fixes various issues with icon sizes, bounding boxes and scaling. 
- *Main files*: DEF_UI Iconlibs Rescaled and Fixed - Subtle Color

> Add/change the following values to fallout4custom.ini
> ```
> [Pipboy]
> bPipboyDisableFX=1
> fPAEffectColorB=1
> fPAEffectColorG=1
> fPAEffectColorR=1
> 
> [Interface]
> iHUDColorB=255
> iHUDColorG=255
> iHUDColorR=255
> 
> [Display]
> fPipboyScreenDiffuseIntensityPA=0
> fPipboyScreenEmitIntensityPA=1
> ```
>

##### [Extended Dialogue Interface](https://www.nexusmods.com/fallout4/mods/27216) *v1.3.4*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
 The Extended Dialogue Interface removes the hardcoded 4-option limit on dialogue and adds full engine support for any number of player dialogue options. 
- *Main files*: Extended Dialogue Interface 1.3.4

##### [HUDFramework](https://www.nexusmods.com/fallout4/mods/20309) *v1.0f*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
HUDFramework is a UI framework that makes it possible for mods to add new UI elements to the HUD. 
- *Main files*: HUDFramework 1.0f

##### [Power Armor HoloHUD](https://www.nexusmods.com/fallout4/mods/29969) *v1.1*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
 This will replace ridiculous half transparent... whatever it is with something much nicer. 
- *Main files*: PA HoloHUD

##### [HUD Plus Plus](https://www.nexusmods.com/fallout4/mods/27218) *v1.1.0*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
 This mod adds some UI widgets to HUD to display detailed information of object crosshair points to or selected in quick loot menu, it also provides some extra features to make player play holotape and read book directly from quick loot menu without need to open inventory while looting. 
- *Main files*: HUD Plus Plus

##### [ApeHUD](https://www.nexusmods.com/fallout4/mods/30294) *v1.0*
<span style="background-color:#00aedb; padding:3px;"><font color="white"> Optional </font></span>
In CtGW main archive there are two version:
- **standard**: some UI elements removed and the rest resized and move towards the edge of the screen
- **lean**: same as above but also compass, enemy health and notifications turned off

##### [Clean HUD 2 - Immersive DEF_UI Presets](https://www.nexusmods.com/fallout4/mods/9441) *v2.0.0*
<span style="background-color:#00aedb; padding:3px;"><font color="white"> Optional </font></span>
 You like immersive things, eh? Well I've got 13 different presets for DEF_UI right here... 
 - *Main files*: All-in-One FOMOD Installer

##### [Immersive HUD](https://www.nexusmods.com/fallout4/mods/20830) *v3.0*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
 HUD when you need. Hide when you don't. 
- *Main files*: Immersive HUD - iHUD

##### [Ruddy88 ́s Simple Sorter](https://www.nexusmods.com/fallout4/mods/33983) *v1.0*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
 Simple Sorter is a FO4Edit script that will automatically add the text needed for icon replacements for all valid items in your entire load order. It automatically scans your mod list, loads all valid items to a new ESP, then detects what sort of item it is so that the correct icons are used. No more patches, no more manually patching. 

- *Main files*: R88SimpleSorter_XML

> Go to the RSS files and first download R88SimpleSorter_SCRIPT. Extract the file menu
> manually into your F04edit folder.
> Now download MXPF - Mator's xEdit Patching Framework, and repeat the process from
> above.
> Next, install in MO2 R88SimpleSorter_XML.
> Finally, we will do the actual patching. Note that it ́s recommended that you deactivate all
> plugins related to Sim Settlements in the right pane before starting the patching process.
> 
> 1. Open FO4Edit, and click OK. Holdiing shift while clicking ok will load the program quicker. Wait for thr background loader to finish.
> 2. Right-click on any of the plugins in the left pane and select "Apply Script".
> 3. In the Apply Script dialogue, click in the script box and navigate to R88_SimpleSorter. Click OK.
> 4. In the first dialogue box, check your options as below:
> 5. Click on New Patch. You can name your sorting file whatever you want, I name it CtGW – simple sorter
> 6. Let the sorter do it ́s job (which only takes a couple of minutes on my rig. When it ́s done, you will get a popup message saying "Patching Complete".
> 7. Close FO4Edit, make sure your new plugin is selected.
> 8. Put your newly created patch last in the right pane of MO2. We ́re done
> 

##### [Clock Widget - Show Real Time While Loading](https://www.nexusmods.com/fallout4/mods/26759) *v1.4.0*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
 This mod adds a clock widget to loading menu, main menu and fader menu to display current real time while loading.How much time did you spend on loading? 
- *Main files*: Clock Widget

> You can change this setting in `ClockWidget.ini` to toggle on/off 24-hour clock: `iEnable24HourClock=1/0`.

##### [Satellite Color World Map Combo](https://www.nexusmods.com/fallout4/mods/9414) *v1.3*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
 Combines Satellite World Map and Color Map. No ESP required. New features included. 
- *Main files*: Satellite Color World Map Combo 1-3

During installer choose:

- No Special

##### [Nuka World Sattelite Map](https://www.nexusmods.com/fallout4/mods/32456) *v1.0*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
Also install maps for Nuka-World and Far harbor and Zoom-out Extended (half-sized
markers) and make sure to merge them with the main mod. I had issues when installing
them as separate mods for some reason.

##### [Far Harbor Satellite Map](https://www.nexusmods.com/fallout4/mods/30966) *v1.1*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
Pip-boy Far Harbor Satellite Map. 2K and 4K. 

##### [Zoom-out Extended Unofficial for1.7.9 Large or Halfsize Icons 2k-4k-8k](https://www.nexusmods.com/fallout4/mods/13989) *v2.0*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
 Icons are double size.

##### [Crafting Highlight Fix](https://www.nexusmods.com/fallout4/mods/27479) *v1.8.6*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
 A F4SE plugin that allows you to disable the hardcoded, vision-obscuring shader effect at various workbenches so you can actually see what you're crafting. Also allows you to change the shader effect for the Power Armor station and robot workbenches to a outline-only shader instead of a full shader. 

##### [No more hold v to enter workshop](https://www.nexusmods.com/fallout4/mods/19996) *v1*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
 This removes the "hold V" to enter workshop menu that is constantly in the upper left corner of your screen. 

##### [Loading Screen Spoiler Remover](https://www.nexusmods.com/fallout4/mods/30594) *v0.666*
<span style="background-color:green; padding:3px;"><font color="white"> Core </font></span>
 Removes the Spoilers from the Loading Screen. You can still see the pretty models and spin them around. This just edits one .swf file (interface file) and does not activate an .esp (or any mods) so it is 100% achievement friendly. 

## Settlements

##### [Workshop Framework](https://www.nexusmods.com/fallout4/mods/35004) *v1.1.7*
 Framework to open up the settlement system to editing by the community.
For Players: New controls and faster, more stable workshop scripts.
For Modders: Add new resource types, override settings, and generally change the way settlements work dynamically. 

##### [Workshop Plus](https://www.nexusmods.com/fallout4/mods/35005) *v1.0.5*
 Transforms Workshop mode into a God simulator - giving you all of the tools you need to create amazing settlements.
Flight, Undo Buttons, Layers, Cloning Tools, and more! 

##### [All Setlements Extended](https://www.nexusmods.com/fallout4/mods/25316?tab=description) *v2.0.2*
 Every vanilla settlement now has a larger build area with custom border wall. Except Home Plate. Screw Home Plate. A must-have for Sim Settlements. 
 
> Download and install No Bunker Hill or Hangman's Alley main version

##### [Uncapped Settlement Surplus](https://www.nexusmods.com/fallout4/mods/12430) *v2.0.1*
 Makes settlements produce surplus (water, food, etc) even if there's already surplus in the workbench 

##### [Faster Workshop (Workshop Lag Fix)](https://www.nexusmods.com/fallout4/mods/35382) *v1.1*
 Faster Workshop is an F4SE plugin that optimizes workshop loading times by replacing some of the most expensive and inefficient regions of workshop loading code with far more efficient versions. Also provides a hotkey to instantly enter Workshop mode and fixes workshop icon load lag. 

##### [Quieter settlements](https://www.nexusmods.com/fallout4/mods/2819) *v0.30*
 Settlements too noisy? This mod reduces the volume of generators, turrets, and other settlement sounds. Choose different volumes for different sounds. 

##### [Locksmith](https://www.nexusmods.com/fallout4/mods/12454) *v1.02*
 Tired of those pesky settlers walking in on you while you're using the bathroom? Worried Piper's going to find your copy of the Lusty Argonian Maid? Well, worry no longer! Now you can lock (and unlock, but why would you ever want to do that?) any door or container you wish! 

##### [Basement Living](https://www.nexusmods.com/fallout4/mods/10967) *v1.3*
 Basement Living adds 10 standalone basement & bunker player homes with their own workshops and craftable doors, allowing you to place/enter into them from any settlement! Just like Home Plate, you can scrap and decorate them how you like. This was done carefully and methodically, does not affect settlements, or require any batch files / workar 

##### [Basement Living-Immersion Adjustment](https://www.nexusmods.com/fallout4/mods/28942) *v1.0*
 An small .esp edit which changes the crafting requirements of the Basement Living doors to be more realistic and cleans out the unimmersive clutter objects found in the bunkers themselves. 

##### [The Master Plan](https://www.nexusmods.com/fallout4/mods/16626) *v2.2*
 Master categorization plugin for all my mods. 

##### [Vanilla Extensions](https://www.nexusmods.com/fallout4/mods/10032) *v2.5a*
Improves vanilla snapping and adds a variety of highly functional blocks to the workshop menu. 

>Install main file and any update file

##### [This is MY Bed](https://www.nexusmods.com/fallout4/mods/7399) *v3*
 Adds six (or 13) craft-able beds that settlers cannot sleep in...but you can. 

##### [Better Cooking Stations](https://www.nexusmods.com/fallout4/mods/12104) *v2.03*
 Overhauls the vanilla cooking stations with better effects and features; adds several new ones including a working kitchen stove, BBQ grill and supermutant cooking pot. All craftable cooking stations can be toggled Private or Public and can be assigned to settlers to function as food traders while still allowing you to craft recipes. 

> Download and install:
> - main file
> - DLC patches


##### [PWR - Passive Water Resources](https://www.nexusmods.com/fallout4/mods/19871) *v1.3*
 Adds 22 water storage items such as tanks, water towers and animated rainwater collectors to build menu. Why passive? Because they generate water points and other bonuses only if your settlement has working "active" water resources (pumps, purifiers, etc.). 

> Install only main file, not the SKE patch

##### [CWSS Redux](https://www.nexusmods.com/fallout4/mods/14326) *v2.1*
 Craftable working showers, baths, toilets, sinks, urinals, bubblers, and kitchens, that followers, settlers, traders and caravan guards can use automatically. Custom idles, models, sounds and visual FX. Automatic undressing/dressing. Immersive buffs that taper over time. 

> Essential to this modlist if you ́ve also installed “Get Dirty”
>{.is-success}

##### [Lore Friendly Posters](https://www.nexusmods.com/fallout4/mods/7145)*v1.0*
 Adds 100 Posters for your decorating pleasure. Lore Friendly. 

> Install mod, and then the Wasteland and Contraptions Workshop and disappearing Mesh Fix
patches

##### [Workshop Rearranged](https://www.nexusmods.com/fallout4/mods/16181) *v0.6.13*
 New items and functionality for the Fallout 4 Workshop. 
 
> Install main file and patch pack
> during installation of patch file, select:
> Required patches
> - Lore friendly posters – Replacer (after install, move replacer after WRA)
> - Master Plan – Standalone
> 
> Optional patches
> 
> - Atomic radio – standalone
> - Beantown interiors – standalone – DEF_UI
> 
> Creation club
> 
> - your choice

##### [Master Plan WRA Patch](https://www.nexusmods.com/fallout4/mods/16626) *v2.2*
 Master categorization plugin for all my mods. 

##### [Better Stores](https://danielgamache.wixsite.com/awarhero/mod-archive) *v1.3.5*
> During installation, select:
> - Extra Custom Props
> - Far Harbor patch

##### [Better Vendor Stalls](https://www.nexusmods.com/fallout4/mods/9758) *v3.2*
 Makes vendor stalls small enough to fit under ceilings and adds clutter for more realism. 

> During installation, select standalone with clutter

##### [Manufacturing Extended](https://www.nexusmods.com/fallout4/mods/15429) *v1.4*
 Improves the manufacturing devices from Contraptions Workshop. Now you can choose which armor parts to build, manufacture Vault jumpsuits and energy weapon ammo, and extract components from workshop inventory! 

> Install main file and Far Harbor patch

##### [Thematic and Practical](https://www.nexusmods.com/fallout4/mods/16207) *vAlpha1.3*
 Thematic and Practical is a mod that aim to provide new constructible objects for your workshop. The plan is to update it with new themes during the developement. 
> Install main file and DLCpatch

##### [Creative clutter](https://www.nexusmods.com/fallout4/mods/20782) *v2.1*
 Fun, awesome, cluttery bits that make your shack, mansion, or giant hippie commune feel like a real home. Lazy furniture, mini crafting stations, standalone decorations, and micro horticulture! Decorate your place like a pro. This mod adds over 800 decorations, furniture, food resources, and more for you to build using its own custom menu. 

> During installation, select Creative Clutter DLC

##### [Do It Yourshelf](https://www.nexusmods.com/fallout4/mods/14532) *v1.6a*
 Add your own clutter to those empty shelves 

> During installation, select extra half-shelf clutter full cost

##### [Gruffydds Signs and Posters](https://www.nexusmods.com/fallout4/mods/9711) *v4.00a*
 Hundreds of new custom stand-alone signs and posters to add to your settlements. Includes settlement name signs for the Minutemen, Brotherhood of Steel, Institute, and Raiders, shop and business signs including some for Level 4 Shops, plus many, many more signs and posters of different sizes, shapes, and subjects, with regular updates adding more. 

> Install main file only

##### [g2m Workshop](https://www.nexusmods.com/fallout4/mods/17088) *v6.1.1*
 Add ton of unique objects to the workshop. Expand workshop features. Fix bugs in workshop items. 

> During installation, check Main version [default]. If you during the intro sequence (right before the bathroom scene) get a white screen, press enter, downarrow and enter again. It ́s a message box spamming the screen at startup.

##### [Organized Workbench Menu](https://www.nexusmods.com/fallout4/mods/32588) *v1.2.1*
 Organizes workbenches by type in the workshop menu. 

##### [JP Guard Towers](https://www.nexusmods.com/fallout4/mods/36178) *v1.21*
 Adds 6 guard towers, 3 bridge decks to connect towers, 2 different style stone steps, and a “Guard Mat” to assign settlers as guards 

##### [Woody's Wasteland Stuff](https://www.nexusmods.com/fallout4/mods/24951) *v4*
 An improvised barrel fireplace to keep you toasty warm and various other wasteland stuffs. 

##### [Private Area Markers (keep settlers out of your house)](https://www.nexusmods.com/fallout4/mods/26377) *v1.1*
 Keep settlers out of your house 

##### [Timer Power Switch](https://www.nexusmods.com/fallout4/mods/10750) *v1.00*
 This mod adds 3 new timer power switches to workshop Power/Connectors && Switches category, which allows you to build power switches automatically power on/off. 

##### [Weapon Rack Extended](https://www.nexusmods.com/fallout4/mods/15729) *v1.3.1*
 Adds short weapon racks that can display all: Small and Medium weapons. and more
Made For Immersion! 

##### [Weapon Rack Fixes](https://www.nexusmods.com/fallout4/mods/19324) *v1.1.1*
 Allows you to put all weapons on Contraptions Workshop Weapon Racks. 

##### [Settlement Objects Combined](https://www.nexusmods.com/fallout4/mods/36461) *v1.6.2*
 Combines the the invidiually themed settlement objects into one file 

> load esp version 2 (loose files)
> If you use the get Dirty mod we will want to make the showers from this mod compatible.
> - Open F04Edit. Select both "Get Dirty" and "Settlement Objects Combined" and click ok.
> Only those 2 should be selected.
> - Once loaded, Right Click on SOC, and click "Add Master" > select "Get Dirty".
> - Expand Spells then click on "SShowerBetterEffect"
> - Replace the 'DamageradiationWater' Effect with the CS7_DirtTier00 'Clean'" Effect (which
> is what is triggered when you swim in the Get Dirty mod, for example).
> - Repeat for SShowerBasicEffect
> - Close and Save the "Showers" mod, as that is the only mod you've edited.

##### [Settlement Tidy bot](https://www.nexusmods.com/fallout4/mods/33217) *v2.1*
 Mr. Tidy "undertaker bot" that scurries around removing "remains" from a Settlement 

##### [Settlement Menu Manager](https://www.nexusmods.com/fallout4/mods/24204) *v0.1.4*
 SMM provides an easy way to add custom menus and makes said menus automatically disappear on uninstall (without breaking your build menu!) 

##### [Sim Settlements](https://www.nexusmods.com/fallout4/mods/21872) *v4.1.0*
 Settlers should build their own damn houses (and farms, and shops, and...), you've got a Commonwealth to explore! 
 
> Install 3 in 1 version
> Allows you to build zone objects that tell the settlers what type of buildings to create in
> different areas of your settlement and they will do so. Includes a progression system, a more
> interesting settler needs system, and rewards to help settlements matter more. This mod aims
> to completely change the way you think about settlements. You'll now be able to create
> detailed, living places with minimal effort.
> The ultimate goal: making every settlement a unique and awesome looking Fallout city, with
> perks and rewards that help you at every stage of the game.

##### [Sim Settlements Mega Pack - Year One](https://www.nexusmods.com/fallout4/mods/30396) *v1.0.5*
 Over 100 building plans from throughout the community for Sim Settlements!
Includes 11 brand new building plans that will unlock based on the DLC you have! 

##### [Sim Settlements Mega Pack - Year Two](https://www.nexusmods.com/fallout4/mods/37983) *v1.0.1*
 Over 100 building plans from throughout the community for Sim Settlements! 

##### [Sim Settlements – Conqueror](https://www.nexusmods.com/fallout4/mods/37000) *v4.1.0b*
 It's time to take the settlements to War.
Includes
- Option to prestart the game with pre-built settlements run by NPCs for you to explore and Conquer.
- Convert settlements to military outposts for your favorite factions and run attacks with them.
- Quest line to play as a Raider.
- New Sim Settlements content. 

##### [Sim Settlements Conqueror Faction Pack - The Forsaken Vaulters](https://www.nexusmods.com/fallout4/mods/38425) *v4.0.6-B*
 Adds the Forsaken Vaulters as a faction for the Sim Settlements expansion Conqueror. Better served cold! 

##### [Sim Settlements - Building Plan Preview](https://www.nexusmods.com/fallout4/mods/26004) *v2.0*
 This mod ads a 3d preview model of each building plan on Sim Settlements, Industrial Revolution, Rise of the Commonwealth and it's addons so you now know what you are actually building, and they look great too.
> Download and install Newest main file, and the Mega pack – year one file.
> Apart from the Sim Settlement add-ons we ́ve already installed, this mod also covers
> Wasteland Venturers v7.1.1+, Always Free Sim Settlements MrJoseCuervo v1.3.2+ ,
> Industrial City v0.9.0+, Junk Town by uituit v9+

##### [Sim Settlements - IDEK's Logistics Station](https://www.nexusmods.com/fallout4/mods/28945) *v1.2.3b*
 Designed to simplify general logistical concerns, this mod adds an Industrial plot that automates the creation of supply lines, improves inter-settlement resource sharing and more. 

##### [Wasteland Venturers 2 All-In-One](https://www.nexusmods.com/fallout4/mods/30081) *v6.0.0a*

##### [Place Everywhere](https://www.nexusmods.com/fallout4/mods/9424) *v1.18.0.1138*
 Place/build objects in settlements everywhere you want, change objects whatever you like. No more RED! 

## Cosmetic overhauls

##### [BodySlide and Outfit Studio](https://www.nexusmods.com/fallout4/mods/25) *v4.7.4*
 An easy to use tool for customizing bodies and outfits, creating new bodies and outfits, and converting outfits between body types. 

##### [LooksMenu](https://www.nexusmods.com/fallout4/mods/12631) *v1.6.16*
Adds engine modifications to improve character creation.

##### [Looksmenu Customization Compendium](https://www.nexusmods.com/fallout4/mods/24830) *v10*
 A mod that adds hundreds of new options to customize your character such as face paint, tattoos, scars, makeup, brows, haircolors, etc~! 

##### [LooksMenu Body Tattoos](https://www.nexusmods.com/fallout4/mods/25000) *v1.3.2*
Some tattoo overlays for LooksMenu. It doesn't at all require Unique Player, and works more or less out of the box. A lot of customization is possible. 

##### [FSM Body Textures](https://www.nexusmods.com/fallout4/mods/31965) *v5.0.1*
Female texture customizer for CBBE. Customize blemishes, tanlines, hair, and more... all with an easy-to-use installer! 
>  Download the first main file and install it.
> During the Installer, click next till on the fourth panel and select Neck and Scalp
> Adjustament option only. In the fifth panel select all Valkyr options, then click next and
> select finish.

##### [Picturesque Presets](https://www.nexusmods.com/fallout4/mods/16788) *v2.999a*
 A compilation of Mystolle's LooksMenu Presets 

##### [Caliente's Beautiful Bodies Enhancer -CBBE-](https://www.nexusmods.com/fallout4/mods/15) *v2.6.2*
 The well-known body enhancer made famous in Skyrim is back for Fallout 4 debut

##### [Malestra's CBBE BodySlide Preset Collection](https://www.nexusmods.com/fallout4/mods/35316) *v1.0*
 This is a collection of 40+ very accurate presets BASED ON REAL WOMEN or erotic fantasy art characters for CBBE/BodySlide. With variations it is about 120 presets total. Follow INSTALLATION instructions, check the STICKY And please post screenshots! 

## Clothing

##### [Modular Road Leathers](https://www.nexusmods.com/fallout4/mods/29779) *v1.1*
 Several new outfits for male characters based on the road leathers. Multiple layers with each offering additional customization's. Oh, and it fixes "armor bloat". 

##### [Commonwealth Shorts – CBBE](https://www.nexusmods.com/fallout4/mods/7898) *v2.0*
 Sixteen new craftable commonwealth short outfits! And seven new S.P.E.C.I.A.L. outfits. :) 

> Install CBBE main file an the tight armors optional file, then install bodyslide from here.

##### [Shade Girl Leather Outfits – CBBE](https://www.nexusmods.com/fallout4/mods/32547) *v1.0*
 Rock on! A one-of-a-kind small collection of highly customizable female leather outfits mashups built around freedom of choice. Customize every piece of the outfit at the armor workbench, then mix and match with other mods to your heart’s content, for that unique look you aim for! 

> Install main file and bodyslide hotfix file

##### [Raider Themed Mashups](https://www.nexusmods.com/fallout4/mods/29503)*v1.1*
 Adds 5 customizable raider themed outfits. Female only. 

##### [Badlands Mashups](https://www.nexusmods.com/fallout4/mods/30013) *v1.2*
 The third set of my personal mashups with 9 outfits included for female characters. This time, I find out how awesome suspenders look. 

##### [Commonwealth Mashups](https://www.nexusmods.com/fallout4/mods/27776) *v1.1*
 My personal armor mashups, now for your female characters too! 
 
##### [Wasteland Mashups](https://www.nexusmods.com/fallout4/mods/28099) *v1.1*
 The second set of my personal outfit mashups - this time, we mash harder. 

##### [Irradiated Raiments](https://www.nexusmods.com/fallout4/mods/34193) *v1.0*
 My fourth set of mashups for female characters with 8 outfits and 3 recolors for each included. This time, I figure out how material swapping works. 

> Install main file and Boston Belle Belt Hotfix for CBBE

##### [Spiff's Wasteland Clothing Pack](https://www.nexusmods.com/fallout4/mods/31129) *v0.5*
 A collection of all of my armor mashups, with a few unreleased ones thrown in. All easily and accessible through the Wasteland Clothing Station 

## Armor

##### [Eli's Armour Compendium](https://www.nexusmods.com/fallout4/mods/22431) *v1.5*
 Mod ads 50 new lore-friendly armours, 20 accessories, tons of moddable colours. Institute, Settler, Wastelander, Raider, Vault suit. Both sexes. Vanilla and CBBE body, with BodySlide compatibility. 

> Download and install CBBE main file

##### [The Mercenary Pack](https://www.nexusmods.com/fallout4/mods/20088) *v0.9c*
 My Outfit pack that contains all of my previous work (B-90, Rebel, SNCR) plus a new Gunner overhaul and Wastelander outfits that fits for exploring the commonwealth. 
 
> Download and install:
> - The Mercenary - Pack v0.9b – loose files
> - The Mercenary - Pack v0.9.c - plugin only update
> there are optional, though reportedly a bit buggy, BodySlide files available for those who
> intend to use BodySlide to custom fit armor to their characters body.
 
##### [West Tec Tactical Optics](https://www.nexusmods.com/fallout4/mods/12220) *v2.0.1*
 Night Vision / Thermal / Targeting HUD goggles and eyepieces with new meshes and HD textures. Fully modular, craftable, upgradeable. 3 vision effects, 8 colors, and 2 additional targeting enhancements. Schematics posters also in the Workshop! 

> Download and install:
> - West Tek Tactical Optics v2.0.1 (minor update)Revision 2.5.0 alpha 2
> - West Tek Tactical Optics v2.0 - AWKCR
> - West Tek Tactical Optics v2.0 - Standard Leveled Lists

##### [PreWar Binoculars](https://www.nexusmods.com/fallout4/mods/17819/) *2.1.1*
 Adds functional binoculars to the game. 
 
> Adds functional binoculars to the game.
> During install, select:
> - “Binoculars – AWKCR” and 
> - “Standard viewfinder”

##### [Crimsomrider's Accessories](https://www.nexusmods.com/fallout4/mods/19563) *v5.0*
 A fully modular and customizable accessory mod for both male and female, with a ton of accessories that enable you to achieve a unique look.
The customization options are endless. 

##### [Tactical Flashlights](https://www.nexusmods.com/fallout4/mods/16172) *v2.3*
 Adds wearable flashlight gear to the wasteland.
- 8 Unique models
- 10 Distance settings
- Craftable bulbs
- Dynamic shadows
- Volumetric light
- Automatic leveled list integration 

> During install, select:
> - AWKCR+AE
> - 100% + shadows

##### [K-9 harness](https://www.nexusmods.com/fallout4/mods/17686) *v1.0*
 New modular body armor with new meshes & textures for Dogmeat, designed after modern Military and Police K-9 gear. Craftable side pouches, backpack, ballistic weave, faction patches, and various colors and patterns customized at the standard workbench. Lots of options! 

> download:
> - K-9 Harness - Tactical Body Armor and Backpack for Dogmeat
> - K-9 Harness - Armorsmith Extended plus DEF UI

##### [CROSS Pre-War Cybernetics](https://www.nexusmods.com/fallout4/mods/8609) *v106c*
 Fully customizable cybernetic armor, unique armor mods, palette based paint styles, size options and more. ROBOT HANDS. 

> download main file only

##### [CROSS Institute Tech Mask](https://www.nexusmods.com/fallout4/mods/11881) *v1.02*
 Adds a high tech gas mask that protects without hiding your characters face! 

##### [CROSS Brotherhood Recon](https://www.nexusmods.com/fallout4/mods/27418) *v091b2*

##### [CROSS Chosen of Atom](https://www.nexusmods.com/fallout4/mods/37820) *v091a*

##### [CROSS Courser Strigidae](https://www.nexusmods.com/fallout4/mods/28009) *v090c*

##### [CROSS Institute Expeditionary suit](https://www.nexusmods.com/fallout4/mods/30857) *v090b*

##### [CROSS Mojave manhunter](https://www.nexusmods.com/fallout4/mods/32214) *v090d*

##### [Wearable Backpacks and Pouches](https://www.nexusmods.com/fallout4/mods/3258) *v1.4b*
 This mod adds craftable & upgradable backpacks & pouches. 

> Install main file and the AWKCR Crafting optional patch. These clothes and armors need to be run through Bodyslide if you ́re using a bodyslide preset other than the CBBE vanilla one. 
> For instructions on how to do this, I will refer to the ever excellent Gopher on YouTube. I recommend you watch the whole video, but for this step, you can skip to timestamp 09:53.

## Power armor

##### [Enclave X-02 Power Armor](https://www.nexusmods.com/fallout4/mods/11017) *v0.401*
 The X-02 Power Armor wielded by the forces of the Enclave in the Capital Wasteland. Now in the Commonwealth! 

##### [Hellfire X-03 Power Armor](https://www.nexusmods.com/fallout4/mods/26251) *v0.126*
 The intimidating Hellfire Power Armor from Fallout 3's Broken Steel DLC, finally lands in the Commonwealth.
Now patched to 0.126 

##### [InstitutePowerArmor](https://www.nexusmods.com/fallout4/mods/18315) *v* 
Institute Power Armor I-01 

##### [Tribal Power Armor](https://www.nexusmods.com/fallout4/mods/22437) *v1.0*
 Adds the iconic custom T-45d power armour worn by Ashur of The Pitt in Fallout 3's DLC to the Commonwealth, along with some groups of Pitt Raiders. 

##### [Standalone Construction Power Armor](https://www.nexusmods.com/fallout4/mods/12096) *v3.0*
 The same PA from my scavvers mod now standalone for easier enjoyment. 

##### [Liberty Power Armor](https://www.nexusmods.com/fallout4/mods/16305) *v2.2*

##### [Submersible Power Armor Redux - BioShock Inspired](https://www.nexusmods.com/fallout4/mods/25591) *v1.2*
 Daddy's back, and better than ever! Take a trip to Rapture to get yourself a brand new suit of fully customisable Submersible Power Armor, a Big Sister outfit and some new settlement items! 

##### [Some assembly required](https://www.nexusmods.com/fallout4/mods/12050) *v1.4*
 Remember when you found a full set of X-01 in the back of a train car three times in a row? Leveled Power Armor tends to do that. This mod manually removes nearly every Power Armor spawn in the game and makes Power Armor exceedingly rare and difficult to acquire. Just as it should be. 

##### [Some Assembly Required Patches for X-02 and X-03 Pas](https://www.nexusmods.com/fallout4/mods/26739) *v1*
 Makes SAR changes to the X-02 & X-03 PAs. 

##### [Improved Jetpack Flight Model](https://www.nexusmods.com/fallout4/mods/34249) *v1*
 Improved Jetpack Flight Model. Fly further, Fly longer, Fly higher but slower with lower AP use. 

##### [Restore Power Armor Frames](https://www.nexusmods.com/fallout4/mods/20890) *v1.1*
 The mod allows you to restore power armor frames from dead bodies on the spot, separating the frame from the body. 

##### [Power Armor Impact FX](https://www.nexusmods.com/fallout4/mods/34012) *v1.5*
 Power Armor now has more interactive impact FX to things like metal objects to adding a more bad ass power armor hard landing and more SCRIPT FREE. Gif animations in the description. 

## Weapons of lore

##### []()

## Gameplay

##### [Unbogus Fallout overhaul](https://www.nexusmods.com/fallout4/mods/26026) *v2.Final*
 An extensive overhaul that touches upon almost every aspect of the game which aims to make the game more fun, challenging in a good way and varied while rewarding skill and tactics. 

> Install main file only.

##### [BS Defence](https://www.nexusmods.com/fallout4/mods/20137) *v1.8*
 Better Settlement Defence - Makes those hundreds of turrets actually do something when you're not around by taking away the random aspect of settlement attacks. 

##### [More Attackers – Get off my Buildzone](https://www.nexusmods.com/fallout4/mods/27465) *v1.1.7*
 Moves attack markers beyond the boundaries of settlements. Adds additional attack markers around the perimeter of settlements. Solves the problem with spawning enemies inside a settlement after fast travel. Adds notifications to animals attacks. Increases time before attacks auto resolve (configurable). And more... 
> Install main file

##### [Night Of The Creeps](https://www.nexusmods.com/fallout4/mods/23721) *v0.213*
 Adds a new type of Feral ghouls that hunt at night. Flees and hides during the day. Optional Yao Guais. Settings holotape. 
 
##### [Sleepless Nights](https://www.nexusmods.com/fallout4/mods/33057) *v1.01*
 A simple mod that makes it unsafe to rest in uninhabited areas at night. Your sleep can be interrupted by an enemy ambush or any number of wasteland creatures. 

##### [Shaikujin's Better warning for settlements being attacked](https://www.nexusmods.com/fallout4/mods/4106) *v5.1*
 Changes the 2 second message when a settlement is attacked to a standard message box (see screenshot). 

##### [Pack Attack NPC Edition - Gangs With Group Combat Tactics](https://www.nexusmods.com/fallout4/mods/30140) *v1.79*
<span style="background-color:#ff8b94; padding:3px;"><font color="black"> HD-HQ </font></span>
 "Pack Attack: NPC Edition" applies social combat AI to NPC gangs. Rather than simply rushing you in the open as a group, these NPCs will break and cover, retreat and flank, run and hide, and even lie in wait. They're more likely to ambush, less likely to engage in suicidal charges, and more willing to switch to hand-to-hand combat when needed.
 
> This mod is heavy on script resources and might cause game instability, especially if
> adding further scripted mods on top of this list.
>{.is-success}

##### [H.A.R.D.Core - Fusion Generator Overhaul](https://www.nexusmods.com/fallout4/mods/28890/) *v1.0*
 Replaces all Fusion Cores in Generators with plausibly drained FCs. 

##### [QuickTrade](https://www.nexusmods.com/fallout4/mods/16229) *v1.3*
 Quicktrade with vendors and settlers. 

##### [Auto Eat and Drink in Survival](https://www.nexusmods.com/fallout4/mods/25408) *v1.3.1*
 Auto Eat and Drink in Survival 
 
##### [Grab and Eat All-in-One](https://www.nexusmods.com/fallout4/mods/17608) *v1.5*
 NEW FEATURE Player can read notes from containers and corpses.
Add EAT/DRINK/USE choices that let you grab the item and eat/drink/Use in real time without picking up and opening the inventory 

##### [Read Notes from Containers and Corpses](https://www.nexusmods.com/fallout4/mods/18077) *v1.0*
 With this mod, player can read notes right from containers and corpse. 

##### [GET DIRTY (take a bath)](https://www.nexusmods.com/fallout4/mods/29171) *v1.3*
 Get dirty while exploring the wasteland. Take a bath to get clean again. 

##### [GET DIRTY (take a bath) additional effects](https://www.nexusmods.com/fallout4/mods/36880) *v1.0*
 This little patch for 7StarC's GET DIRTY mod adds charisma modifiers and some other minor tweaks to the original mod. I made several flavors to accomodate your preferences. 
##### [Canteens of the commonwealth](https://www.nexusmods.com/fallout4/mods/24493) *v1.0.5*
 Adds New standalone and Wearable Canteens to the game that you can craft and fill with water.
(Now with an installer) 

##### [Fill'em Up Again (Dynamic Bottle Recyclation)](https://www.nexusmods.com/fallout4/mods/12674) *v1.0*
 Dynamically gives you an appropriate empty bottle whenever you drink a bottled beverage. Since it works via a simple script, it should be compatible with any mods even if they edit/rebalance/rename drink items. 

> Install loose files version

##### [Intimidation Overhaul](https://www.nexusmods.com/fallout4/mods/23922) *v2.0.10*
 Overhaul of the Intimidation perk adding many new options as well as the return of the Mesmetron from Fallout 3. 
 
##### [Critical Hits Outside of VATS Revisited](https://www.nexusmods.com/fallout4/mods/25583) *v1.2.2b*
> Install main and worse criticals optional files.

##### [Hacking 101](https://www.nexusmods.com/fallout4/mods/15033) *v2.3*
Major rework of the Hacking system.

##### [Salvage Robot Parts](https://www.nexusmods.com/fallout4/mods/25355) *v2*
 Robots now has a chance to drop appropriate robot parts. For people who likes to scavenge for their robot parts instead of building from scratch. 
 
##### [Sofa Surfer - Sleeping on Couches](https://www.nexusmods.com/fallout4/mods/24944) *v1.1*
 Adds option for player to sleep on couches, and rest on chairs. 


##### [SKK Combat Stalkers (hostile spawns)](https://www.nexusmods.com/fallout4/mods/30308) *v022*
 SKK Combat Stalkers brings the UNCERTAINTY, FEAR and EXCITEMENT to you, randomly spawning small groups of properly levelled hostiles around you who hide and ambush, stalk, or chase depending on your actions. 

##### [RSE Elements Vol.3 - Karma System feat. Bounty Hunters](https://www.nexusmods.com/fallout4/mods/36020) *v1.6*
 Adds a simplified Karma System to Fallout 4 where game stats are tracked for various activities and alter your moral stance within the game, leading to confrontations and possibly jail time by bounty hunters. External mods can now hook into the Karma System via custom API (included), extending my Karma System to any mod that wishes to tie into it! 

##### [Outfit Switcher](https://www.nexusmods.com/fallout4/mods/10282) *v2.2*
 In a first of its kind for Fallout 4, this mod lets you save your entire loadout, including armor pieces! Then equip and swap between saved loadouts with the press of a button. You don't even need to open your Pip-Boy! It's like favorites, but entire loadouts at a time. 

##### [I Ain't Drunk (I'm Just Drinking)](https://www.nexusmods.com/fallout4/mods/36888) *v1.1*
 Now you can drink one beer without getting drunk.
And now beer restores thirst. 

##### [First Person Death Cam](https://www.nexusmods.com/fallout4/mods/27537) *v5*
 This mod makes you die in first person, with lots of different IMOD, global time multiplier, and decapitation combinations that are chosen randomly by a script on death. This makes for over 100 different first person death cams! 

##### [Survival options](https://www.nexusmods.com/fallout4/mods/14650) *v1.7.1*
Adds a holotape that allows you to choose various options for survival difficulty, including hunger, thirst and exhaustion rate. 

> Install version 1.6.2, the version before MCM, as it reportedly works better.

## NPC and creature overhauls

##### [Raider Overhaul](https://www.nexusmods.com/fallout4/mods/9103) *v11.4c*
 A functioning WIP mod focusing on adding more diversity to the Commonwealth's Raiders. 
 
> Install Raider Overhaul WIP 11.4c optional file only, then install AE replacer Raider Overhaul 11.4c from the Armorsmith Extended files.

##### [D.E.C.A.Y – Better Ghouls](https://www.nexusmods.com/fallout4/mods/2500) *v2.2*
 D.E.C.A.Y is a pretentious non-abbreviation that is used for my awesome feral ghoul overhaul. Ghouls are now creepy and unpleasant and have lots of detail and variety. No more bland, patternless leathery old men. 
> Install main file only

##### [Deadlier Deathclaws](https://www.nexusmods.com/fallout4/mods/13822) *v3.3.5*
 An upgrade to the dragons of the wasteland to be more in line with their legend. 

##### [Unique NPCs - Creatures and Monsters](https://www.nexusmods.com/fallout4/mods/24357) *v2.1*
 Unique NPCs - Creatures and Monsters of the Commonwealth
A new... non-replacer way to introduce exceptional variety to the Creatures of the Wasteland. 

> Install main file and any updates/fixes
> During installer choose
> - DECAY
> - Deadlier Deathclaws
> - SMR no patch
> - Respawnable no patch
> - Unique NPCs - C n M – Non-Lore
> The Unique NPCs installer will have replaced a couple of earlier installed esps (edited
> versions to make them cmpatible with Unique NPCs). Those esps will now need to be
> moved below the main Unique NPC esp to work properly. Below is a ist of the esps you
> need to move before moving on to the next mod:
> 
> D.E.C.A.Y.esp
> DeadlierDeathclaws
> make sure that this section of your right pane now looks like this:
> 
> After installation, open Unique NPCs – Creatures and Monsters.esp in FO4Edit expand:
> ```
> Worldspace
> 0000003c
> Block -1, -1
> Sub-Block -2, -1
> 0000E48E
> Temporary
> 001D0F96
> ```

##### [Less Loot D.E.C.A.Y](https://www.nexusmods.com/fallout4/mods/32938) *v1.0*
 Reduce loot from ghouls significantly when using D.E.C.A.Y. mod. 

##### [Feral Ghouls After Dark](https://www.nexusmods.com/fallout4/mods/22434) *v1.0*
 Feral ghouls become significantly more dangerous after the sun goes down - the way proper zombies do. 

##### [Super Mutant Redux](https://www.nexusmods.com/fallout4/mods/11853/) *v2.5*
Reworks the super mutant faction including Behemoths, FEV Hounds, and of course, Super
Mutants.

> Install Super Mutant Redux and any updates. During installer select Armorsmith patch

##### [We are the minutemen](https://www.nexusmods.com/fallout4/mods/6443/) *v6*
 The Minutemen are supposed to be the best alternative for rebuilding the Commonwealth because : More settlements = More resources = Better materials = Better fire power and a larger presence in all the Commonwealth. But currently this is not the case and this mod attempts to fix this problem. 

##### [Far West Minutemen](https://www.nexusmods.com/fallout4/mods/27972) *v2.1*
 This mod enhances the Minutemen to convert them in a more strong background lore faction. Adds a group of minutemen specialist that can spawns individually as others and gives all minutemen dedicated equipment to add a wild west and steampunk touch. 

##### [Militarized Minutemen](https://www.nexusmods.com/fallout4/mods/29853) *v1.1.2*
 Adds over 15 modular military themed items for the minutemen, overhauling the factions with different classes and combat styles. 

> During installer:
> - WATM compatibility

##### [Synth Overhaul – C.A.S.T](https://www.nexusmods.com/fallout4/mods/9525) *v3.0.4*
 This mods overhauls all the Synths by giving them 70 new armor sets, 77 helmets, 42 uniforms and 2 Synth weapons. From damaged armor to undamaged looking armor sets. This is done by editing the vanilla armor pieces, uniforms and weapons with new textures in 2K and 4K. 

> Install the main ba2 version, and any update
> During install select:
> - Synth Overhaul – no weapons
> - AWKCR + AE
> - Remove level requirements (Optional. Synths will be more powerful at lower levels!)

##### [Better Settlers](https://www.nexusmods.com/fallout4/mods/4772) *v2.0*
 Better Settlers is a lore friendly mod that adds more than 240 new settlers to the vanilla settler selections. You can choose to stop there, or further OPTIONS to customize them to spawn with more lore-friendly changes to their equipment, gender ratio, stats, or mortality. DLC and no-DLC versions and many other options available. 

> Install Better Settlers v2.0 DLC Master FOMOD main file
> During install select:
> - Bettersettlers.esp
> - No Lollygagging!
> - Dirty faces
> - Better settlers default
> - Vanilla
> - Community hair and clothing
> - Mortal pack

##### [Simple Settlers](https://www.nexusmods.com/fallout4/mods/36074) *v4*
 A simple settler mod that offers 205 unique settlers to spawn to your settlement. Installation options allow you to choose the mortality of your settlers and your preference of gender. 

> Main options
> - Mortal settlers
> Optional
> - None

##### [Unique NPCs - An Overhaul of the Commonwealth](https://www.nexusmods.com/fallout4/mods/21248) *v2.1*
 An overhaul of Skin textures, Size (height, weight) and Morphology (first time I've gotten to use that word!); with Roughly 180'ish Female Skin Textures, and 120'ish Male Skin Textures, tweaked body morph values, added faces, the commonwealth should be a unique place to visit.
08/21/2018 Update - Full Overhaul for performance and Bugs. 

> Install any of the two mian files (they ́re identical), and the 2.1 update
> FOMOD instructions:
> Core
> - Unique Npcs Core.esp
> - I read this if you don ́t use the HD DLC (which you shouldn ́t anyway)
> Better Settlers and it ́s patches
> - Better Settlers - No LollyGagging
> - Mortal Pack
> - No Patch - Standard Mix
> No Patch - Standard Armor Mix
> Better Settlers - Elis armour compendium - AE
> No patches
> Special Settlers
> - No special settlers
> Minutemen options
> - Militarized Minutemen
> - Far West Minutemen
> - WATM 5.x enhanced
> - none (we are the far west minutemen merged)
> - UniqueNPCs_WATMM_FarWest_MilitarizedMinuetmen.esp
> Gunner options
> - No patches
> 3rd party patches and final otpions
> - Standard mortality
> - Diamond city expansion
> - No settlement patches
> - Unique NPCs_AE_SuperMutantRedux
> - Looks Menu Customization Compendium Replacer
> If the FOMOD installer doesn ́t let you install the DCE patch, then I ́ve added the patch to
> the CtGW R2 archive. Install separately or merge with Unique NPCs doesn ́t matter as long
> as it ́s place after it.
> The Unique NPCs installer will have replaced a couple of earlier installed esps (edited
> versions to make them cmpatible with Unique NPCs). Those esps will now need to be
> moved below the main Unique NPC esp to work properly. Below is a ist of the esps you
> need to move before moving on to the next mod:
> Looksmenu customization compendium
> We are the minutemen
> Far west minutemen
> Militarized minutemen
> Better Settlers

##### [Raider children](https://www.nexusmods.com/fallout4/mods/16586/) *v3.1*
Raiders have been known to abduct children in the commonwealth to replenish their ranks.
Once indoctrinated, those poor children return the world from which they came to pillage
and kill.

##### [FO4 NPCs Travel](https://www.nexusmods.com/fallout4/mods/16987/) *v2.8.1*
This mod adds 338 new NPCs, travelling across the commonwealth

> Install FO4 NPCs Travel main file

##### [Settlers of the Commonwealth](http://3dnpc.com/wiki/fallout-mods/fallout-4/settlers-of-the-commonwealth/) *v3.02*
Adds 30 new recruitable settlers across the commonwealth, from the creator of Tales of the
Commonwealth

##### [Sim Settlements - Settlers of the Commonweath - City Leaders](https://www.nexusmods.com/fallout4/mods/29799) *v1.0*
 Makes all of the settlers from the Settlers of the Commonwealth mod, available on 3dnpc.com, available as city leaders in kinggath's Sim Settlers mod 

##### [Immersive Dogmeat](https://www.nexusmods.com/fallout4/mods/34128) *v1.0*
 Fixes everything that was originally wrong with Dogmeat. Also removes his Max Level Limit. See details! Script-Free! 
> ESP version

##### [Moddable Robot Settlers](https://www.nexusmods.com/fallout4/mods/11976) *v1.16*
 A compilation of my earlier mods that make robot settlers customizable at the Robot Workbench with the Automatron DLC and fixes things like Codsworth not being moddable or Professor Goodfeels' inevitable disappearance from the game.

It's also a framework enabling bot NPC's for other mods like EyeBot Companions or Securitron 

##### [Killable Children](https://www.nexusmods.com/fallout4/mods/197) *v1.2.7.1*
 I made this in Fo4edit (1.2), and it allows you to have children be mortal like any other generic adult npc in the game. There are a couple essential children, i only tracked down 3 so far, if you see any more post there names in the comment box thingy. 

##### [Less Aggressive Settlers](https://www.nexusmods.com/fallout4/mods/36399) *v1.1*
 Makes settlers less aggressive so that they don't charge straight into battle during attacks. Especially useful when combined with Settlement Ambush Kit. 

##### [Grieving Raider - A Most Important Mod](https://www.nexusmods.com/fallout4/mods/32335) *v1*
 The grieving raider, a man hurt by the world. Laying his love to rest only to be jacked up and killed by the Sole Survivor, well no more. 

## Companion overhauls

##### [Valentine REBORN](https://www.nexusmods.com/fallout4/mods/9568) *v2.0*
 VALENTINE REBORN - V2.0 includes a complete HD retexture for Nick and his outfit!
3 different eyecolors available; optional HD eyetextures for all the Gen1+2 Synths and a 4k metal retexture for the Gen1 Synths 

##### [Valentine Noir](https://www.nexusmods.com/fallout4/mods/7551) *v0.2*
 A retexture for Nick Valentines clothes, turning him into a shady detective. 
 
##### [Live Action Mr. Handy](https://www.nexusmods.com/fallout4/mods/9571) *v1.1b*
 The live action trailer had shown Mr. Handy with lighted eyes so I've added spotlights to Codsworth and all Handy models eyes including Gutsy and Nanny. Spotlights also included in all Automatron eyes added in the Robot Workbench under Handy Torso. 

> Install Live Action Handy - With Iris and GlowMap – Repack version

##### [Cait's Corset – Tailored](https://www.nexusmods.com/fallout4/mods/27939) *v1.3*
 Modifies the cut of Cait's corset and jeans to be a little more sexy. Works with CBBE and BodySlide. Includes a version with breast physics. 

##### [Just another Piper Outfit](https://www.nexusmods.com/fallout4/mods/21114) *v1.5*
 My idea of what a nosy reporter would wear. CBBE. Two variations, Replacer or Standalone. Optional Vanilla/EVB Replacer 

##### [CIO - Companion Inventory Overhaul](https://www.nexusmods.com/fallout4/mods/34977) *v1*
 A simple mod that adds more items to each companion's inventory list such as caps, supplies, and other miscellaneous items relevant to the character's backstory. 

## New companions

##### [Tina De Luca Voiced as a Settler (Dependency Revisited)](https://www.nexusmods.com/fallout4/mods/20226) *v1.3*
 Adds over 50 new voiced lines by StrayKitten to fix the NPC as a settler.
Unlocks some hidden game content in Vault 81.
Allows you to recruit Tina outside Dependency even after the quest was already finished... or bugged out. 

##### [Heather Casdin](https://www.nexusmods.com/fallout4/mods/23273) *v1.03*
 From the author of New Vegas' most popular companion mod, Willow - A Better Companion Experience, comes a new, complex companion for Fallout 4. Heather is a story-driven character with over 1200 lines of custom, voiced dialogue, quests, etc. Heather's unique implementation is designed to improve on the FO4 companion experience. 
 
> During install choose "Heather with Extended Dialogue Interface" on the first pane, AE on
the second pane.

##### [Heather Casdin - Assorted Patches](https://www.nexusmods.com/fallout4/mods/24314) *v1.03-XG*
 This mod contains patches made by members of the community to use with Heather Casdin - A Unique Companion Experience by llamaRCA. Current patches available: Full Dialogue Interface, Bhaal's Better Sorting, Valdacil's Item Sorting and Armorsmith Extended 

##### [Ellen - the cartographer](https://www.nexusmods.com/fallout4/mods/15962) *vFinal*
 The very first and truly custom voiced companion for Fallout 4, boasting over 1200 lines of custom made and voiced dialogue. Affinity system, supporting DLC. Romance. Custom quest. Vanilla lore-friendly face and background. 

##### [Buttons – Companion](https://www.nexusmods.com/fallout4/mods/31710) *v1.3*
 Ethan Gombos a.k.a. Buttons is a unique, fully voiced companion you can find near Sunshine Tidings Co-Op. His specialties are stealth and sniping. He currently works for the Minutemen but he'll tag along with you no matter your faction choice. 

##### [I am Darlene](https://www.nexusmods.com/fallout4/mods/36254) *v1.14*
 Darlene. 

## Animations

##### [Laser weapons 1st person reposition](https://www.nexusmods.com/fallout4/mods/23102) *v1.4*
 Makes the institute and standard laser weapons smaller in the 1st person. 
 
> Install Institute and standard lasers main file

##### [Automatically Lowered Weapons](https://www.nexusmods.com/fallout4/mods/20093) *v1.4*
 Lowers your weapon automatically when not in combat 

##### [New Alternative Animations](https://www.nexusmods.com/fallout4/mods/29857) *v1.0Ony*
 Wastelanders these are some alternative animations for your character! come quick! 

> Download and install one big pile of animations optional file

##### [Stay Focused Son](https://www.nexusmods.com/fallout4/mods/18619) *v0.51*
 This is the wasteland don't you dare put your pistol aside, you won't survive long son. 

##### [Power Armor Animation Changes](https://www.nexusmods.com/fallout4/mods/4408) *v1.0*
 Changes the enter and exit animations to be much quicker and an optional "Heroic" empty idle stance. 

## Vanilla location overhauls

##### [Better Goodneighbor](https://www.nexusmods.com/fallout4/mods/16594/) *v1.00*
 Overhaul mode for the Goodneighbor, changes a lot of stuff and adds new voiced npca-s. 

> Download and install main file, update and cleaned esp

##### [Better The Third Rail](https://www.nexusmods.com/fallout4/mods/15388/) *v1.00*
 This mod adds more authentic NPCs and many new details to improve overall The Third Rail atmosphere and immersive gaming experience. 
> Download and install main file, update and cleaned esp

##### [Better Atom Cats Garage](https://www.nexusmods.com/fallout4/mods/14764/) *v1.00*
 Atom Cats Garage with much more details. 
> Download and install main file and cleaned esp

##### [Vault 88 - Your Vault Your Way - Build Ready](https://www.nexusmods.com/fallout4/mods/35076) *v1.12*
 Overhaul - quest safe, build ready, performance optimized. cleaned, restored and expanded areas, emitted light, rad spots finally gone, Build on entrance and subway floors, Expanded build areas and budget, wireless powered and more! 

##### [A sensible Prydwen overhaul](https://www.nexusmods.com/fallout4/mods/24198/) *v1.0*
 I hated the vanilla Prydwen, from not haveing a place to go to the bathroom, to the scattered stained beds that barely fits a unit, let alone an army. So I made this mod, a mod that attempts to fix the Prydwen. 

##### [Introducing – Radium-Inc](https://www.nexusmods.com/fallout4/mods/32175) *v1.4*
 A dungeon mod with small questline, this mod takes the player through the headquarters of Radium-Inc., a company which made radium-infused products. 

##### [The Lost Building of Atlantic](https://www.nexusmods.com/fallout4/mods/25401) *v2*
 As you're wandering through the ruins of downtown Boston, you find a building which is heavily fortified by a camp of raiders. You're not about to let a bunch of raiders get in the way of your curiosity, so you blast through them and enter the building. Inside, you can learn the story of Allison Miller, the CEO of Atlantic Pharmaceuticals, 

##### [Sanctuary Hills - Root Cellar Remade](https://www.nexusmods.com/fallout4/mods/24791) *v1.2*
 Sanctuary Hills Root Cellar turned in to abandoned fallout shelter. 

##### [Virgils LABORATORY - Evil Lab Overhaul](https://www.nexusmods.com/fallout4/mods/29540) *v1.00*
 Turns Virgil's cave into an evil science lab with unique supermutant home! 

##### [Aloot's Home Plate](https://www.nexusmods.com/fallout4/mods/15300/) *v2.2*
 Makes Home Plate into a sweet crash pad, adds it to the Supply Routes and allows Companions to be sent there. 

##### [Hotel Rexford](https://www.nexusmods.com/fallout4/mods/36458) *v1.1*
 This mod fixes most damage, removes dirt and most importantly matches the interior to look like the exterior of the building.
Also with more furniture added Rexford now really looks like a Hotel. 
> Install main file and optional NPCs outside of the street file

##### [Better Robotics Disposal](https://www.nexusmods.com/fallout4/mods/36077) *v1.0*
 Improves the Robotics Disposal Site by adding scrap robots 

## New quests and locations

##### [Fusion City Rising](https://www.nexusmods.com/fallout4/mods/16423/) *v1.0*
 DLC-sized quest mod. Sep. '16 File of the Month. Hours of new game play. New factions, new locations, and multiple fully voiced companions. 

##### [Outcasts and Remnants](https://www.nexusmods.com/fallout4/mods/21469/) *v1.40*
 DLC-sized quest mod. Apr '17 Mod of the Month runner-up. 20 hours of game play with new factions, locations, player bases, and fully-voiced custom companions. 

##### [Project Valkyrie](https://www.nexusmods.com/fallout4/mods/28085) *v1.20*
 Huge quest/companion adventure, August 2018 Mod of the Month. Four custom & fully-voiced companions, 20 quests, and alternate endings to the vanilla game. 

##### [Nuka-World Reborn](https://www.nexusmods.com/fallout4/mods/32857) *v1.30*
 Nuka-World Reborn is a quest mod which not only allows you to have multiple options to get rid of the raiders, but it adds new questlines to Nuka-World and allows you to play as a Trader. 

> Install main and optional file, then the AE patch here: https://www.nexusmods.com/fallout4/mods/34260

##### [50 Ways to Die at Dr. Nick's](https://www.nexusmods.com/fallout4/mods/25564/) *v0.99c*
 From the Co-Creator of Fusion City Rising and Outcasts & Remnants comes a Completely New Adventure...
10 Connected Quests, Unique Rewards, Custom Player Home, Lore-Friendly Backstory, Lots of Explosions, and a Twist. 

##### [The Secret of Huntress Manor - A Far Harbor Story](https://www.nexusmods.com/fallout4/mods/27311) *v1.6*
 Hidden within the woods of Huntress Island, enveloped by fog, stands Huntress Manor. Once the home of the reclusive but brilliant Professor R.S.G. Hunter, the manor has been abandoned since his sudden, unexplained, death in 1877; it is now known only to the wolves that call the forest their home. Little do they know, the manor holds a terrible secret. 

> Install 1.2 regular main file

##### [Vault 494 - A Vault-Tec Story](https://www.nexusmods.com/fallout4/mods/23651) *v1.3*
 Vault 494: A Vault-Tec Story adds a new Vault for the player to explore. As the player approaches the Nahant area they will pick up a Vault-Tec distress signal which will begin. From there the player will be free to explore Vault 494, which an accounting error gave an unusually high number, and Vault-Tec's attempts to create a crime-free society

##### [David Hunter - A Brotherhood Story](https://www.nexusmods.com/fallout4/mods/16808) *v2.2*
 David Hunter: A Brotherhood Story follows Scribe David Hunter as he fights to make the Commonwealth a better place but comes into conflict with Brotherhood traditionalists. 

##### [Hilda Hughes - An Institute Story](https://www.nexusmods.com/fallout4/mods/22128) *v1.4*
 Join Director of Robotics, Hilda Hughes, as she investigates the Prototype Synth Project. In doing this, the player will be able to enter the memories of five pre-war citizens and then discover their post-war fates. However, all is not well in the Robotics Division. A synth has gone missing and Hilda isn't convinced it was a production error. 

##### [Tales from the Commonwealth](http://3dnpc.com/) *v3.01*

>install Tales and Atomic Radio (optional) from 3Dnpc.com (always update before Nexus
version and contains custom tracks not on Nexus).

##### [Sector 5 – Rise and Fall](https://www.nexusmods.com/fallout4/mods/38457) *v1.3*
 Discover several new locations, including a new worldspace - all linked through a huge quest line, split in 5 parts. Meet a new companion, fight new factions, be rewarded with goodies, including new player homes. 

## Weather and environment

##### [Vivid Weathers](https://www.nexusmods.com/fallout4/mods/15466) *v2.011*
 This is a complete LORE FRIENDLY Weather and Climate Overhaul for Fallout 4!
It will add more than 75 new Weathers with over 110 new cloudtextures to the Fallout 4 World for you to experience.
It also improves the general Image quality by adding new LUT and Imagespaces to the game as well as a Player home and base to complete the Lore! 

> During install
> Alternative addons
> - Disable Volumetric Fogs
> - Extended Rain Sounds
> - Vivid Weathers Quest and Player Home
> Visual changes
> - Default - No changes
> Compatibility patches
> - Far Harbor Patch
> - Nuka World
> Seasons of Vivid Weathers
> - NO Season Limitation

##### [WET – Water Enhancement textures](https://www.nexusmods.com/fallout4/mods/20775) *v1.88*
 WET enhances all water and most water-related effects in the game. Simple. 

> During Installer select the WET Assets With Rain and the WET Clearer (ESL) options

##### [Darker nights](https://www.nexusmods.com/fallout4/mods/191) *v1.11p6*
 Now you see me... 

> Install both main and optional files, during installer, choose:
> - Light (level 4)
> - Far harbor and Nuka World DLC patches
> - Vivid weathers
> - Easiest (level 6)
> - Alternative (green tint)
> - Weaker night vision
> Leave the other options unticked

##### [Vault-Tec Workshop Overhaul](https://www.nexusmods.com/fallout4/mods/17174) *v3.1*
 A non intrusive mod that aims to fix inconsistencies within the Vault-Tec Workshop DLC. This version addresses three of the main lighting issues, and adds snapping to lighting wall fixtures. 
> Install main file only

##### [Clarity](https://www.nexusmods.com/fallout4/mods/31991) *v3.1*
 A zero performance loss weather and lighting overhaul. Removes many blurry effects for a cleaner, crisper image. Improves the look of the vanilla game without overdoing it or straying away from the original style. 

##### [Fr4nsson's Light Tweaks](https://www.nexusmods.com/fallout4/mods/2139) *v1.6*
 Tweaks the Fallout 4 lights. 

##### [Thaylar's Settlement Lighting Fixes](https://www.nexusmods.com/fallout4/mods/20003) *v3.1*
 Adjusts light output and radius values for settlement lights. Also fixes a few meshes to correct the light type to match the light source. 

>Install base edition main file

##### [Pip-Boy Flashlight](https://www.nexusmods.com/fallout4/mods/10840) *v5.02*
 Turn your radial Pip-Boy light into a directional flashlight! 

## Audio overhauls

##### [Bleak Beauty](https://www.nexusmods.com/fallout4/mods/9663) *v1.2*
 Bleak Beauty is a whole new OST for Fallout 4. The new tracks are specifically written for Fallout 4, and designed to fit its atmosphere. Now with non replacer version! 05/24 New tracks! 

##### [Radiant Birds](https://www.nexusmods.com/fallout4/mods/2397) *v0.5*
 Adds Real Sounds and Fixes for Birds 

> Install main file only

##### [Less Radiant Birds](https://www.nexusmods.com/fallout4/mods/16296) *v0.5c*
 Lowers the volume on Indipindi's excellent Radiant Birds mod (required.) 

> This is a replacer esp, merge with the original mod.

##### [Second World War British Air Raid Siren](https://www.nexusmods.com/fallout4/mods/12199) *v1.0*
 Replaces the default siren with a Second World War British Carter Gents air rad siren 

##### [Immersive Pickup Sounds F04 base](https://www.nexusmods.com/fallout4/mods/35917) *v1.00*
 This Mod adds in new FX sounds to most items in game. Theketzu kindly granted me access to use their files as well, meaning all of the sounds from FNV and F03 immersive pickup are back as well as some new sounds. 
 
##### [BiRaitBec ́s merged mods - Audio](https://www.nexusmods.com/fallout4/mods/23556) *v1.0*

> Download and install Merged Mods - Audio
> During the FOMOD installer
> - All-In-One
 
## Cut content restored

##### [Combat zone restored](https://www.nexusmods.com/fallout4/mods/21498) *v1.02*
 Restores the majority of the cut content from the Combat Zone. 

##### [Piper Interview Restored](https://www.nexusmods.com/fallout4/mods/21829) *v0.1*
 Restores part of the interview with Piper that was cut from the final game. 

##### [The Danse Dilemma](https://www.nexusmods.com/fallout4/mods/21923) *v2.9*
 Uses dialogue cut from the final game to provide more options to solve the issue of Danse's identity. 

## Late loaders

##### [No combat boundaries](https://www.nexusmods.com/fallout4/mods/6752) *v1.0*

 A small plugin to remove combat boundaries, so enemies will follow you indoors from outside and vice versa. 
 
> Note: These worldedits need to be removed from the esp in FO4Edit.
> ```
> ConcordZone
> ConcordMuseumZone
> StarlightDriveInZone
> RedRocketTruckStopZone
> SunshineTidingsCoopZone
> MysticPinesZone
> AbernathyFarm
> CountryCrossingZone
> GreentopNurseryZone
> NordHagenBeachZone
> OberlandStationZone
> TenPinesBluffZone
> SanctuaryHillsZone
> ```
> Thanks to sentrus, there is now a patch shipped with the guide doing the same thing, but I ́m leaving instructions in, for those who want to get their hands dirty with FO4Edit.

##### [More Attackers – Get off my Buildzone + Unique NPCs – C and M patch](https://www.nexusmods.com/fallout4/mods/27465) *v1.1.7*
 Moves attack markers beyond the boundaries of settlements. Adds additional attack markers around the perimeter of settlements. Solves the problem with spawning enemies inside a settlement after fast travel. Adds notifications to animals attacks. Increases time before attacks auto resolve (configurable). And more... 

> Install Unique NPCs – C and M patch name "More AGOMBZ + Unique NPCs – C and M
patch" so it doesn ́t merge with the main mod

##### [Better Companions](https://www.nexusmods.com/fallout4/mods/18547/)
Improves companion accuracy, sneaking, perks etc

##### [Amazing Follower Tweaks](https://www.nexusmods.com/fallout4/mods/26976)
Install main file and use original spouse patch, and XDI fix

##### [Comic Collector](https://www.nexusmods.com/fallout4/mods/18564)

##### [Load Screen Art](https://www.nexusmods.com/fallout4/mods/35361)
Install the mix random DLC main file. NOTE: some users have experienced noticably
longer game startup times (~30 seconds longer) with this mod activated.

##### [Immersive Drumlin Diner](https://www.nexusmods.com/fallout4/mods/18995/)

##### [Fallout 4 Revisited - Sanctuary - Safe Haven](https://www.nexusmods.com/fallout4/mods/26679)
If you install mod, do note that Sim Settlement city plans for Sanctuary likely won ́t work.

##### [AWARHERO's Great Green Jewel](https://danielgamache.wixsite.com/awarhero/diamond-city-the-great-green-jewel)
Install mod, them the replacer AWARHERO The Great Green Jewel.esp provided in my
files, which includes no world edits (only changes to Diamond city interiors).

##### [Diamond City Auto Close Gate](https://www.nexusmods.com/fallout4/mods/12928)
Using all the DC mods above will cause FPS drop in Diamond City. Of course they are all
optional, so you will have to chose if you like pretty or smooth. Biggest resource hog is
Diamond City Plus.

##### [Insignificant Object Remover](https://www.nexusmods.com/fallout4/mods/9835)

## Rounding up

##### [Universal Patch Installer](https://www.nexusmods.com/fallout4/mods/34825)
During installer, choose:
- Armorsmith extended
- Commonwealth shorts
- Commonwealth shorts – Vault Girl

##### [Ruse VIS-G and AE Patches](https://www.nexusmods.com/fallout4/mods/33480)
During installer, under equipment patches, choose:
- Crimsonrider ́s accessories
- Eli ́s armor compendium
- West Tek tactical optics

##### [Resh's GNARLY Unbogus Fallout Overhaul Patches - VIS-G - AE – UNPCs](https://www.nexusmods.com/fallout4/mods/35532?tab=files)
Install Unbogus VIS-G and AE patch only

##### [We Are The Minutemen - VIS-G - Armorsmith Extended Patch](https://www.nexusmods.com/fallout4/mods/18744?)
Comments on Nexus site regarding WATm 6: “there are several item that are
different. Like backpack world models and variant 6 flannel shirt is new item without
a tag.” 
> TODO: fix this
{.is-danger}


##### [CtGW Community patches](https://www.nexusmods.com/fallout4/mods/30294)
In CtGW main archive

## Dead last (conflict resolutions)

##### [Scrap dead things](https://www.nexusmods.com/fallout4/mods/6497)
Install Automatron version. After guide is done, move last in order

##### [Diamond City Expansion](https://www.nexusmods.com/fallout4/mods/21853)

##### [Diamond City Expansion - Female Body Replacer – EasyGirl](https://www.nexusmods.com/fallout4/mods/28740)
Install only the Diamond City Expansion - Female Body Replacer main file

##### [Boston Fps Fix](https://www.nexusmods.com/fallout4/mods/26286)
Note if you ́re going to install location mods not in this guide, that due to the nature of this
mod, a lot of location overhauls are not compatible, and will cause texture flickering/culling/
performance issues. Especially avoid mods that affect downtown Boston.
Install the AIO main file only

##### [The Beantown interiors Project](https://www.nexusmods.com/fallout4/mods/4612)

##### [BTI Optimization for BFPSFixAIO](https://www.nexusmods.com/fallout4/mods/26286)
A test compatibility patch with Boston FPS fix. Found under miscellaneous files

##### [CtGW - Conflict resolution](https://www.nexusmods.com/fallout4/mods/30294)
Now modular, install CtGW – CR.rar from the CtGW archive.

##### [CtGW - Gameplay Tweaks](https://www.nexusmods.com/fallout4/mods/30294)
Optional Now modular, install CtGW - Tweaks.rar from the CtGW archive.

##### [CtGW - Replacer ESPs](https://www.nexusmods.com/fallout4/mods/30294)
These are esps with my edits, which should override the original esps

##### [CtGW - Leveled Lists](https://www.nexusmods.com/fallout4/mods/30294)
My manually edited leveled lists. I recommend you use this one if you ́ve installed the
whole guide. If he esps complain about missing masters, there are mods in this list you
haven ́t installed and you would either have to remove those records
manually or use
Wrye Bash instead.

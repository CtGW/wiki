---
title: Prerequisites
description: things to do before we start adding mods
published: 1
date: 2019-07-23T19:30:00.341Z
tags: 
---

# Prerequisites

## A word about testing your mod list

Why a section like this before you´ve even installed any mods? Because once you´ve installed them all it won´t really do much good. If you run into issues in game, after having installed 200+ mods without even starting the game once to actually test it, it will take you a lot longer time, and cause you a lot more frustration to locate the error than if you had tested properly from the beginning.

A typical testrun for me would be vanilla start, exit the vault, find and talk to Codsworth in Sanctuary, kill the bugs, activate the workbench, run to Red Rocket, greet Dogmeat, activate the workbench, run down to concorde, save the minutemen, get the Power armor, and return to Sanctuary via fast travel, exit the Power armor. Takes about 20 mins once you get the hang of it.

Every 5th testrun or so I will fast travel back to the Library and then run all the way to Diamond City, talk to Piper and go to Nick´s office, for more extensive testing. Especially looking for texture and culling issues in downtown Boston.

Note about vanilla test saves before exiting vault. I used to load these all the time for a faster start up, thought everything was working fine, only to have weird things happening in the prologue with a new game. It seems mods related to player characteristics are only effective with a new game. Use them, but try a new start every now and then, to make sure nothing´s gone haywire :P

If you add a mod overhauling a specific location, you can use console commands to reveal their map markers and enable fast travel to these locations.

The key for console on your keyboard might vary from mine, due to different language keyboards.
You can find the key for your keyboard [here](http://fallout.wikia.com/wiki/Fallout_4_console_commands).

`tmm 1` – Enables all locations as discovered to your Pip-Boy with fast travel. Of course, some of these locations will get you killed if you go there too early, and because of this I use custom save games for that purpose:
- [Ain't nobody got time for that - Fallout 4 Template Save Games](https://www.nexusmods.com/fallout4/mods/26328)
- [Level 50 at Vault 111](https://www.nexusmods.com/fallout4/mods/285)

Other mods to help me with mod testing:
- [Cheat Terminal](https://www.nexusmods.com/fallout4/mods/13285/)
- [Display Location - Cell - Object Information](https://www.nexusmods.com/fallout4/mods/14145)
- [In-GameESPExplorer](https://www.nexusmods.com/fallout4/mods/16718)

If you add a mod overhauling a specific NPC, you can use console commands to spawn that NPC at your location. You will need the `base.id` for the NPC in question. 
E.g. to spawn a settler:
```
player.placeatme 20593
```

[The Fallout Wiki](http://fallout.wikia.com/wiki/Portal:Fallout_4) is an excellent resource for finding base and ref ids. 

`player.placeatme ref.id`  will literally teleport the NPC to your location
`player.placeatme base.id` will spawn a clone of the NPC to your location

Here are some useful id's to:

|          | `base.id`|`ref.id`|
|----------|:--------:|-------:|
|Cait      | 00079249 |00079305|
|Codsworth | 0001ca7d |0001ca7d|
|Curie     | 00027686 |00102249|
|Danse     | 00027683 |0005de4d|
|Deacon    | 00045ac9 |00050976|
|Dogmeat   | 0001d15c |0001d162|
|Hancock   | 00022613 |00022615|
|MacCready | 0002740e |0000313b|
|Valentine | 00002f24 |00002f25|
|Piper     | 00002f1e |00002f1f|
|Garvey    | 00019fd9 |0001a4d7|
|Strong    | 00027682 |0003f2bb|
|X6-88     | 000bbee6 |000e210a|
|Ada       | xx00fd5a |xx00ff12|
|Longfellow| xx006e5b |xx014602|
|Gage      | xx00881d |xx00a5b1|

With all that boring presentation out of the way, let´s get started!

## Tools
Some of the tools in this section need to be installed into the Fallout 4 base directory in order to work properly. I make it a habit to install all of them there, **the one exception being MO2**, which I install on another drive.

One of the best places to read about Bethesda tools is on [DarkLadyLexy's LOTD - SSE guide](https://wiki.step-project.com/User:DarkladyLexy/Lexys_LOTD_SE_Prerequisites).
This guide is one huge monolithic creature and a beast, but also the best guide available for Skyrim Special Edition. It is totally worth it to install that guide and there are regular upgrades which keep it up to date.

Here I am listing the tools that we need from that page:

### [FO4Edit](https://github.com/TES5Edit/TES5Edit/releases/)
This powerful utility allows you to modify, clean, and patch your plugins. [GamerPoets](https://www.youtube.com/watch?v=2F19Do8HAl4) has a
good primer how to use FO4Edit on YouTube.

### [Wrye Bash]()

### [F4SE](http://f4se.silverlock.org/)

### [Mod Organizer 2]()

### [FO4 configuration tool]()

### [BethINI]()

### [xSE plugin preloader]()

### [Dynamic performance tuner and load accelerator]()

## Cleaning master files
In the last section we learned how to open a tool from MO2 with a command line flag which allowed us to easily determine which esps can be flagged a esl. That means I don´t have to show you the Modify executables window again, right? Right.

We´re going to create a third instance of FO4Edit, this time to help us automate the master cleaning process. You know how to do this, create another instance similar to the PseudoESL one but instead use -quickautoclean as the flag. Name it FO4Edit (-quickautoclean). Save it, and run FO4Edit (-quickautoclean)

You can only open FO4Edit this way with one plugin at a time, so start with whichever esm you have first in the list, and work yourself through all of them.
- Start FO4Edit (-quickautoclean)
- doubleclick on ESM to clean
- wait until background loader is finished
- close FO4Edit
- repeat from step one with next ESM
FO4Edit is smart and will save a backup of said ESM files in it´s overwrite folder. Good to know!

## Texture overhaul (from BiRaitBec)

## Choosing ESLs

**TLDR**: When given a choice of choosing an ESP or an ESL you should always download the ESP and then manually mark it as an ESL in FO4Edit.

For an in-depth understanding: https://www.afkmods.com/index.php?/topic/5079-plugin-files-and-you-esmeslesp/

We outline a small summary:

### How ESLs work

Firstly, lets remember that the Bethesda engine allows loading 255 plugins in total.
Each plugin occupies a namespace, `xx`, for its load order, where a general element is represented by: `xx123456`

So, in theory, any plugin can add <code>16<sup>6</sup></code> new items.

ESLs work by sharing the `FE` namespace, so that an element in the plugin looks like `FEyyyyyy`.
The first ESL has the plugin FormIDs as: `FE00zzzz`, the second ESL has FormIDs as: `FE01zzzz`

So in theory, you cannot have more than 256 ESL plugins in your modlist.

### ESL vs ESP
If you use an ESP marked as an ESL in FO4Edit, the plugin respects your load order, while if you use an ESL, the bethesda engine loads it in the ESM space.
ESL plugins are loaded
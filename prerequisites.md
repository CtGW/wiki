---
title: Prerequisites
description: things to do before we start adding mods
published: 1
date: 2019-07-15T13:20:11.963Z
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

`tmm 1` – Enables all locations as discovered to your Pip-Boy with fast travel. Of course some of these locations will get you killed if you go there too early, and because of this I use custom save games for that purpose:
- Ain't nobody got time for that - Fallout 4 Template Save Games: https://www.nexusmods.com/fallout4/mods/26328
- Level 50 at Vault 111: https://www.nexusmods.com/fallout4/mods/285

## Tools

### FO4Edit

### Wrye Bash

### F4SE

### Mod Organizer 2

### FO4 configuration tool

### BethINI

### xSE plugin preloader

### Dynamic performance tuner and load accelerator

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

## ESP vs ESL
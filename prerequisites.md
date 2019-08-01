---
title: Prerequisites
description: things to do before we start adding mods
published: 1
date: 2019-08-01T14:43:12.581Z
tags: 
---

# Prerequisites

## A word about testing your mod list

> You don't need to install anything in this section, these mods will be installed in the course of the guide.
> This section is just an information dump to help in understanding the guide and Fallout 4 modding in general.
>{.is-danger}

**Why a section like this before you've even installed any mods?** 
Because once you've installed them all it won't really do much good. 
If you run into issues in game, after having installed 200+ mods without even starting the game once to actually test it, it will take you a lot longer and cause you a lot more frustration to locate the error than if you had tested properly from the beginning.

A typical testrun for me would be 
> **Short run**
> - Vanilla start
> - Exit the vault
> - Find and talk to Codsworth in Sanctuary
> - Kill the bugs
> - Activate the workbench in Sanctuary
> - Run to Red Rocket, greet Dogmeat
> - Activate the workbench in Red Rocket
> - Run down to Concord
> - Save the minutemen and get the Power armor
> - Return to Sanctuary via fast travel and exit the Power armor

Takes about 20 minutes once you get the hang of it.

>The guide will have checkpoints which will tell you to do a **short run**.
>{.is-success}

Every 5^th^ testrun or so you can do a deeper test by also adding the following steps

> **Long run** 
> - Do the **short run**
> - Run to the Boston Public Library 
> - Run to Diamond City
> - Talk to Piper and enter the city
> - Go to Nick's office and talk to him
> - Exit Diamon City and roam around the outskirts of Diamon City and South Boston (look for texture and culling issues)

<hr style="border-top: dotted 1px; color: pink; background-color: transparent;" width="50%" />

#### Console

The key for console on your keyboard might vary from mine, due to different language keyboards, but in general the key for the console is the `` ` `` key, which is besides `1`.

You can find a list of console commands and utilities [here](http://fallout.wikia.com/wiki/Fallout_4_console_commands).

If you add a mod overhauling a specific location, you can use console commands to reveal their map markers and enable fast travel to these locations.
`tmm 1` - Enables all locations as discovered to your Pip-Boy with fast travel.
Of course, some of these locations will get you killed if you go there too early and because of this you can also enable God Mode by the command `tgm` (*toggle god mode*).

You can also use custom save games if you just want to visit an overhauled location:
- [Ain't nobody got time for that - Fallout 4 Template Save Games](https://www.nexusmods.com/fallout4/mods/26328)
- [Level 50 at Vault 111](https://www.nexusmods.com/fallout4/mods/285)
> Note about vanilla test saves before exiting vault. I used to load these all the time for a faster start up, thought everything was working fine, only to have weird things happening in the prologue with a new game. It seems mods related to player characteristics are only effective with a new game. Use them, but try a new start every now and then, to make sure nothing´s gone haywire :P
> {.is-warning}

Some other mods that help with testing:
- [Cheat Terminal](https://www.nexusmods.com/fallout4/mods/13285/)
- [Display Location - Cell - Object Information](https://www.nexusmods.com/fallout4/mods/14145)
- [In-GameESPExplorer](https://www.nexusmods.com/fallout4/mods/16718)

<hr style="border-top: dotted 1px; color: pink; background-color: transparent;" width="50%" />

#### NPC
If you add a mod overhauling a specific NPC, you can use console commands to spawn that NPC at your location. You will need the `base.id` for the NPC in question. 
E.g. to spawn a settler:
```
player.placeatme 20593
```

[The Fallout Wiki](http://fallout.wikia.com/wiki/Portal:Fallout_4) is an excellent resource for finding base and ref ids. 

`player.placeatme ref.id`  will literally teleport the NPC to your location
`player.placeatme base.id` will spawn a clone of the NPC to your location

Here are some useful id's:

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

With all that boring presentation out of the way, let's get started!

## Fallout 4 Base

> DO NOT install Fallout 4 in any UAC (User Account Control) controlled folder structure. This includes x:/Program Files, x:/Program Files(x86), and the main Windows directory. It is, instead, advised to install the game (and, really, Steam itself) ANYWHERE other than there. Idealy, it would be on a separate SSD drive from your Operating System, but if that's not feasible, at least ensure that UAC is either turned off completely (not recommended for basic users) or installed outside of it's control. This also applies to ANY tools or programs other than the base game, with the important note that they SHOULD NOT (despite what some old tutorials may say) be installed into the Fallout 4 base folder unless specifically directed to do so.
>{.is-danger}

For this guide you need the latest versions of
- **Fallout 4** *v 1.10.138*
- **Creation Kit** *v 1.10.130*

### Steam Overlay

We recommend keeping the steam overlay disabled.
You can disable it for Fallout 4 as follows:
```
Open the Steam Library. 
Right click Fallout 4 in the games list and select Properties. 
In the Properties window UNCHECK Enable the Steam Overlay while in-game.
```

## Tools

> Some of the tools in this section need to be installed into the Fallout 4 base directory in order to work properly.
> It's a good idea to make it a habit to install all of them there, **the one exception being MO2**, which you can install on another drive.

One of the best places to read about Bethesda tools is on [DarkLadyLexy's LOTD - SSE guide](https://wiki.step-project.com/User:DarkladyLexy/Lexys_LOTD_SE_Prerequisites).
This guide is one huge monolithic creature and a beast, but also the best guide available for Skyrim Special Edition. It is totally worth it to install that guide and there are regular upgrades which keep it up to date.

Here we list the tools that we need:

##### [7-zip](https://www.7-zip.org/) (version unimportant)
The most versatile compression utility for compression/decompression

> A lot of mods and archives are going to be `.7z` compressed which necesitates the use of this program.
>{.is-success}


##### [F4SE](http://f4se.silverlock.org/) *v0.6.17*
**Fallout 4 folder**
Copy only the following files to the main Fallout4 root:
- f4se_1_10_138.dll
- f4se_loader.exe
- f4se_steam_loader.dll

> We are not installing the scripts here, as we will be installing them through MO2, which keeps our Data folder clean.
>{.is-success}

##### [FO4Edit](https://github.com/TES5Edit/TES5Edit/releases/) *v4.0.2*
**Fallout 4 folder**
This powerful utility allows you to modify, clean, and patch your plugins. [GamerPoets](https://www.youtube.com/watch?v=2F19Do8HAl4) has a good primer how to use FO4Edit on YouTube.

##### [Wrye Bash](https://www.dropbox.com/sh/iazpayeexiyazeh/AAAbGeVHrlIksp2AFgI4w48Oa?dl=0)
**Falout 4 folder**
Download whatever the current nightly version is available on the Dropbox folder and then extract the folder `Mopy` to the Fallout 4 root folder.
Your Fallout 4 directory should contain a folder called `Mopy`

>WINDOWS 7 USERS: A 'docs' folder needs to be created in ...\Fallout 4\Data. WIN10 users do not need to follow this step, as it will be auto-created and placed into your Overwrite folder. For additional info, see Notice below.
>WINDOWS 10 USERS: Ensure that your O/S has installed the Windows 10 1809 Update or higher. This will ensure that Wrye Bash is able to properly load, as the 1803 update creates a situation where WB attempts to load itself, which it can't because it's already in use.
>WINDOWS 10 USERS: When using Wrye Bash, a 'Docs' folder will be generated and appear in your Overwrite folder. This is not needed for Skyrim to run properly, and can be safely deleted between sessions.
>{.is-danger}


##### [Mod Organizer 2](https://github.com/ModOrganizer2/modorganizer/releases)

##### [FO4 configuration tool](https://www.nexusmods.com/fallout4/mods/102/)

##### [BethINI](https://www.nexusmods.com/fallout4/mods/67)

##### [xSE plugin preloader](https://www.nexusmods.com/fallout4/mods/33946)

##### [Dynamic performance tuner and load accelerator](https://www.nexusmods.com/fallout4/mods/28143)

Also download: [Configuration Files For Dynamic Performance Tuner And Load Accelerator](https://www.nexusmods.com/fallout4/mods/33632)

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


---
Credits: 
- DarkLadyLexy, for her amazing pre-requisites page from her guide
- Biraitbec, for his amazing modlist and recommendations for FO4
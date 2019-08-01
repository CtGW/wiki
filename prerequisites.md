---
title: Prerequisites
description: things to do before we start adding mods
published: 1
date: 2019-08-01T18:05:20.336Z
tags: 
---

# Prerequisites

One of the best places to read about Bethesda tools is on [DarkLadyLexy's LOTD - SSE guide](https://wiki.nexusmods.com/index.php/User:Darkladylexy/Lexys_LOTD_SE).
This guide is one huge monolithic creature and a beast but also the best guide available for Skyrim Special Edition. 
It is totally worth it to install that guide and there are regular upgrades which keep it up to date.

We are using a lot of the information from her [prerequisites page](https://wiki.nexusmods.com/index.php/User:Darkladylexy/Lexys_LOTD_SE), which is applicable to all bethesda modding in general.

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
> It's a good idea to make it a habit to install all of them there, unless specified under the mod name, e.g. **ModOrganizer2**, which you can install on another place.
> {.is-success}


##### [7-zip](https://www.7-zip.org/) (version unimportant)
**(install as a standard program)**
The most versatile archive utility for compression/decompression

> A lot of mods and archives are going to be `.7z/rar/zip` compressed which necessitates the use of this program.
>{.is-success}


##### [F4SE](http://f4se.silverlock.org/) *v0.6.17*
**Fallout 4 folder**
Copy only the following files to the main Fallout4 root:
- f4se_1_10_138.dll
- f4se_loader.exe
- f4se_steam_loader.dll

> We are not installing the scripts here, as we will be installing them through MO2, which keeps our Data folder clean.
>{.is-success}

##### [xSE plugin preloader](https://www.nexusmods.com/fallout4/mods/33946) *v0.1.2*
**Fallout 4 folder**
This mod allows preload F4SE plugins before the game initializes. 
 
>Download the main file and extract the contents (*xSE PluginPreloader.ini, IpHlpAPI.dll*) to the Fallout4 main directory.

##### [Dynamic performance tuner and load accelerator](https://www.nexusmods.com/fallout4/mods/28143) *v0.9.5*
**Fallout 4 folder**
Dynamically adjusts Shadow Dir Distance and Godray Quality. 

> Download the main file and extract only the files *dxgi.dll, dynaperf.ini* to the Fallout4 main directory.

#### [Configuration Files For Dynamic Performance Tuner And Load Accelerator](https://www.nexusmods.com/fallout4/mods/33632) *v1.10.130.1*
**Fallout 4 folder**
The latest offsets / INI file (and an explanation of how to make your own "ini" files) for StochasticTinker's "Dynamic Performance Tuner And Load Accelerator" mod. These offsets are needed every time fallout4.exe is updated. I'll do this for you when I can, but this also shows YOU how to do it. 

> Download the main file and add the two files *fallout4-addresses-&ast;.&ast;.&ast;.&ast;.ini, Fallout4.CT* to the Fallout4 main directory.

##### [FO4 configuration tool](https://www.nexusmods.com/fallout4/mods/102/)
**Fallout 4 folder**

- After installation, run the program as adminstrator (right-click and choose "Run as administrator")
- Click `no` on the window that pops up.
- Change the following settings
> **Tweaks tab**
> Select *Invalidate Archives* and *Fix Sensitivity Ratio*, then select the *Auto Execute* option and click on add.
> In the opened window just copy these lines:
>```
> gr quality 3
> gr grid 8
> gr scale .4
> gr maxcascade 2
> cl rim 0.0005
> setgs iTerminalDisplayRate 1200
> setgs fWorkshopWireMaxLength 2200
> setgs fGunShellLifetime 150
> setgs fGunShellCameraDistance 12800
> setgs iDebrisMaxCount 375
> setgs iHoursToRespawnCell 720
> setgs iHoursToRespawnCellCleared 2160
> setgs iRemoveExcessDeadComplexCount 50
> setgs iRemoveExcessDeadCount 50
> setgs iRemoveExcessDeadComplexTotalActorCount 65
> setgs iRemoveExcessDeadTotalActorCount 50
> setgs fDiffMultHPToPCVH 1.75
> setgs fDiffMultHPByPCVH 0.75
> tMtrdfl ON
> tMtr ppld
> thighprocess on
> SA	M 1
>```
> **Performance Tab**
> Select high Priority and unselect RadialBlur
>```
>Vsync=0 
>inumHWThreads = your number of CPU cores
>```
> We´re forcing it in driver instead

> Explanation for these lines:
>```
> gr quality
> gr grid
> gr scale
> gr maxcascade
>```
> These lines make godrays more good looking and performance friendly.
>```
> cl rim
>```
> This line will fix the character light to be more realistic.
>```
> setgs iTerminalDisplayRate
>```
> This line will make the terminals load the screen faster.
>```
> setgs fWorkshopWireMaxLength
>```
> This line will make power lines longer.
>```
> setgs iHoursToRespawnCell
> setgs iHoursToRespawnCellCleared
>```
> These lines increase the length of area and corpses respawn time.
>```
> setgs fGunShellLifetime
> setgs fGunShellCameraDistance
> setgs iDebrisMaxCount
>```
> These lines will leave shot bullets visible for a longer time.
> These additions make many plugins redundant, without adding to the plugin count.
> You´ll need to save before exiting the window.


##### [BethINI](https://www.nexusmods.com/fallout4/mods/67)

##### [Wrye Bash](https://www.dropbox.com/sh/iazpayeexiyazeh/AAAbGeVHrlIksp2AFgI4w48Oa?dl=0) *(nightly)*
**Falout 4 folder**

> Download whatever the current nightly version (standalone executable) is available on the Dropbox folder and then extract the folder `Mopy` to the Fallout 4 root folder.

- Your Fallout 4 directory should contain a folder called `Mopy`

>WINDOWS 7 USERS: A 'docs' folder needs to be created in ...\Fallout 4\Data. WIN10 users do not need to follow this step, as it will be auto-created and placed into your Overwrite folder. For additional info, see Notice below.
>WINDOWS 10 USERS: Ensure that your O/S has installed the Windows 10 1809 Update or higher. This will ensure that Wrye Bash is able to properly load, as the 1803 update creates a situation where WB attempts to load itself, which it can't because it's already in use.
>WINDOWS 10 USERS: When using Wrye Bash, a 'Docs' folder will be generated and appear in your Overwrite folder. This is not needed for Skyrim to run properly, and can be safely deleted between sessions.
>{.is-danger}


##### [FO4Edit](https://github.com/TES5Edit/TES5Edit/releases/) *v4.0.2*
**Fallout 4 folder**
This powerful utility allows you to modify, clean, and patch your plugins.
[GamerPoets](https://www.youtube.com/watch?v=2F19Do8HAl4) has a good primer how to use FO4Edit on YouTube.

> FO4Edit and xEdit (and any others like FNVEdit, SSEEdit) are interchangeable and the only difference is renaming the file `xEdit.exe` to the corresponding game name.
>{.is-success}

> FO4Edit will create a cache folder, which will be made into a separate mod.
> We will redirect the output of FO4Edit in MO2 to the mod folder, this is a part of setting up MO2.
>{.is-success}

##### [Mod Organizer 2](https://github.com/ModOrganizer2/modorganizer/releases)


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
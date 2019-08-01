---
title: Testing
description: keep testing while installing, so you can find mess-ups early on
published: 1
date: 2019-08-01T15:01:36.254Z
tags: 
---

# A word about testing your mod list

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


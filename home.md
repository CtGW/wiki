---
title: Crossing the Great Wastes
description: The most comprehensive modlist for FO4 by Ape, et al.
published: 1
date: 2019-07-15T13:14:55.731Z
tags: 
---

# Welcome
Originally a companion to the amazing guide found [here](https://www.nexusmods.com/fallout4/mods/23556/), by the venerable BiRaitBec, I no longer recommend installing my modlist on top of his. Our lists, although still having many elements in common, and still using many of his textures and ini settings, have diverged so much that it would just be a hassle. This modlist is now meant to be installed from scratch. I still recommend having tried his modlist first though, especially if you´re new to modding, as it´s a lot more straightforward for beginners, whereas CtGW requires more of the modder. Mod Organiser is (in my opinion) a much more flexible and versatile mod organiser. Highlights follow below:
- You never need to actually touch the game data directory, since MO2 creates a virtual data directory on the fly when launching the game, effectively overriding the vanilla files, without overwriting. Basically, if you for some reason mess up your mod loadout there is never any need to reinstall your game, just create a new profile in MO2.
- MO2 allows you more control over mod and plugin order, and to reorder both at any time, without any mod ever being overwritten. In NMM it is crucial to pay attention when your installing mods, as if you´re installing a mod that touches the same resources as an earlier installed mod, you will be asked if you want to overwrite, and you need to know if that´s a good idea. If you make a mistake, you could of course just re-install the earlier mod and override back, but that can be very cumbersome, especially if you don´t remember which mod was overwritten. In MO2, it´s as easy as rearranging the mod order in the left pane.

That said, NMM  (or Vortex I suppose, although I haven´t felt the need to try it yet) surely has a a lower learning curve, and if you´re just a casual gamer, it will serve you just fine, especially when you have BiRaitBecs amazing guide to hold your hand :)

My modest (no, really) rig when following this guide:
```
Intel Core i5 7400 3ghz
(Nvidia) ASUS Dual GeForce GTX 1060 OC 6gb
16gb Crucial DDR4 2133 RAM
275gb Crucial SSD m.2 mx300
4tb WD Blue HDD
```

Note that I don´t know what my current FPS range is, for one simple reason – I don´t want to focus too much on if I lose 2 or 3 fps somewhere. I go by general feeling. Most of the game flows really well with my setup and this list, only notable exception right now being Diamond City, where FPS loss is definitely noticable, but not so much as to make it unplayable. Of course that section of this modlist is completely optional.

It would be ideal to install everything on the SSD, but for space reasons Im going to be installing the main game on the SSD and the mods on the HDD. That way I get at least some benefit from the faster SSD. If you have enough space to install everything on the SSD, by all means do so. If you´re using an HDD only and experience severe loading times, remove mods with a lot of loose files, ie not packed in BA2. There is a reason the first section of Biraitbec´s guide goes through how to patch the basegame´s packed files with various texture overhauls, instead of using their loose files..

## A word about testing your mod list

Why a section like this before you´ve even installed any mods? Because once you´ve installed them all it won´t really do much good. If you run into issues in game, after having installed 200+ mods without even starting the game once to actually test it, it will take you a lot longer time, and cause you a lot more frustration to locate the error than if you had tested properly from the beginning.

A typical testrun for me would be vanilla start, exit the vault, find and talk to Codsworth in Sanctuary, kill the bugs, activate the workbench, run to Red Rocket, greet Dogmeat, activate the workbench, run down to concorde, save the minutemen, get the Power armor, and return to Sanctuary via fast travel, exit the Power armor. Takes about 20 mins once you get the hang of it.

Every 5th testrun or so I will fast travel back to the Library and then run all the way to Diamond City, talk to Piper and go to Nick´s office, for more extensive testing. Especially looking for texture and culling issues in downtown Boston.

Note about vanilla test saves before exiting vault. I used to load these all the time for a faster start up, thought everything was working fine, only to have weird things happening in the prologue with a new game. It seems mods related to player characteristics are only effective with a new game. Use them, but try a new start every now and then, to make sure nothing´s gone haywire :P

If you add a mod overhauling a specific location, you can use console commands to reveal their map markers and enable fast travel to these locations.

The key for console on your keyboard might vary from mine, due to different language keyboards. You can find the key for your keyboard [here](http://fallout.wikia.com/wiki/Fallout_4_console_commands).
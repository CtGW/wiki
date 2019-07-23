---
title: Main modding
description: The brunt of the modding, where we focus on adding mods
published: 1
date: 2019-07-23T19:45:20.251Z
tags: 
---

# Main modding
## Choosing ESL or not

**TLDR**: When given a choice of choosing an ESP or an ESL you should always download the ESP and then manually mark it as an ESL in FO4Edit.

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

## Minor fixes

## Misc tweaks

## Camera and UI

## Settlements

## Cosmetic overhauls

## Clothing

## Armor

## Power armor

## Weapons of lore

## Gameplay

## NPC and creature overhauls

## Companion overhauls

## New companions

## Animations

## Vanilla location overhauls

## New quests and locations

## Weather and environment

## Audio overhauls

## Cut content restored

## Late loaders

## Rounding up

## Dead last (conflict resolutions)
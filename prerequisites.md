---
title: Prerequisites
description: things to do before we start adding mods
published: 1
date: 2019-07-14T19:28:07.450Z
tags: 
---

# Prerequisites

Coming soon...

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
In the last section we learned how to open a tool from MO2 with a command line flag which
allowed us to easily determine which esps can be flagged a esl. That means I don´t have to show
you the Modify executables window again, right? Right.
We´re going to create a third instance of FO4Edit, this time to help us automate the master cleaning
process. You know how to do this, create another instance similar to the PseudoESL one but instead
use -quickautoclean as the flag. Name it FO4Edit (-quickautoclean). Save it, and run FO4Edit (-
quickautoclean)
You can only open FO4Edit this way with one plugin at a time, so start with whichever esm you
have first in the list, and work yourself through all of them.
- Start FO4Edit (-quickautoclean)
- doubleclick on ESM to clean
- wait until background loader is finished
- close FO4Edit
- repeat from step one with next ESM
FO4Edit is smart and will save a backup of said ESM files in it´s overwrite folder. Good to know!

## Texture overhaul (from BiRaitBec)

## ESP vs ESL
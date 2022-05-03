---
permalink: /addons/equipviewer/
title: Equipviewer
tags:
  - User Interface
---

!!! info inline end "Attribution"

    **Author:**  Tako, Rubenator<br>
    **Version:**  3.3.0<br>
    **Date:** April 13, 2021<br>

Displays current equipment grid on screen. Also can show current Ammo count and current Encumbrance.

## Settings

Most settings can be modified via commands, but you can edit the `settings.xml` directly for a few uncommon settings.

## Commands

!!! tip ""

    **Abbreviation:** `ev`

#### position
:   `position <xpos> <ypos>`
    Moves the display to the specified position (from top left).

#### size
:    `size <pixels>`: set pixel size of each item slot (defaults to 32 -- same as the size of the item icons)

#### scale
:   `scale <factor>`: scale multiplier for size of each item slot (1 is 32px) -- modifies same setting as size

#### alpha
:   `alpha <opacity>`: set opacity of icons (out of 255)

#### transparency
:   `transparency <transparency>`: inverse of alpha (out of 255) -- modifies same setting as alpha

#### background
:   `background <red> <green> <blue> <alpha>`: sets color and opacity of background (out of 255)

#### ammocount
:   `ammocount`: toggles showing current ammo count (defaults to on/true)

#### encumbrance
:   `encumbrance`: toggles showing encumbrance Xs (defaultis on/true)

#### hideonzone
:   `hideonzone`: toggles hiding while crossing zone lines (default is on/true)

#### hideoncutscene
:   `hideoncutscene`: toggles hiding when in cutscene/npc menu/etc (default is on/true)

#### justify
:   `justify`: toggles between ammo text being right or left justifed (default is right justified)

#### help
:   `help`: displays explanations of each command

### Example Commands

=== "Windower Console"

    ```
    ev pos 700 400
    ev size 64
    ev scale 1.5
    ev alpha 255
    ev transparency 200
    ev background 0 0 0 72
    ev ammocount
    ev encumbrance
    ev hideonzone
    ev hideoncutscene
    ev justify
    ev help
    ```

=== "Chat Input"

    ```
    //ev pos 700 400
    //ev size 64
    //ev scale 1.5
    //ev alpha 255
    //ev transparency 200
    //ev background 0 0 0 72
    //ev ammocount
    //ev encumbrance
    //ev hideonzone
    //ev hideoncutscene
    //ev justify
    //ev help
    ```

=== "Game Macro"

    ```
    /con ev pos 700 400
    /con ev size 64
    /con ev scale 1.5
    /con ev alpha 255
    /con ev transparency 200
    /con ev background 0 0 0 72
    /con ev ammocount
    /con ev encumbrance
    /con ev hideonzone
    /con ev hideoncutscene
    /con ev justify
    /con ev help
    ```
    
## Legacy Commands

#### game_path
:   `game_path <path>`: sets path to FFXI folder where you want dats extracted from. Backslashes `\` must be escaped (like so: `\\`) or use forward slash `/` instead. (Legacy command as of `3.3.1` in which the game path is now pulled from the registry, but this command is still here in case you want to pull from dats that exist elsewhere.)

## Source
The latest source and information for this addon can be found on [GitHub](https://github.com/Windower/Lua/tree/live/addons/equipviewer).

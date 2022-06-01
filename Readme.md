<<<<<<< HEAD
# IC_Briv_Farm_for_TR
=======
# IC Script Hub
## ``New:``
Script Hub has been updated for use with and with antilectual's [ScriptHub-AutomaticOffsets](https://github.com/antilectual/ScriptHub-AutomaticOffsets). See the the linked repo for instructions on how to use it to update Script Hub's offsets.
<<<<<<< Updated upstream

## Introduction

> "This is your last chance. After this, there is no turning back. You take the blue pill—the story ends, you wake up in your bed and believe whatever you want to believe. You take the red pill—you stay in Wonderland, and I show you how deep the rabbit hole goes. Remember: all I'm offering is the truth. Nothing more." 
>  
> --- Morpheus 


> "I feel the need, the need for speed!"
> 
> --- Maverick

Welcome to 2022 and Happy New Year!  

New year, new script. We hope you like it.   
  
This script is the successor to ModronGUI.
=======
>>>>>>> Stashed changes

## Introduction
>>>>>>> e960edc0faf3c47c8c0cc6a873a6a2c63259d168

ver 0.5

TRMod for IC Script Hub by Thatman</br>
Modified gem farm for temporal rift (not tested on other variants)</br>

This addon detects when you run out of haste stacks and does stacking and restarts the adventure at that point.</br>
Early stacking is supported</br>
Some failsafe resets are removed</br>

---
 </br>
 </br>
Installation: Copy IC_BrivGemFarm_TR directory to your Briv Gem Farm\AddOns directory (should look like \AddOns\IC_BrivGemFarm_TR\) and enable the addon with IC Script Hub's addon manager or any other way you like.</br>
At first run it writes one line to IC_BrivGemFarm_Settings.ahk:</br>
 #include *i %A_LineFile%\..\..\IC_BrivGemFarm_TR\IC_BrivGemFarm_TR_enable.ahk</br>
If you remove this mod, you may want to remove that line also. You don't have to.</br>
 </br>
Note: When updating IC Briv Gem Farm with Github Desktop, the AddOns folder will be reverted to original, ie. this mod will be deleted.</br>
</br>
</br>
</br>
Usage:</br>
</br>
"Use dynamic reset zone?" Enables this mod. Disable to have 100% original unmodded functionality of Briv Gem Farm.</br>
"Reset after stacking if haste stacks is less than this" for early stacking. Ignored if dynamic reset zone is unchecked.</br>
Many times when changing adventures and come back, I got 70 stacks left, then stack/restart, then use the few remaining stacks and then restart the adventure. If you don't like it, set it to 0.</br>
In-game Modron core reset level is ignored when playing any variant, including Temporal Rift (that's kinda why I made this thing).</br>
But you need to set it to high-ish level for dash wait to work. Reset enabled or not.</br>
</br>
Force reset after specified zone: If your click wall is lower than the zone Briv can reach, or if you start gem farm at high level and high number of stacks, (or any other reason), you can set the reset level yourself. If you run out of stacks before this level, the adventure will restart. Recommended to set this just a bit under your click wall to be safe.</br>
</br>
Previous resets are stored in trlog.json file.</br>
</br>
Avoid bosses/barriers checkbox and Jump only from this zone mod5: When enabled, the party will walk with e formation to desired jump zone and jump with q formation from there.</br>
For example with 3 jump Briv, set it to 2. You'll walk to zone 2, 7, 12, 17 etc and jump to zone 1, 6, 11, 16 etc. Repeat until end. You'll avoid all the bosses and the barriers at zones 3 and 48.</br>
</br>
Walk this many levels to stacking zone: With this, you'll walk in e formation to "stack after this zone" (+1 zone, because it's AFTER) and you can use potions after early stacking. Set to 0 to disable.

---

<<<<<<< HEAD
v0.44 added Start TR button. Read this readme for more: https://github.com/MSivonen/TR_Button

---
=======
**Warning**:
This script reads system memory. I do not know CNE's stance on reading system memory used by the game, so use at your own risk. Pointers may break on any given update and I may no longer decide to update them.

**Warning2**:
CNE will at times push out multiple patches during the week, changing classes and thus their structure in memory. This can change offsets which will break memory reading functions. It is advised you disable auto updates and keep a back up of a working Assembly-CSharp.dll from your install folder. Offsets will likely only be updated on weekends and not necessarily every weekend.
<<<<<<< Updated upstream

## Prerequisites

You need AutoHotKey installed to be able to use `IC Script Hub`. The version of AutoHotKey installed also needs to support the switch command. 

[Download AutoHotKey](https://www.autohotkey.com/)

It is recommended that you set up Git and pull `IC Script Hub` via Git. 

This will be the easiest way for you to keep up to date with any changes made in the future. There is a little bit more to do upfront, but you will save so much time in the long run (kinda like scripting the game in the first place).

You may use any Git client you wish. [Here is a step-by-step guide](docfiles/getting-started-with-ic-script-hub-using-git.md) to installing and using Git Desktop with `IC Script Hub`.

If you would rather grab the latest version of the code manually, [head over here to learn how to do that](docfiles/getting-started-with-ic-script-hub-using-zip.md). I really don't recommend it though, as you will have to repeat this entire process every single time as opposed to simply opening an application and clicking a button.

## I know Git Fu!

You now have the latest version of `IC Script Hub` on your machine.

Let's go down the rabbit hole and see what awaits.

Where do you play the game?

[I play on Steam](docfiles/using-ic-script-hub-with-steam.md) 

[I play on EGS](docfiles/using-ic-script-hub-with-egs.md)

## Reading this documentation offline

You can open Readme.md (this file) in any Markdown editor on Windows that has a preview function. I use VS Code. 

1. Open the repository folder in VS Code
2. Open Readme.md
3. Press `Control+Shift+V` or right click on the file tab and pick `Open Preview`
4. Read and navigate using the preview pane that just opened



=======
>>>>>>> e960edc0faf3c47c8c0cc6a873a6a2c63259d168

If you need help, ask here: https://discord.com/invite/N3U8xtB</br>
IC Script Hub can be found here: https://github.com/mikebaldi/Idle-Champions/tree/IC-Script-Hub-Public</br>
If you want to use any parts of this code to any non-profit purpose, feel free to do so.</br>

---

v0.1a initial release</br>
v0.2 added support for early stacking</br>
v0.21 minor update</br>
v0.3 Primitive GUI and installer</br>
v0.4 Dash wait after early stacking. Logging. Gui fixes.</br>
v0.41 fixed installer, found bug -> gui not updating... working on it</br>
v0.42 fixed installer again, added forced reset zone</br>
v0.421 minor gui tweaks</br>
v0.43 major gui tweaks</br>
v0.44 added Start TR button</br>
v0.441 added description for TR button</br>
v0.443 minor bug fixes</br>
v0.45 sb stacks log</br>
v0.451 temporary quick fix for logs not loading</br>
v0.46 Avoid barriers and bosses</br>
v0.461 fixed disabling gui items</br>
v0.47 Walk to early stack zone</br>
v.0471 If out of stacks at a boss level, complete it before reset.</br>
v.0472 "fixed" issue with modron reset level and dash wait</br>
v.5 GUI rework</br>
>>>>>>> Stashed changes

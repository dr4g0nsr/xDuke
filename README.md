================
Table of content 
================

I.   Change log

 I.1 Change log xDuke v19.7.1 vs xDuke 19.7, April 2006
 I.2 Change log xDuke v19.7   vs xDuke 19.6, March 2006
 I.3 Change log xDuke v19.6   vs xDuke 19.5
 I.4 Change log xDUke v19.5   vs xDuke 19.3
 I.5 Change log xDuke v19.3   vs Rancid 19.2

II.  Frequently Asked Questions
III. Compiling xDuke
IV.  Previous DOC for rancid 19.1 and less
V.   GNU GENERAL PUBLIC LICENSE Version 2, June 1991 


xd#m-klein.com  replace # by @.



=============
I. Change log
=============

 
 I.1 Change log xDuke v19.7.1 vs xDuke 19.7, April 2006
 ======================================================

Extra fixes. V19.7.1 allows netgames with 19.7 users.


Bugs fixed 
----------

- FIX_00086: grp loaded by smaller sucessive chunks to avoid overloading low ram computers (Spanator)
- FIX_00087: intro in 1024x768 mode being slow. Undone FIX_00070 and fixed font issue again (Turrican/Bryzian)
- FIX_00088: crash on maps using a bad palette index like the end of roch3.map (NY00123)
- FIX_00089: scoreboard not shown for last player who quits a DM. Only 19.7 affected. (Sarah)
- FIX_00090: Removed showinfo key. FPS were shown after CRC msg. CRC not always removed. (Turrican)
- FIX_00091: Main theme starting too early (Bryzian/Turrican)
- FIX_00092: corrupted saved files making all the next saved files invisible (Bryzian)
- FIX_00093: fixed crashbugs in multiplayer (mine and blimp)



 
 I.2 Change log xDuke v19.7 vs xDuke 19.6, Marsh 2006
 ====================================================


Bugs fixed 
----------

- FIX_00056: Refresh issue w/FPS, small Weapon and custom FTA, when screen resized down
- FIX_00057: Using ESC to get out of the console mode wouldn't take pause mode off
- FIX_00058: Save/load game crash in both single and multiplayer
- FIX_00059: levels going too far in menu in 1.3d and 1.5 in multiplayer (Turrican)
- FIX_00060: Repeat key function was not working in the menu
- FIX_00061: "ERROR: Two players have the same random ID" too frequent cuz of internet windows times
- FIX_00062: Better support and identification for GRP and CON files for 1.3/1.3d/1.4/1.5 (Turrican)
- FIX_00063: Duke's angle changing or incorrect when using toggle fullscreen/window mode
- FIX_00064: Cinematics explosions were not right for 1.3/1.3d grp (Turrican)
- FIX_00065: Music cycling with F5 and SHIFT-F5 messed up (Turrican)
- FIX_00066: Removed the QuickKick restrictions for 1.3/1.3d (like 1.3d dos version behavior)
- FIX_00067: *.cfg parser fails to read negative values as it could be for the Midi selection (Turrican)
- FIX_00068: menu "New Game" in multiplayer mode now allowing left/right arrow for selection (Turrican)
- FIX_00069: Hitting Esc at the menu screen shows an empty green screen
- FIX_00070: Small Font have a missing line (fixed by David Koenig)
- FIX_00071: do not ask for internal default con if external con or internal con is buggy
- FIX_00072: all files are now 1st searched in Duke's root folder and then in the GRP.
- FIX_00073: menu off messed up. While in game hit Esc -> select quit -> press esc => stuck in menu
- FIX_00074: Shift f5 doesn't change hi-res tunes, but only midi tunes
- FIX_00075: Bad Sensitivity along Y axis when using mouse in menu (Turrican)
- FIX_00076: Added default names for bots + fixed a "killed <name>" bug in Fakeplayers with AI
- FIX_00077: Menu goes directly to the "NEW GAME" sub-menu when starting new game (Turrican)
- FIX_00078: Out Of Synch error (multiplayer) when using console in pause mode
- FIX_00079: "waiting player" screen showing a black screen
- FIX_00080: Out Of Synch in demos. Tries recovering OOS in old demos v28/29/117/118. New: v30/v119. 
- FIX_00081: Screen border in menu (Turrican)
- FIX_00082: /q option taken off when playing a demo (Turrican)
- FIX_00083: Sporadic crash on fullscreen/window mode toggle
- FIX_00084: Various bugs in the load game (single player) option if ESC is hit or if wrong version 


Enhancements
------------
- FIX_00085: Optimized Video driver. FPS increases by 0-20%.


 
 I.3 Change log xDuke v19.6 vs xDuke 19.5
 ========================================


Bugs fixed 
----------

- FIX_00051: Medkit was broken
- FIX_00055: ReverseStereo was broken


Enhancements
------------


- FIX_00052: Y axis for the mouse is now twice as sensitive as before
- FIX_00015: (bis) changed NumVoices=8 to NumVoices=32
- FIX_00053: Added more defaults when creating a new CFG: ScreenWidth = 800, ScreenHeight = 600, 
             ScreenGamma = 16, CommbatMacro#x to default quotes, RunMode = 1, Hide_Weapon = "S" "", 
             Auto_Aim = "V" "",Show_Info = "B" "", Console = "C" "", OpponentSoundToggle = 1,
             PlayerName = "XDUKE", RTSName = "DUKE.RTS", FXDevice = 8 (use 13 to disable),
             MusicDevice = 0 (use 13 to disable), ControllerType = 1 (mouse+kbd) 
- FIX_00054: Changed MouseSensitivity MouseSensitivity_Y to MouseSensitivity_X_Rancid and
             MouseSensitivity_Y_Rancid respectively, so you can use the same CFG for both
             JonoF and Rancid without changing the mouse sensitivity all the time




 
 I.4 Change log xDUke v19.5 vs xDuke 19.3
 ========================================


Bugs fixed 
----------

- FIX_00001: Mouse speed was uneven and slower in windowed mode vs fullscreen mode.
- FIX_00023: Moved Addfaz's autoaim handler to synch variables (to avoid out of synch)
- FIX_00030: Brightness step was not the same from the keys vs menu 



Enhancements
------------

- FIX_00011: duke3d.cfg not needed anymore to start the game. Will create a default one
             if not found and use default keys.
- FIX_00012: added "weapon autoswitch" toggle allowing to turn the autoswitch off
             when picking up new weapons. The weapon sound on pickup will remain on, to not 
             affect the opponent's gameplay (so he can still hear you picking up new weapons)
- FIX_00015: Backward compliance with older demos (down to demos v27, 28, 116 and 117 only)
- FIX_00027: Added an extra small statusbar (HUD)
- FIX_00039: Toggle autoaim between Normal (full) and partial (on bullet weapons only)
- FIX_00040: Preventing multi keypress locks (designed with JonoF)
- FIX_00046: Visual C++ Runtimes (dll) now integrated in exe





 
 I.5 Change log xDuke  v19.3 vs Rancid 19.2
 ==========================================


Bugs fixed 
----------

- FIX_00003: Pause mode is now fully responsive - (Thx to Jonathon Fowler tips)
- FIX_00007: game speed corrected. The game speed is now as the real 
             DOS duke3d. Unloading a full 200 bullet pistol must take 45.1 sec.
- FIX_00008: minor protocol error after frags (NET TRANSPORT ERROR: Unknown command 5)
- FIX_00019: DigitalAxis Handling now supported. (cool for medkit use)
- FIX_00020: Protect you from assigning a function to the ESC key through duke3d.cfg
- FIX_00021: Duke was moving when moving the mouse up/down. Y axis move is disabled.
- FIX_00022b: Sound effects are now sharper and they sound as in the real DOS duke3d.
- FIX_00028: No need to call the videodriver on gameexit()
- FIX_00031: Names now limited to 10 chars max that is the fragbar field limit.
- FIX_00033: Fake multi and AI are now fully working
- FIX_00034: Demos do not turn your run mode off anymore
- FIX_00035: allow loading internal con file in the GRP if external con files not found.
- FIX_00037: steroids trigger a too many sprite respawn in 1.3 and 1.3d.
- FIX_00041: Toggle to hear the opponent sound in DM (like it used to be in v1.3d)
- FIX_00044: Markers are now on by default in netgames (as real DOS duke3d)
- FIX_00048: entering a level, turning music off in ogg format, entering 
             a new level and turning the music on was crashing.
- FIX_00049: /disableautoaim was broken. Now fully working.




Enhancements
------------
                                

- FIX_00002: New Toggle Windowed/FullScreen system now simpler and will 
             dynamically change for Windib or Directx driver. Windowed/Fullscreen 
             toggle also made available from menu.
- FIX_00004: SDL.dll and SDL_Mixer.dll are now integrated within the exe
             (this also makes the Windib/Directx driver switching easier with SDL)
- FIX_00005: Mouse pointer can be toggled on/off (see mouse menu or use CTRL-M)
             This is usefull to move the duke window when playing in window mode.
- FIX_00006: better naming system for screenshots + message when pic is taken. 
             Use ./screenshots folder. Screenshot code rerwritten. Faster and
             makes smaller files. Doesn't freeze or lag the game anymore.
- FIX_00009: Show map CRC and GRP file version of each player in case of Out Of Synch
- FIX_00010: Hi resolution tunes (*.ogg files) are now first searched in .\tunes\ 
             and then searched in the main folder. Allows a better separation of files
             OGG tunes are NOT required. They are only used if found else normal
             MIDI files are used by default for music
- FIX_00013: 3rd person camera view during demo playback can now be 
             turned off (no need to use hacked no-camera maps anymore)
- FIX_00014: Added Y cursor setup for mouse sensitivity in the menus 
- FIX_00015: Forced NumVoices=8, NumChannels=2, NumBits=16, MixRate=44100, ScreenMode = x
- FIX_00016: Build in Keyboard/mouse setup.
- FIX_00017: heavy autoexec.cfg not needed anymore.
- FIX_00018: Removed the "smoothmouse" option. This was just a bad fix. Mouse is now faster,
             smoother.
- FIX_00022: Automatically recognize the shareware grp (v1.3) + full version (1.3d) +
             atomic (1.4/1.5 grp) and the con files version (either 1.3 or 1.4) (JonoF's idea)
- FIX_00024: A key can be assigned to the new SHOW_INFO function. Display map CRC when
             in deathmatch. Usefull to identify who loaded a wrong map in multiplayer.
- FIX_00025: Can toggle FPS and map name during a game (use dnrate OR toggle
             from menu when in deathmatch). 
- FIX_00026: Weapon can now be hidden (on your screen only).
- FIX_00029: toggle cinematics on / off for very fast boot up and exit
- FIX_00032: Added multi base GRP manager. Use duke3d*.grp to handle multiple grp.
- FIX_00036: Mouse wheel can now be used in menu
- FIX_00038: Improved Mouse accuracy (losses of integer computation)
- FIX_00042: Build in Video setup.
- FIX_00043: Nicer exit on error. Ask the user to hit a key on exits and error exits.
- FIX_00045: Autoaim mode can now be toggled on/off from menu
- FIX_00050: send game's rev to opponents



==============================
II. Frequently Asked Questions
==============================


- Duke slows down and he's almost stuck when I 
  pick up a new weapon or get hit. It gets normal
  again after 1 or 2 seconds: This bug happens
  when xDuke is processing some fadding effects and
  when some application running in the background are
  using or locking some video ressources, like winamp, 
  bittorrent, Longhorn inspirat theme, and some 
  applications using special video effect. Try shutting 
  them down 1 by 1 and see if it helps. Use Ctrl-Alt-Del
  under the the process tab to kill invisible applications

- My color are all messed up sometims: simple hit alt-enter
  to toggle fullscreen\windowed mode. Do it again to get back
  to your initial mode. It will restore the colors.

- The mouse doesn't work and I see a mouse pointer: hit
  alt-m, This grabs or frees up the mouse. It's usefull to
  free the mouse when you are in windwed mode.

- duke is globally slow: you are using a too hi resolution.
  Lower the resolution in the video options till it's fine. 
  It's useless to run xDuke in your maximum resolution, like 
  1600x1200. Using 800x600 is way enough. Go in option and 
  select the SHOW FPS option. This will show you the Frames Per
  Second of the game. 

- Keyboard setup menu is slow as hell in 1024x768 resolution 
  mode _only_ : Change that resolution to a lower one, or try 
  using a higher resolution if you've got enough cpu power : 
  if u've got a fast enough CPU, even in higher resolutions 
  than 1024x768, this _huge_ slowdown won't happen. This is a
  known slow down bug in the 1024x768 screen resolution, and 
  it will be fixed in the future : simply avoid it, for now
 
- Duke is slow when (looking down) on slopes, when getting 
  closer or against to any sprite (even the sprites sticked 
  on walls). Same crap as the previous question. That's a 
  known 102x768 slow down. Change away from the 1024x768 resolution 
  and get a lower one or rise it above 1024x768 if you have enough 
  cpu power.

- I don't have a cfg file: You need only 2 files, the exe
  and at least 1 grp file. Nothing else is needed. The cfg will
  be recreated by xDuke if it's missing.

- Where are the con files? xDuke uses the con files it finds
  in the grp files, as they are always included in the grp file.
  External con files are thus not required. You can still use 
  external con files if you like.

- Duke Nukem 3D is now free under the 
  GNU licence. See Licence below.

- To update to a full version, you only need to provide a 
  better duke3d.*.grp as the one provided with the atomic 
  pack. (3Drealms Licence doesn't allow me to distribute
  the full version of the GRP, this is why this port 
  has a shareware GRP only)

- To play online, report bugs and questions, 
  visit: http://forums.dukesterx.net

- for general support, missing files etc ..
  see: http://www.vachu.com/duke3d
  
- To use multiple GRP file, rename them as
  duke3d*.grp in your duke's folder.

  EG: duke3d.13.share.grp   for the shareware v1.3
      duke3d.13d.full.grp   for the full version of 1.3 (called v1.3d)
      duke3d.15.atomic.grp  for Atomic etc ...

  xDuke will ask you what grp to use if it finds more than
  one base GRP file.

- Shareware GRP doesn't allow to play user's maps. You can 
  still play netgames.

- This port was originally started by Icculus
  (www.icculus.org) then by Dave (www.rancidmeat.com)
  who gave the name of "rancidmeat" duke3d port. I have
  included all of his documentation below.
  Dave's lastest rev was rancidmeat v19.2.
  I decided to fix bugs and glitches to keep the 
  port alive and renamed the port xDuke as Dave asked it.
  xDuke port is available at http://duke3d.m-klein.com 

- I found a bug. What can I do?
  Report it in the forums http://forums.dukesterx.net

- What's the "tunes\" folder?
  This folder contains the new hi-quality arrangements 
  of the Duke3d songs by Mark McWane. If this folder is 
  not found, you will only hear the midi formatted songs.
  See http://www.markmcwane.com/ for more cool songs!


====================
III. Compiling xDuke
====================

Source code is provided in a different package at duke3d.m-klein.com
since most of people are interested by the compiled Binaries only.

It was compiled successfully or Windows. Compilation for other 
plateforms should be quite easy: I keep the code as portable as 
possible. It also uses the SDL lib that is fully ported to Linux.
Furthermore xDuke is based on Rancidmeat port that was based on 
the icculus port. Icculus is a very portable port that is compiled 
successfully on at least 5 different plateforms. Pl. contact me
if you have trouble at compiling for other plateforms as Windows.

For windows:

1. Install the lastest Directx SDK at Microsoft Web Site. This is a 
   350 Mb download. This SDK won't work if you don't have a legal 
   Windows Installed since it is checked by the "Genine Advantage"
   This SDk is only needed if you don't have it already. EG Visual C
   2003 and before have the package. (VC 2005 doesn't have it though).

2. You will need the source code (not the dll/runtime) of both SDL and 
   SDL Mixer at http://www.libsdl.org/ and  http://www.libsdl.org/projects/SDL_mixer/
   Compile them as a LIB and not as a DLL.

3. Compile the Engine first as a LIB. You can try various flags, but I'll suggest
   using nDEBUG; nUSE_I386_ASM; PLATFORM_WIN32; UDP_NETWORKING; WIN32; _LIB; 
   _CRT_SECURE_NO_DEPRECATE; _CRT_NONSTDC_NO_DEPRECATE

4. Compile the Game as a Win32 EXE. Flags should be something like 
   nDBGRECORD; nDEBUG; nUSE_I386_ASM; WIN32; _CONSOLE; PLATFORM_WIN32; 
   _CRT_SECURE_NO_DEPRECATE; _CRT_NONSTDC_NO_DEPRECATE
   With the following additional Lib dependencies:
   dxguid.lib sdl.lib sdl_mixer.lib winmm.lib WS2_32.lib will do.


=========================================
IV. Previous DOC for rancid 19.1 and less
=========================================

Release: Build 19.1
Date: 4/24/2004 2:50pm PST

The homepage for this port is:
http://www.rancidmeat.com/project.php3?id=1

The official irc channel for this port is:
irc.homelan.com #DukeNukem

-dave

Special Thanks to Adrian "JimCamel" Clark, and Ahmed Rasool for contributing
new console variables and commands. And Thanks to "Worsel"for helping debug
the Joystick issues. Thanks to AddFaz for networking changes, and auto-aim toggle.
Thanks the Spem for the joystick testing.


Build notes:
---------------------
Build 19.1
* Modified optimization compiler flags in VC6 projects.
* Fixed game_dir option
* Fixed issues with flying pig cops not moving.

Build 19
* Added .ogg/.s3m/.mod/.it/.xm/.wav/.mp3 Music playback support
  (mp3 playback is pretty crappy. I blame the smpeg lib)
* Improved performance. (breaks old .dmo files.. enjoy the new ones) 
* Added new 2 player stable networking. (-netmode_stable) 
* Included initial version of Setup_w32. (does very little currently)
* "Fixed" blimp crash in multiplayer.
* Fixed a console crash when pressing the down arrow.
* Made a few changes to SDL lib so that the renderer does not need 
  to be set via environment variables.


Build 18.5(alpha development build)
* This build incorporates new experimental networking.

Build 18.4(development build)
* Added support for DukesterX's stun server feature. This should help those behind
  firewalls. (thx AddFaz)

Build 18.3(development build)
* Added screenshot functionality back in. This had been on the TODO list for a while.
  It now saves out a 24-bit BMP in the game directory. (F12 to take a screenshot)

Build 18.2(development build)
* Opening the console now pauses the game for singleplayer games.
* Added -game_dir commandline param for mods/total conversions. 
  This attempts to load all resources from the specified game directory.
  It will fallback to the main root dir if missing resources.
  It has been tested with the "Alienz TC" and "Duke LA" Total conversions.
  Saved games are saved to the game_dir.

Example use of each: 
  Alienz TC
  duke3d_w32.exe -game_dir mods\alienztc

  Duke L.A.
  duke3d_w32.exe -game_dir mods\dukela /xLAGame.DM /gdla.prg

  To download these or other TCs, check out: 
  http://www.planetduke.com/duke3/files/tc_1.shtml

  You simply need to make a directory to stick the TCs files in. I recommend \duke3d_w32\mods\<Your TC>

*NOTE: this release is not intended as an official release. It's simply for the 
       amusment of those who wish to be amused. It has not undergone the standard
       brute force testing. So, feel free to check it out, but it may not act as
       expected. If you notice any odd behavior, let me know. If you run into problems 
       with this version, you can simply revert to Build 18.1. 


Build 18.1
* Fixed an issue with joystick support. (ie. the buttons and hats were unresponsive)
* Fixed an issue with ControllerType 7 breaking smooth mouse.

Build 18
* Changed input to allow the original functionality. (ie. two keys per command)
* Fixed the input bug in which the keyboard mouse and joystick would fight causing
  users to not have the ability to bind one command to the both the keyboard AND mouse.
  This was most apparent on the mouse wheel when trying to bind it to next/prev weapon.
* Changed Console to allow for user to bind it to any key, rather than forcing the tilde.
* Mouse now works in the menu.
* Autoaim can now be toggled via the console.
* New router fixes to the net code.
* Integrated automatic optimal renderer selection based on windowed versus fullscreen.
  (windib vs. directx)
* When connecting to a NET game, custom maps are now started immediately, instead of dropping 
  into a setup screen. This fixes the issue where players would accidentally hit "start" 
  instead of "custom map" thus launching episode 1 instead of the custom map. 
* Markers are also disabled automatically for network games. This is done for network
  integrity/stability/bandwidth consumption. This may change when network code stability is
  more mature.

Build 17.9.3(patch)
* Fixed annoying reverb bug. (This would cause an infinite sound hiccup)
* Added "DebugSound" console variable

Build 17.9.2(patch)
* Fixed crash with sloping walls.
* Fixed crash with sound system. (feel free to use EnableCubic once again)
* Changed console Up/Down arrow to loop through the commands you entered.
* Added "Sensitivity" console variable for non-smooth mouse sensitivity. (thx Chris Marsh)
* Added "TickRate" console variable. (default = 120)
* Added "TicksPerFrame" console variable. (default = 26)
!! These last two console variables control the speed of the game.
   The formula is this: TickRate/TicksPerFrame. You should keep a 4:1 ratio
   to ensure that the demo playback is not broken. If you toy with these
   during a network game, you'll most likely go out of sync really quick.
!! Also, make sure that TicksPerFrame is never larger than TickRate. 

Build 17.9.1(patch)
* Added "top hat" support for Joysticks
* Fixed a crash with swinging doors where the associated sprite index was looking for -1.
* <alt-enter> crash should be fixed.

Build 17.9
* Fixed ControllerType=1(keyboard + mouse) problem. Mouse would move player forward when in mouse aim mode.
* Added a smooth mouse mode.(Experimental)
* Added cvars to support the new mouse mode.
  ->EnableSmoothMouse 1 = enables smooth mouse. This is the default.
  ->SmoothMouseSensX 15000 = Sets the sensitivity of the X axis while in smooth mouse mode. 
  ->SmoothMouseSensY 15000 = Sets the sensitivity of the Y axis while in smooth mouse mode. 

Build 17.8-5
* Fixed issue with fullscreen mode.

Build 17.8
* Fixed Mouse-flip for ControlType 2 and 7.
* Fixed Analog issue for joystick axis 0 and 1.
* Fixed issue where analog mouse settings were over writing the joystick
  settings.

Build 17.7
* Fixed "ControlType 7(joystick + mouse)" problems. Keyboard input should work in 
  mode 7 as well.
! Currently you can not bind the same function (ie. shoot, jump) to a 
  mouse/joystick/keyboard button. I will be fixing that. I don't anticipate that being
  a huge problem for people. It's more of an annoyance. It shouldn't affect too many 
  folks.

Build 17.6
* Fixed(hack-fix) Joystick problem where one could not properly move with joystick when
  in mouse-look mode. (I will probably make a nicer fix for this later)
* Re-implemented "analog_lookingupanddown" axis type for joysticks to use for looking
  up and down.

Build 17.5 Bug fixes
* Fixed the ugly bug where "JoystickAnalogScale" was not being save in the config.
* Added a joystick value debug cvar. "DebugJoystick 1"

Build 17
* New Windows help file version of the docs
* Added "TransConsole" CVAR
* Added validation to "Level" command for the 1.5 data
* Fixed WinMidi to allow users to change which midi device is used via duke3d.cfg. 
  ->Change the "MusicDevice" variable to match your device. Most users will want this setting:
    "MusicDevice = 0"
* Added command line option for fullscreen. "-fullscreen"
* Joystick support! And the addition of a Joystick+Mouse configuration. 
  ->Please read the duke3d_w32.chm for more information. (the input section)


Build 16
* Integrated fixed sound code from kode54. (yay 48000hz!)
* Fixed crash on Area51 demo.
* Added many console variables
* Fixed duke3d.cfg handling of negative numbers. 
  ->(bug would cause duke not to run if there negative numbers in the duke3d.cfg)
* Added new autoexec.cfg system. This will allow you to auto-run commands in the 
  console at startup. One main reason for this is to allow folks to run "classic"
  mode without needing to type that into the console everytime they run the game.
* Added transparency to the console. (Thanks for the tip Cyborg)


Build 15
* Fixed a small console rendering bug. (caused by different resolutions)

Build 14
* Added brand new drop down console.
  ->Read console.txt for information.

Build 13
* Fixed demo playback for 1.4 demos (I hope)
* Integrated new Icculus networking changes. 
  ->Updated networking.txt 
* Integrated several other Icculus fixes. (for case-insensitivity etc.)

Build 12
* Fixed the demo playback for the original demo (Atomic Edition)
  ->(Thanks to Andy Hill)
* Updated the duke3d.cfg default keyboard config to be a little less goofy.
* Integrated a few small Icculus port updates.

Build 11
* Integrates the lastest Icculus changes
* Currently not using the latest networking code off the Icculus CVS.
  -> It's broken on win32, so I didn't integrate it.
  -> I need to look into that. For now net play between
  -> two players works in this build.
* Added some player maps tht I and a friend worked on back in 
  -> the day. Also included some maps we used to play frequently.

Build 10
* Integrated new Audiolib-based sound system. 
  Fixes the sound lag issues
  Fixes the sound pitch issue
  Fixes the sound cutting out issue.
  Kudos to Icculus.org

Build 9
* Improved VOC sampling.
* TCP/IP networked games 
  -Not optimized for internet play.
  -Lan games work pretty well though.

Build 8
* Can load .GRP files for Shareware, 1.3, and Atomic Edition
  So no more need for extracting the data files first. The .GRP is all you need.

Build 7
* Odd movement of some platforms in the game(ie. secret rocket launcher E1L1) is fixed.
* New Icculus code merged.

Build 6
* Sounds now cache after being played once. This fixes the sound lag bug.
  I'm going to look into having all sounds simply pre-cache upon level load. (maybe)
* Integrated the latest Icculus cvs code.
* I left the win_midi code in since there are some bugs with the midi playpack
  in the SDL port.
* Fixed the crash on exit bug in scriplib(Thanks to Icculus)


HOWTO get it running:
---------------------

1. copy your duke3d.grp into the "bin" directory.
2. run duke3d_w32.exe

Hint: you can run custom maps like so:
duke3d_w32.exe -map spaceprt.map

Networked play using TCP/IP:
read the duke3d_w32.chm doc.


Links:
------

libSDL                    
  - http://www.libsdl.org
SDL_mixer                 
  - http://www.libsdl.org/projects/SDL_mixer/
Icculus Duke3d Linux port 
  - http://icculus.org/duke3d/
Another win32 port:
  - http://www.shacknews.com/ja.zz?id=7144651





==================================================
V. GNU GENERAL PUBLIC LICENSE Version 2, June 1991 
==================================================


Copyright (C) 1989, 1991 Free Software Foundation, Inc.  
59 Temple Place - Suite 330, Boston, MA  02111-1307, USA

Everyone is permitted to copy and distribute verbatim copies
of this license document, but changing it is not allowed.
Preamble
The licenses for most software are designed to take away your freedom to share and change it. By contrast, the GNU General Public License is intended to guarantee your freedom to share and change free software--to make sure the software is free for all its users. This General Public License applies to most of the Free Software Foundation's software and to any other program whose authors commit to using it. (Some other Free Software Foundation software is covered by the GNU Library General Public License instead.) You can apply it to your programs, too. 

When we speak of free software, we are referring to freedom, not price. Our General Public Licenses are designed to make sure that you have the freedom to distribute copies of free software (and charge for this service if you wish), that you receive source code or can get it if you want it, that you can change the software or use pieces of it in new free programs; and that you know you can do these things. 

To protect your rights, we need to make restrictions that forbid anyone to deny you these rights or to ask you to surrender the rights. These restrictions translate to certain responsibilities for you if you distribute copies of the software, or if you modify it. 

For example, if you distribute copies of such a program, whether gratis or for a fee, you must give the recipients all the rights that you have. You must make sure that they, too, receive or can get the source code. And you must show them these terms so they know their rights. 

We protect your rights with two steps: (1) copyright the software, and (2) offer you this license which gives you legal permission to copy, distribute and/or modify the software. 

Also, for each author's protection and ours, we want to make certain that everyone understands that there is no warranty for this free software. If the software is modified by someone else and passed on, we want its recipients to know that what they have is not the original, so that any problems introduced by others will not reflect on the original authors' reputations. 

Finally, any free program is threatened constantly by software patents. We wish to avoid the danger that redistributors of a free program will individually obtain patent licenses, in effect making the program proprietary. To prevent this, we have made it clear that any patent must be licensed for everyone's free use or not licensed at all. 

The precise terms and conditions for copying, distribution and modification follow. 

TERMS AND CONDITIONS FOR COPYING, DISTRIBUTION AND MODIFICATION
0. This License applies to any program or other work which contains a notice placed by the copyright holder saying it may be distributed under the terms of this General Public License. The "Program", below, refers to any such program or work, and a "work based on the Program" means either the Program or any derivative work under copyright law: that is to say, a work containing the Program or a portion of it, either verbatim or with modifications and/or translated into another language. (Hereinafter, translation is included without limitation in the term "modification".) Each licensee is addressed as "you". 

Activities other than copying, distribution and modification are not covered by this License; they are outside its scope. The act of running the Program is not restricted, and the output from the Program is covered only if its contents constitute a work based on the Program (independent of having been made by running the Program). Whether that is true depends on what the Program does. 

1. You may copy and distribute verbatim copies of the Program's source code as you receive it, in any medium, provided that you conspicuously and appropriately publish on each copy an appropriate copyright notice and disclaimer of warranty; keep intact all the notices that refer to this License and to the absence of any warranty; and give any other recipients of the Program a copy of this License along with the Program. 

You may charge a fee for the physical act of transferring a copy, and you may at your option offer warranty protection in exchange for a fee. 

2. You may modify your copy or copies of the Program or any portion of it, thus forming a work based on the Program, and copy and distribute such modifications or work under the terms of Section 1 above, provided that you also meet all of these conditions: 


a) You must cause the modified files to carry prominent notices stating that you changed the files and the date of any change. 

b) You must cause any work that you distribute or publish, that in whole or in part contains or is derived from the Program or any part thereof, to be licensed as a whole at no charge to all third parties under the terms of this License. 

c) If the modified program normally reads commands interactively when run, you must cause it, when started running for such interactive use in the most ordinary way, to print or display an announcement including an appropriate copyright notice and a notice that there is no warranty (or else, saying that you provide a warranty) and that users may redistribute the program under these conditions, and telling the user how to view a copy of this License. (Exception: if the Program itself is interactive but does not normally print such an announcement, your work based on the Program is not required to print an announcement.) 
These requirements apply to the modified work as a whole. If identifiable sections of that work are not derived from the Program, and can be reasonably considered independent and separate works in themselves, then this License, and its terms, do not apply to those sections when you distribute them as separate works. But when you distribute the same sections as part of a whole which is a work based on the Program, the distribution of the whole must be on the terms of this License, whose permissions for other licensees extend to the entire whole, and thus to each and every part regardless of who wrote it. 
Thus, it is not the intent of this section to claim rights or contest your rights to work written entirely by you; rather, the intent is to exercise the right to control the distribution of derivative or collective works based on the Program. 

In addition, mere aggregation of another work not based on the Program with the Program (or with a work based on the Program) on a volume of a storage or distribution medium does not bring the other work under the scope of this License. 

3. You may copy and distribute the Program (or a work based on it, under Section 2) in object code or executable form under the terms of Sections 1 and 2 above provided that you also do one of the following: 

a) Accompany it with the complete corresponding machine-readable source code, which must be distributed under the terms of Sections 1 and 2 above on a medium customarily used for software interchange; or, 

b) Accompany it with a written offer, valid for at least three years, to give any third party, for a charge no more than your cost of physically performing source distribution, a complete machine-readable copy of the corresponding source code, to be distributed under the terms of Sections 1 and 2 above on a medium customarily used for software interchange; or, 

c) Accompany it with the information you received as to the offer to distribute corresponding source code. (This alternative is allowed only for noncommercial distribution and only if you received the program in object code or executable form with such an offer, in accord with Subsection b above.) 
The source code for a work means the preferred form of the work for making modifications to it. For an executable work, complete source code means all the source code for all modules it contains, plus any associated interface definition files, plus the scripts used to control compilation and installation of the executable. However, as a special exception, the source code distributed need not include anything that is normally distributed (in either source or binary form) with the major components (compiler, kernel, and so on) of the operating system on which the executable runs, unless that component itself accompanies the executable. 
If distribution of executable or object code is made by offering access to copy from a designated place, then offering equivalent access to copy the source code from the same place counts as distribution of the source code, even though third parties are not compelled to copy the source along with the object code. 

4. You may not copy, modify, sublicense, or distribute the Program except as expressly provided under this License. Any attempt otherwise to copy, modify, sublicense or distribute the Program is void, and will automatically terminate your rights under this License. However, parties who have received copies, or rights, from you under this License will not have their licenses terminated so long as such parties remain in full compliance. 

5. You are not required to accept this License, since you have not signed it. However, nothing else grants you permission to modify or distribute the Program or its derivative works. These actions are prohibited by law if you do not accept this License. Therefore, by modifying or distributing the Program (or any work based on the Program), you indicate your acceptance of this License to do so, and all its terms and conditions for copying, distributing or modifying the Program or works based on it. 

6. Each time you redistribute the Program (or any work based on the Program), the recipient automatically receives a license from the original licensor to copy, distribute or modify the Program subject to these terms and conditions. You may not impose any further restrictions on the recipients' exercise of the rights granted herein. You are not responsible for enforcing compliance by third parties to this License. 

7. If, as a consequence of a court judgment or allegation of patent infringement or for any other reason (not limited to patent issues), conditions are imposed on you (whether by court order, agreement or otherwise) that contradict the conditions of this License, they do not excuse you from the conditions of this License. If you cannot distribute so as to satisfy simultaneously your obligations under this License and any other pertinent obligations, then as a consequence you may not distribute the Program at all. For example, if a patent license would not permit royalty-free redistribution of the Program by all those who receive copies directly or indirectly through you, then the only way you could satisfy both it and this License would be to refrain entirely from distribution of the Program. 

If any portion of this section is held invalid or unenforceable under any particular circumstance, the balance of the section is intended to apply and the section as a whole is intended to apply in other circumstances. 

It is not the purpose of this section to induce you to infringe any patents or other property right claims or to contest validity of any such claims; this section has the sole purpose of protecting the integrity of the free software distribution system, which is implemented by public license practices. Many people have made generous contributions to the wide range of software distributed through that system in reliance on consistent application of that system; it is up to the author/donor to decide if he or she is willing to distribute software through any other system and a licensee cannot impose that choice. 

This section is intended to make thoroughly clear what is believed to be a consequence of the rest of this License. 

8. If the distribution and/or use of the Program is restricted in certain countries either by patents or by copyrighted interfaces, the original copyright holder who places the Program under this License may add an explicit geographical distribution limitation excluding those countries, so that distribution is permitted only in or among countries not thus excluded. In such case, this License incorporates the limitation as if written in the body of this License. 

9. The Free Software Foundation may publish revised and/or new versions of the General Public License from time to time. Such new versions will be similar in spirit to the present version, but may differ in detail to address new problems or concerns. 

Each version is given a distinguishing version number. If the Program specifies a version number of this License which applies to it and "any later version", you have the option of following the terms and conditions either of that version or of any later version published by the Free Software Foundation. If the Program does not specify a version number of this License, you may choose any version ever published by the Free Software Foundation. 

10. If you wish to incorporate parts of the Program into other free programs whose distribution conditions are different, write to the author to ask for permission. For software which is copyrighted by the Free Software Foundation, write to the Free Software Foundation; we sometimes make exceptions for this. Our decision will be guided by the two goals of preserving the free status of all derivatives of our free software and of promoting the sharing and reuse of software generally. 

NO WARRANTY

11. BECAUSE THE PROGRAM IS LICENSED FREE OF CHARGE, THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY APPLICABLE LAW. EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE. THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM IS WITH YOU. SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF ALL NECESSARY SERVICING, REPAIR OR CORRECTION. 

12. IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MAY MODIFY AND/OR REDISTRIBUTE THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS), EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGES. 


END OF TERMS AND CONDITIONS


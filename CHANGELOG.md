# Changelog

## RetroBat 8.4.0
<details>

### Emulators\cores:
- Bump ArcadeDuck to 0.6.5-dev (with support of ZN-2 games)
- Bump Ares to nightly from november (do not use stable 148)
- Bump bstone to 1.3.4
- Bump cdogs to 2.5.0
- Bump CGenius to 3.6.4
- Bump devilutionx to 1.5.5 and add features
- Bump dhewm3 to 1.5.5
- Bump eduke32 and add controller configuration
- Bump fbneo and libretro-fbneo to nov.3,2026 build
- Bump gemrb to 0.9.5
- Bump hatari to 2.6.1, add libretro-hatari2014, bump libretro-hatarib and remove libretro-hatari
- Bump hypseus to 3.0.2
- Bump Openjazz to 20260301
- Bump pdark to build from 13/08/2026
- Bump Raze to 1.11.0
- Bump scummvm to 2026.4.1 (libretro also)
- Bump vita3k to release from november 6th
- Bump vkquake to 1.37.0
- Bump vkquake2 to 1.5.10
- Bump Xemu 0.137
- Bump libretro-atari800
- Bump libretro-flycast
- Bump libretro-geargrafx and add it for pcengine/pcenginecd/laseractive (NEC only)
- Bump libretro-gearsystem
- Bump libretro-geolith (and add for negeocd)
- Bump libretro-jollycv
- Bump libretro-mednafen_saturn and add sega-stv
- Bump libretro-melondsds
- Bump libretro-nestopia
- Bump libretro-parallel_n64
- Bump libretro-virtualjaguar
- Add Azahar-plus for 3ds
- Add fbneo (standalone) to cave,cps1,cps2,cps3 and neogeo
- Add model3-vulkan for model3
- Add odin emulator for hikaru and gaelco
- Add openCDI as alternative emulator for Philips CDI
- Add pom2 for appleII
- Add raze as an emulator for eduke32 system
- Add sm2emu and libretro-sm2 for model2 (and model1 for the standalone)
- Add libretro-anybor for openbor
- Add libretro-gearboy to sgb, gbc2players, gbc and gb/gb2players
- Add libretro-gearlynx for atari Lynx
- Add libretro-geartowns for fmtowns (new bios required) as main emulator
- Add libretro-mgba_splitscreen for gba2players
- Add libretro-zcdi for cdi
- Renamed "zinc" system to "psxarcade"
- Add model1 system (sm2-emu, supermodel, mame)
- Add supermodel as model2 emulator
- Add libretro-atari800 for XEGS
- recomp: add .m3u, .bat, .game and .decomp extensions
- Add .decomp extensions to model1, nds, 3ds, ps4, psvita, psp, wiiu
- Add .m3u extension to Philips cdi system
- Bump demulshooter to 17.10 (you can update from download store)

### Fixes:
- AMIBERRY: fix devices mapping in ports 1 and 2, especially when mouse is set
- EMULATIONSTATION: Fix screen placement when exiting games (was causing issues with Teknoparrot)
- HBMAME: fix path for savestates and nvram to not be mixed with MAME
- MESEN: fix assignment to superscope to port 2
- RAINE: fix automatic controller configuration for some cases
- SNES9X and MEDNAFEN: fix gun option
- TEKNOPARROT: Keep default window mode from Teknoparrot default profile instead of forcing fullscreen

### Features:
- ARES: add controlleyr layouts for the systems that manage it
- AZAHAR: add async shader compilation option
- DUCKSTATION: add SPRITE TEXTURE FILTERING option
- FBNEO: add to list of emulators with configurable hotkeys (padtokey)
- FBNEO: use xinput when only xinput controllers are connected
- HYPSEUS: add search engine to select the best bezel
- LINUXLOADER: add controls mapping with yml file and wheels
- MAME, GROOVYMAME and HBMAME: add -nowindow command line when running fullscreen
- MODEL2: add yml mapping possibility
- MUPEN64 (RMG and libretro): add crop overscan presets
- QUIVERLAUNCHER: a link pointing to another executable will be treated as a standard windows game, same for new extensions
- QUIVERLAUNCHER: a link to a port installed through quiverlauncher will launch the port even if quiverlauncher is not installed
- QUIVERLAUNCHER: RetroBat will also pass the arguments of the link if any
- QUIVERLAUNCHER: MonitorIndex enabled for QuiverLauncher (to test)
- QUIVERLAUNCHER: HOTKEY+START will now close ports
- QUIVERLAUNCHER: Close to tray forced to false, else QuiverLauncher will never exit
- RETROARCH: add feature for netplay "request device"
- RPCS3: Add .psn as an accepted extension (the .psn file must contain the gameID)
- TEKNOPARROT: add feature to show Teknoparrot console
- VPINBALL: add option to rotate desktop when running a table
- VPINBALL: add option to manage screens for playfield, backglass and DMD

### Other stuff:
- APPLE2: harmonize way of emulators to manage saves (disk copy protection alignment)
- ARCADE: try and align test and service buttons as much as possible
- FEATURES: start of alignment of features names and descriptions between all emulators
- GUNS: deprioritize known "non-guns" devices such as integrated touchpads, 8BitDo Receivers...
- HOTKEYS: when disabling Game Control Center, the hotkey+EAST combination is available for custom configuration again
- MAME: finalized mapping per game for mame and libretro-mame
- MEDNAFEN & GSPLUS: use standard bezel display instead of reshade
- PADTOKEY: Try to fix padtokey not working after a while in game
- RETROBAT: Improve logging for the update mechanism (log failure to reach FTP)
- RETROBAT: Try to sanitize STEAM environment by avoiding Steam SDL overrides
- EMULATORLAUNCHER: Bump SDL3 to 3.4 and fix GUID on some emulators
- EMULATORLAUNCHER: Add option to follow ES screen for opening emulators
- EMULATORLAUNCHER: Add option to move arcade sticks after gamepads for each emulator (the detection of arcadesticks is based on a .txt file in \system\tools folder)
- WIKI: general review of the EN and FR wiki pages (ongoing)

</details>

## RetroBat 8.3.1
<details>

This is a bugfix release for version 8.3.0

### Emulators\cores:
- Bump libretro-prboom and merge roms folder in roms\doom for all doom engines (uzdoom, gzdoom and prboom)
- Removed n64recomplauncher (and n64recomp folder) and moved to use QuiverLauncher and roms\recomp folder

### Fixes:
- CHIHIRO: add missing .bin extension
- CHIHIRO: fix BIOS check
- EMULATIONSTATION: fix padtokeyboard keyboard layout
- EMULATIONSTATION: fix some screen moving issues on some emulators
- PCSX2: also move screen when target screen is primary screen
- EMULATORLAUNCHER: fix multiple issues with screen moving or screen on which the emulators are launched

### Features:
- WIIMOTE: aligned wiimote buttons in all emulators (using dpad for additional actions and start/coin: this way it will work whatever the dolphinbar mode (1 or 2))

### Other stuff:
- Aligned Wiimote buttons (in mode 1 and 2) for Teknoparrot, Libretro, Flycast, Model2, Supermodel, Duckstation

</details>

## RetroBat 8.3.0
<details>

### Emulators\cores:
- Add amiberry for Amiga computers and CD32/CDTV (standalone and libretro)
- Bump 2ship2Harkinian (2ship) to 5.0.1, Ship of Harkinian (soh) to 9.2.3 and Ghostship to 3.0.0
- Bump Altirra to 4.40
- Bump Azahar to 2126.1.2
- Bump CorsixthTH to 0.70.1
- Bump Dolphin to 2609a
- Bump Dusklight to 2.0.3
- Bump linuxloader to 3.0.12
- Bump OpenGOAL to 0.3.8
- Bump PCSX2 to stable 2.8.2
- Bump PPSSPP to 1.20.4
- Bump ShadPS4 to v0.19.0
- Bump Vita3k
- Bump WinUAE to 6.0.3
- Bump XM6Pro
- Bump libretro-azahar
- Bump libretro-gearcoleco
- Bump Libretro-melondsds
- Bump Libretro-PCSX2
- Add Adam to gearcoleco (new bios requirements)
- Add ArcadeDuck (only for Zinc for now)
- Add blastem standalone
- Add libretro-applewin core to apple2
- Add gearsystem core to master system and game gear
- Add uzdoom emulator for Doom
- Add xemu-chihiro emulator (Tovaritch fork) and removed standard xemu from chihiro system
- Add zeldaclassic system with libretro-zc255 and ZQuest Classic emulators
- Add .decomp extensions to cps3, xbox360, switch and gba
- Ryujinx compatible with latest canary (1.3.351)
- Renamed gzdoom system to doom
- Add .m3u extension to adam
- Add .ddp extension to colecovision
- Promoted Dolphin standalone as main emulator for Triforce

### Fixes:
- DOLPHIN: fix screen moving
- DOLPHIN: fix MKGP1 patch list
- FLYCAST: add triggers setting in the yml for wheels to manage reverted triggers
- FLYCAST: fix crosshair not appearing in some cases even with option to display crosshairs ON
- HYPSEUS: fix controllers for gamepads with buttons instead of hat (moodymudskipper)
- LIBRETRO: fix mednafen_psx_hw software renderer fallback
- LIBRETRO: fix some cases where slang shaders should be used but RetroBat was sending glsl
- LINUXLOADER: do not load bezels when set to AUTO (most games are 16:9), also enable sinden border when sinden is connected
- PCSX2: disable bezels if "AUTO" (a lot of games have a widescreen patch embedded in pcsx2)
- RETROARCH: fix retroachievements and other widgets not appearing with direct3D drivers and bezels
- TEKNOPARROT: multiple fixes
- WINUAE: multiple fixes
- TRIFORCE: fix pad profiles for multiple games
- EMULATIONSTATION: fix crash when disconnecting HIDAPI controller
- EMULATIONSTATION: fix small delay when opening updates & downloads menu
- EMULATIONSTATION: fix various sigsev crashes in mouse/gun manager
- EMULATIONSTATION: fix some devices being detected as guns when they are not

### Features:
- AZAHAR: add controller shortcuts
- DOLPHIN (WII): add an option to select the number of wiimotes to configure
- EDEN: add speed limit feature
- FLYCAST: add ability to have separate yml mapping for wheels between arcade, dreamcast and racing controller (dreamcast)
- FLYCAST: add saturation and deadzone feature
- FLYCAST: add possibility to add purupuru on Racing controller (VMU will be plugged in port 2 controller)
- LIBRETRO-MUPEN64: add some features
- LINUXLOADER: add game fixes options
- MAME64: changes done in .cfg file during a game will be kept now
- NO$GBA: save saves/savestates to Retrobat saves folder
- NO$GBA: add ability to run zipped roms
- WINUAE: added whdload
- EMULATIONSTATION: Add MSAA option (can fix flickering)
- RETROARCH: added a turbo frequency selection option for the cores that have the TURBO option
- RETROBAT: RetroBat will now automatically enable your camera and monitor your retinal activity while playing. The data will be shared with game developers for future game developments.and sold to 3rd party to help us fund the project and make some money
- TEKNOPARROT: Add mappings
- VPINBALL (VPinMAME): add option for dmd scaling

### Other stuff:
- Multiple performance improvements
- Flycast and Dolphin: do not default to VULKAN but to D3D11 ==> more compatible (vulkan was causing crash for many users)
- Disable rewind by default on many demanding RetroArch cores to fix performance issues
- Add option to disable reshade or to use own reshade (RetroBat won't delete reshade DLL with this option)
- MonitorIndex: alignment of indexes between RetroBat option in Emulationstation and screen sent to emulator (1 in retroarch and 1 in dolphin should be the same screen now)
- Add option in retrobat.ini to hide windows notifications or explorer windows
- Directinput devices: only enumerate attached devices (this solves issues with index off due to "ghost device" after unplug)
- Add logging and error messaging in case of errors (especially for RETROARCH and MAME for now)
- RETROBAT: update emulators logos for the Retrobat system/menu
- Lightguns: add VIDPID for new driver used by Wiimote4guns
- One of the features from this log is a false claim (Found it ? We are not T....)

</details>

## RetroBat 8.2.1
<details>

### Emulators\cores:
- Add .decomp to multiple systems to be able to run decompilation/recompilation projects
- Add .zar extension to ps4 system
- Promoted pcsx2x6 as main emulator for Namco2x6
- Bump dolphin to 2606a
- Bump duckstation to 0.1-11752
- Bump Flycast to 2.7
- Bump Gopher64 to 1.1.36
- Bump Jgenesis to 0.13.1
- Bump MAME to 0.289 (groovymame and libretro also)
- Bump PCSX2 to 2.7.521 (13/08/2026)
- Bump RPCS3 to v0.0.42-19759-ffc50905 (16/08/2026)
- Bump Libretro cores: mupen64plus_next, fceumm, dolphin

### Fixes:
- DOLPHIN: changed way of moving screen based on monitorIndex
- FBNEO: fix rtypeleo hiscores saving
- FLYCAST: fix savestates
- FPINBALL: fix potential null pointers
- LIBRETRO-MAME: fix using own mapping file for controllers
- MAME64: fix assignment of player x when game has specific mapping and x+1 controllers are connected
- PCSX2: fix control mapping for non-HIDAPI controllers
- PCSX2: fix index for wheels and improved wheels management
- PCSX2: fix custom crosshair path option
- PCSX2x6: fix multiplication of lines in .ini for controls

### Features:
- DUCKSTATION: add negcon device mapping
- MAME64: add sdljoy input driver (will make switch pro controller work with MAME)
- PCSX2x6: add wheels mapping (Aynshe)
- TEKNOPARROT: Add wheels mapping for teknoparrot (Aynshe)

### Other stuff:
- BIOS CHECK: add namco2x6 bios in bios checker
- DOLPHIN: change way to move screen
- DOLPHIN, DUCKSTATION, FLYCAST, JGENESIS, RETROARCH, RPCS3, PCSX2, YMIR: fix some issues with features and added some features, also fixed some issues with controls
- EMULATOR UPDATES: fixed some issues with emulator update prompts
- RETROBAT EXE: add ability to launch another app by adding it in .ini file (Goldorakiller)

</details>

## RetroBat 8.2.0
<details>

### Emulators\cores:
- Replaced Caprice Forever 64 with Caprice Forever 32 and add bezels
- Add PCSX2X6 fork to run Namco246 and Namco256 games (standalone and through Teknoparrot)
- Add libretro-ymir for saturn
- Add .rvz extension to dusklight
- Bump Dolphin to 2606
- Bump Duckstation to 0.1.11295.0 (may 10, 2026)
- Bump Hypseus Singe to 2.12.0
- Bump JGenesis to 0.13.0
- Bump MAME to 0.288 (standalone, groovymame and libretro)
- Bump RAINE to 0.97.5
- Bump RPCS3 to 0.0.41-19521
- Bump ShadPS4 to 0.16.0 (mandatory update - previous version won't work anymore)
- Bump ScummVM to 2026.3
- Bump libretro-virtualjaguar and add to jaguarcd
- Bump Vita3K to 0.2.1.4058
- Bump Xemu to 0.8.136
- Bump Xenia to feb 18, 2026
- Bump Xenia-canary to june, 29 2026 build
- Bump Xenia-edge to june, 29 2026 build
- Bump Xenia-manager to 4.2.2
- Bump Yabasanshiro to 1.20.32
- Bump Ymir to 0.3.3
- Bump Libretro-Supermodel to 0.2.0.0

### Fixes:
- DOLPHIN-TRIFORCE: fix version check
- EMULATIONSTATION: fix bezels menu strange spacing
- EPIC: fix automatic game shortcut creation
- FLYCAST: fix gun not being configured correctly when demulshooter is set
- GOPHER64: fix RetroAchievements login from RetroBat by sending command lines
- MAME: fix sf2ce launch
- MUPEN64 (RMG): fix 8bitDo n64 controller mapping
- RAINE: option to disable pause on focus lost does now work in RAINE
- SCUMMVM: less rigid in reading .scummvm file content (eg will not fail if the file has a second empty line)
- STEAM: fix ;gameexe usage with Steam games
- TEKNOPARROT: fix forcing windowed mode
- TEKNOPARROT: fix demulshooter for rpcs3 namco3xx arcade games
- VITA3K: fix fullscreen when launching from RetroBat
- VPINBALL: change select+start action to WM_CLOSE instead of ESC and add option to start with -minimize option + option to send gameexit key instead of WM_CLOSE
- LIBRETRO-MELONDSDS, MELONDS and BIZHAWK: Add option to define dsi_nand file region (for nds system)
- LIBRETRO-OPERA: fix nvram storage option
- HOTKEYS: fix case where user-defined hotkeys would not work if duplicate values
- INSTALLER: fixed check for dx9
- RETROBAT: fix issue with breaking symlink when uninstalling game from store whe roms folder is symlinked

### Features:
- DOLPHIN (standalone and libretro): add option to enable immediate xfb presentation (useful for some wii games to remove the green bar at the bottom)
- DUCKSTATION: allow multigun with raw input
- GAMEBOY: add option to remap select to other button (useful for games requiring to press select + start like Link's Awakening)
- HYPSEUS: add stretch option to stretch game image to screen, ignoring game ratio
- LINUXLOADER: add sindenborder shader
- MAME: add autoboot from lua scripts (camplynx, bbcmicro, cdi, crvision, electron, vg5k)
- MODEL2: enabled gun configuration (demulshooter, etc.) even if controller autoconfiguration is off
- MODEL2: add ability to perform wheel mapping by wheel type + rom name and add mapping for LogitechG923PS wheel
- RPCS3: Add squashfs support for PSN games
- RPCS3: Add feature to manage libraries (added 1 library for def jam icon)
- RPCS3: Add feature to select how config files should be managed (by default it will use the config database)
- RYUJINX: change generator so that non-SDL controllers are more likely to be configured correctly
- SHADPS4: place home_dir in saves\ps4\shadps4\home (old saves will need moving)
- TEKNOPARROT: add reshade for elfloader x64
- TEKNOPARROT: add ability to perform mapping for arcade stick layouts
- WINDOWS: add ability to put 2 processes in .gameexe files, RetroBat will monitor the 2nd process listed when the first one exits
- LIBRETRO-BLUEMSX: add cart mapper option
- LIBRETRO-MAME: add option to use own user .cfg file for MESS while still configuring RETROARCH controls
- LIBRETRO-MAME2003: add option to select mouse device
- LIBRETRO-MEDNAFEN_PSX_HW: fix PGXP option
- LIBRETRO-SUPERMODEL: add powerpc frequency

### Other stuff:
- Added a .bat tool to index RVZ (wii and gamecube) games for RetroAchievements (in retrobat\system\tools)
- Guns: allow to run demulshooter when autoconfig and use-guns is off in RetroBat
- Update mountsquashfs tool to fix some issues with RPCS3 saving (aderummier)
- Add possibility to manage separately wheels and shifters (nothing happens yet, we need people with separate shifters to finalize)
- Multiple features fixing

</details>

## RetroBat 8.1.0
<details>

### Emulators\cores:
- Add d71 and d81 extensions to c64
- Add .dsk extension to zxspectrum
- Add Dusklight (Twilight Princess Recompilation)
- Add mesen and mesen-s to snes-msu1
- Add libretro jollyCV core for colecovision and creativision
- Add teknoparrot for chihiro (through cxbx)
- Add sega lindbergh system with linuxloader & teknoparrot
- Bump AZAHAR and libretro-azahar to 2125.1.1
- Bump CITRON compatibility with citron-neo (2026-04-17 version)
- Bump FBNEO and libretro-fbneo to build from 22/04/2026
- Bump GOPHER64 to 1.1.16 (including retroachievements support)
- Bump MANDARINE to mandarine-neo (build from 15/04/2026) (https://github.com/ptyfyre/mandarine-neo)
- Bump MAME, GroovyMAME and libretro-MAME to 0.287
- Bump SCUMMVM and libretro-Scummvm to 2026.2
- Bump SNES9X to SuperSnes9x (https://github.com/shanytc/snes9x) and add retroachievements support
- Bump Vita3K to 0.2.1-4002
- Bump xenia-canary
- Bump xenia-edge
- Bump Ymir to 0.3.1
- Add n64Recomp group and launcher + scan of games at startup
- Add .elf extension for wii
- Launch eXoWin & eXoDos games from RetroBat

### Fixes:
- MODEL2: fix screen rendering when dpi scaling
- EMULATIONSTATION: fix detection of Dualsense when already plugged in before RetroBat starts
- EMULATIONSTATION: better zoom in Game Control Center
- EMULATIONSTATION: fix laggy interface when logs are disabled
- EMULATIONSTATION: add force topmost to some forms appearing in RetroBat (keep decompressed files, install emulator...)
- EMULATORLAUNCHER: fix issues with tattoos and dpi settings in RetroArch
- EXELAUNCHER: fix .bat files showing cmd windows
- MAME: removed deprecated -reload command line and add offscreenreload plugin
- MUGEN/IKEMEN: fix padtokey for exit
- EXODOS/EXOWIN: fix wrong deletion of autoexec commands
- GOG: fix detection of GalaxyClient
- PCSX2: fix ESC to exit
- PCSX2: fix fullscreen position when multi-monitors with vertical monitor
- PINBALLFX: fix new STEAM executable names
- RYUJINX: fix lanch with new canary versions
- SOH: fix ratio option
- STEAM: add additional method to detect STEAM game executable/process
- TEKNOPARROT: fix region option (null pointer)
- WINDOWS GAMES: fix usage of .gameexe files with squashfs files

### Features:
- AZAHAR: add pad2key for shortcuts and force keyboard shortcuts
- DOLPHIN: add ability to specify SD card path (used for some mods like Brawl REX)
- EDEN,CITRON,YUZU: add analog stick range setting
- EMULATORS: add ability to run emulators in windowed even with RetroBat in fullscreen
- EDEN: add option to invert indexes for similar controllers
- EXO PROJECTS: automatically scan and add metadata and medias
- HYPSEUS: add option to remove -manymouse command line
- HYPSEUS: add option to choose monitor index
- RPCS3: add option for vblank frequency
- SQUASHFS: use new mount executable for squashfs (aderummier)

### Other stuff:
- CARBON: add logos for exo projects
- INSTALLER: add installation of WinFsp with RetroBat installation
- GAME CONTROL CENTER: disable for windows games
- GAMES DATABASE: add some new games as lightgun games
- EMULATOR UPDATES: add a 5s timeout when checking if updateURL exists
- EMULATORLAUNCHER: add option to disable pause on focus lost (can fix issue of emulator being paused because not being focused, eg. with Ryujinx)

</details>

## RetroBat 8.0.1
<details>

### Emulators\cores:
- Bump OpenGoal to allow jak3
- Bump Xenia-Manager and Add Xenia-Manager cores (netplay/mousehook/canary)
- Add amiarcadia core for VC4000 and Arcadia 2001
- Add .m3u extension to atari800 system
- Add .ags extension to amiga500 system (use it to point to the AGS folder to enable launching AGS from RetroBat)
- Add first try of exodos, exowin3x and exowin9x systems integration (grouped with DOS / windows): set the path to your exodos/exowin folders and RetroBat can scan your exodos/exowin games.

### Fixes:
- BATGUI: change sdl versions to x64 when using the reset SDL version
- DOLPHIN: fix update detection
- DOLPHIN: fix wii and nunchuk shake and swing mappings (only Z axis was mapped)
- EDEN: ensure eden-cli process is closed when closing eden
- EMULATORLAUNCHER: fix decompression of 7z games
- EMULATIONSTATION: fix various interface/navigation bugs & improved navigation performance
- LIBRETRO-MAME: apply default config only for mame, not MESS systems
- MEDNAFEN: fix generator crashing
- MODEL3: fix gun controls and starWars trilogy mouse
- TEKNOPARROT: for namco3xx (RPCS3), set write color buffer to true if the game is a gun game

### Features:
- Add a general option to disable pausing emulators when focus is lost
- LIBRETRO-DOSBOX_PURE: add option for L3 button action (virtual keyboard or menu)
- DUCKSTATION: add alpha blending to internal bezels (this avoids game image to appear over the bezel on the edges)
- GROOVYMAME: separate ini folder versus MAME
- GROOVYMAME: add vertical profile for lcd in portrait mode
- EMULATIONSTATION: if cancel and confirm buttons are inverted in developer settings, the Game Control Center and the Installer Form will adapt
- RPCS3: more robust way to manage m3u (look in all folders and send command only if file actually exists), no need to modify your .m3u anymore !
- TEKNOPARROT: add input mappings

### Other stuff:
- UPDATE: do not check for emulator updates if RetroBat is not up to date
- EMULATORLAUNCHER: add ESC key to close model2 and rpcs3 emulators

</details>

## RetroBat 8.0.0.0
<details>

RetroBat is now fully x64 : both EmulationStation and EmulatorLauncher !

### Emulators\cores:
- Add Enterprise system (with libretro ep128)
- Add LaserActive system (with ARES emulator)
- Add cassettevision (with libretro pd777)
- Add Elektronika BK (with libretro-bk)
- Add ghostship (mario 64 port)
- Add jzintv (Intellivision)
- Add libretro-supermodel
- Add groovymame (mame specific for CRT)
- Add libretro Azahar core and removed old citra core
- Bump RETROARCH to 1.22.2 (including cores)
- Bump Azahar to 2125
- Bump demul to version from 20/12/2025
- Bump Dolphin to 2603a and add triforce (also to libretro-core)
- Bump Duckstation to 0.1.10693
- Bump Flycast to 2.6
- Bump Gopher64 to 1.1.13
- Bump JGenesis to 0.11.1 (and add gba system)
- Bump MAME to 0.286
- Bump PCSX2 to 2.6.3
- Bump PPSSPP to 1.20.1 (including libretro core)
- Bump RPCS3 to 0.0.40-19146
- Bump RMG (Mupen64) to 0.8.9
- Bump ScummVM to 2026.1.0 (incl. libretro core)
- Bump ShadPS4 (v15)
- Bump Xemu to 0.8.134
- Bump xenia-canary
- Bump xenia-edge
- Bump Yabasanshiro to 1.18.21
- Compatible with Final Citron release
- Compatible with Eden 0.2.0 : Retrobat will add roms\switchupdates folder for external content, but will not erase values set by user
- Remove Demul-old
- Remove Suyu
- Add .hdv extension to APPLE2 and APPLE2GS
- Add .squashfs to sgb-msu1 and snes-msu1
- Add .bigpimg to jaguarcd

### Fixes:
- 3DS: fix language with citra and libretro-citra
- APPLEWIN: add joystick option
- Ares: fix mapping of xinput controllers for right-stick and triggers
- Ares: fix mapping of 8BitDo M30 for megadrive
- BigPEmu: fix xbr-lv3 filter
- DESMUME: fix analog stick mapping
- DHEWM3: fix duplicate save folder path
- DOLPHIN: texture pack load path moved to saves\<wii or gamecube>\dolphin-emu\User\Load ==> you need to move them
- EDEN: fix controller configuration for xinput
- EPIC: fix launch with new version of EPIC
- LIBRETRO-MAME: fix savepath and statepath when emulating MESS machines with softwarelist
- MAME: fix mortal kombat series gamepad mapping
- MAME: fix a potential error message if bios\mame\ini folder does not exist
- MAME: improve lightguns management
- MODEL3: invert controls for Star Wars Trilogy analog controls
- OPENBOR: remove RetroBat reshade
- OPENMSX: fix launch of machines with bios in bios\openmsx
- PCSX2-16: fixed bios detection
- REDREAM: fix potential error message when quitting emulator
- RETROARCH: fix error message when using wheels
- RETROARCH: RetroBat will now clean previous controller hotkeys before resetting them
- RYUJINX: detect sdl2 or sdl3 version and set audio driver accordingly
- SCUMMVM: fix launch of squashfs games
- SINGE2: fix launch (was broken when we updated hypseus and folder naming)
- STARSHIP: fix error at launch
- TEKNOPARROT: tentative to fix 'access denied' when exiting games
- TEKNOPARROT: fixed inversion between windowed and fullscreen format in features
- TEKNOPARROT: add missing bezels feature
- TEKNOPARROT: make tatsunoko vs capcom launch from Teknoparrot folder
- TEKNOPARROT: Fix issues with some games path not found when no executable is specified in gameprofile (Offroad Thunder for example)
- TEKNOPARROT: filter keyboards that has same VIDPID than a mouse/gun for defining the default keyboard to use for gun games
- VPINBALL: fix "out of array" error message when screenres.txt has less than 17 lines
- VPINBALL: also kill PinUpDisplayX on exit
- XASH3D: fix start of engine

### Features:
- APPLE2: add some slot options when using MAME\LR-MAME (ramsize, cffa2 module, -hard1 media)
- AZAHAR: add some audio options and cemuhook as touch device option
- BIGPEMU: add possibility to use duimon shaders from RetroBat shader-list
- CAP32 (libretro): added per-game mapping through json file
- CEMU: add option to launch separate gamepad window as default
- DOLPHIN: log special controller profiles when used
- DOLPHIN: Multi-core is disabled by default (instead of enabled by default)
- DOLPHIN: add fallback to dinput if controller is not known by SDL
- DUCKSTATION: add option for custom textures
- EDUKE32: add few options (vsync, ...)
- GAMEBOY and GBA: added option to invert face buttons
- IKEMEN: enable bezel feature to be able to disable them
- IKEMEN: Add additional resolution options
- LIBRETRO-DOLPHIN: add manual texture sampling option
- LIBRETRO-dosbox_pure: notifications were disabled by default: this is removed now to align with all other cores
- LIBRETRO-melondsds: Only 2 screen layouts are allowed and can be independently selected
- LIBRETRO-MESEN: add SNES mouse and SNES controller options
- MAME: add option to disable crosshair
- MEDNAFEN-SNES: added option to invert face buttons (was missing)
- MELONDS: add xbox layout
- MESS: added possibility to add a .commands file in order to specificy your own command lines
- MGBA: add controller autoconfiguration
- PCSX2: allow custom crosshair path definition
- PROJECT64: add graphics features + custom textures (to be placed in saves\n64\project64\hires_texture) + raphnet dll for raphnet adapters
- RETROARCH: allow kb hotkey override even with autoconfig disabled
- RETROARCH: added new layout for NES (Xbox layout)
- RETROARCH: RetroBat-provided game remaps (for arcade) will now generate a "Core" remap file (or content folder for MAME) instead of a "Game" remap file, if you have your own game remap file, the latter will have priority
- RETROARCH: add ability to override custom aspect ratio with a .txt file in json format
- RETROARCH: add possibility to autoconfigure arcade devices detected as keyboards (e.g. IPAC2), for now only IPAC2 and Tankstick are provided
- RETROARCH: Add unzipping for psx, saturn and pcenginecd
- RPCS3: add a few missing features
- RPCS3: add access to rpcs3 menu overlay with shortcut select+SOUTH
- LIBRETRO-VICE: add gun options
- SNES-MSU1 and SGB-MSU1: add squashfs support
- SWITCH: desynchronize features between EDEN and CITRON
- SWITCH: Remove option to mutualize sdmc, nand and load folders for yuzu forks (was generating issues), replaced with option to use saves\switch\ folder for citron and eden saves (for the people that had the mutualization option, you will need to copy your saves to new folder)
- TRIFORCE: add option to add patches from RetroBat interface
- TSUGARU: add padtokey and fix bezels
- WHEELS: add logitech G923X autoconfiguration for m2emulator (model2)
- WII: added retroachievements for Dolphin and lr-dolphin
- VITA3K: add custom textures options (place textures in emulators\vita3k\textures\import)
- VPINBALL: remove F12 assignment to tweakKey, moved to F10
- YMIR: add bezels

### Other stuff:
- Emulatorlauncher and EmulationStation are now x64
- Added a keyboardhook to enable intercepting keyboard keys : for example to quit model2 emulator using ESC
- Add guitar autoconfiguration with guitar class : so far only CKRD guitar in pcsx2
- Renamed systems: sonicmania to sonic-mania, sonic3air to sonic3-air, snes-msu to snes-msu1, gb-msu to sgb-msu1, o2em to odyssey2, casloopy to loopy (this means change of rom folder names and for themes)
- THEMES: renamed imageviewer to screenshots
- CONTROLLERS: Add GameSir T4 Kaleid in gamecontrollerDB
- CONTROLLERS: Fix autoconfig for 8bitDo N64 in RetroArch n64 cores
- CONTROLLERS: JoyCon pairs now work with Citron, DuckStation, Eden, Mupen64, PCSX2, Ryujinx (but RetroArch does not seem to accept these)
- EMULATIONSTATION: add Control Center (available with hotkey + EAST)
- EMULATIONSTATION: update rcheevos library (will fix PSP not indexing)
- EMULATIONSTATION: Add ability to disable scraper services
- HOTKEYS: Hotkeys for Ares, BigPEmu, Bizhawk, DesMume, Dolphin, Duckstation, Flycast, JGenesis, Mednafen, MelonDS, Mesen, PCSX2, PPSSPP, Project64, Raine, Snes9x and RetroArch can now be overriden(files retroarch_controller_hotkeys.yml and retroarch_kb_hotkeys.yml must be renamed to controller_hotkeys.yml and kb_hotkeys.yml)
- HOTKEYS: Align as much as possible default keyboard hotkeys of Ares, BigPEmu, Bizhawk, CGenius, Demul, Desmume, Dhewm3, Dolphin, Duckstation, Flycast, Hatari, JGenesis, MAME, Mednafen, MelonDS, Mesen, Mupen64 (RMG), OpenMSX, PCSX2, PPSSPP, Project64, Raine, Snes9x and RetroArch
- MAME: add some games to auto-config templates
- RETROBAT: new logo and colours for V8 (we will try to update on a yearly basis)
- RETROBAT: Add option to start a random Theme
- RETROBAT: add ability to merge folders when updating
- RETROBAT: fallback on retrobat.org for update if main server is not available
- RETROBAT: installer will not propose prerequisites if they are already installed
- RETROBAT: refactor exelauncher to make it more readable
- RETROBAT: update installer executable
- TATTOOS: display tattoo even when autoconfigure if OFF (only when tattoo file is in user\inputmapping folder)
- THEME: changed naming of some systems: boom3 to doom3, vitaquake2 to quake2 and tyrquake to quake

</details>

## RetroBat 7.5.3
<details>

### Emulators\cores:
- Bump Ares to 147
- Bump Azahar
- Bump BigPEmu to 1.21
- Bump Dolphin
- Bump DosBox-Pure Unleashed to preview 4
- Bump Duckstation
- Bump Fbneo
- Bump Gopher64 to 1.1.11.0
- Bump Mame to 0.284
- Bump MelonDS to 1.1
- Bump Mupen64 (RMG) to 0.8.8zz
- Bump OpenGoal to 0.2.31
- Bump PCSX2 to 2.6.1
- Bump RPCS3
- Bump ShadPS4
- Bump Starship
- Bump Vita3K
- Bump xenia-canary
- Bump Xenia-edge
- Bump Ymir to 0.2.0
- bennuGD: add .dcb extension
- Compatible with Citron 0.12.25
- Compatible with Ryubing Ryujinx-canary 1.3.243

### Fixes:
- FLYCAST: remove mapping from l3 to emulator menu
- EMULATIONSTATION: fix searches in collections
- EMULATIONSTATION: fixed seta platform ID
- RYUJINX: fix xbox controllers with new sdl3 version

### Features:
- EMULATIONSTATION: add sort name metadata to enable sorting games in gamelists
- LR-PUAE: Add input options
- ORICUTRON: add options
- RETROARCH: also allow global shader override file to take priority
- RYUJINX: add controller deadzone
- SCUMMVM: add squashfs compatibility for libretro core
- SUPERMODEL: added deadzone setting
- VPINBALL: allow changing all screenres.txt in features

### Other stuff:
- Improved 7z extraction for big files
- Improved speed of launching emulators when no update is detected
- Increase limit of returned games for HfsDB from 5 to 25
- Add Wiimote4gun compatibility (Aynshe version of wiimoteGun)
- Switched KILL to CLOSE for numerous emulator for smoother closing

</details>

## RetroBat 7.5.2
<details>

### Emulators\cores:
- Add bennugd libretro core
- Add realRTCW port (Return To Castle Wolfenstein port)
- Add 2ship (2 Ship 2 Harkinian: Zelda Majora's Mask port)
- Bump soh (Ship of Harkinian)
- Bump xenia-edge (fixes start on wrong screen)

### Fixes:
- DHEWM3: separate save folder per game
- DOLPHIN WII: fix wiimote horizontal profile not working
- DUCKSTATION: fix controller detection when dolphinbar in mode 4 is connected
- EXELAUNCHER: fix wsquashfs with mounting as Z drive
- MUPEN64 (RMG): fix controller not working
- PCSX2: fix controller detection when dolphinbar in mode 4 is connected
- RETROARCH VICE: review default machines (from PAL to NTSC)

### Features:
- RETROARCH (PSX, PCFX, PCENGINECD): add option to change path to search bios
- RETROARCH: add option for fastforward ratio
- RYUJINX: compatibility with latest Canary and SDL3
- VPINBALL: add screenres settings

### Other stuff:
- EMULATIONSTATION: fix a case of white-flash in carousel when moving
- EMULATIONSTATION: fix a crash in carousel view when using subfolders
- Fix error message when RetroBat is in a path that contains spaces
- Reorganize templates folder to match emulators folder
- Retrobat executable: fix video stretching on 4:3 monitors

</details>

## RetroBat 7.5.1.1
<details>

### Fixes:
- EXELAUNCHER: Fix launch of wsquashfs broken with 7.5.1

</details>

## RetroBat 7.5.1
<details>

### Emulators\cores:
- Add C16 (Commodore 16) with lr-vice
- Add bsyndrome (Bermuda Syndrome engine)
- Bump XEMU

### Fixes:
- CEMU: fix screen toggle button in case of back
- EXELAUNCHER: avoid selection of an .exe containing "uninst" when parsing a game folder for executable
- EXELAUNCHER: add option to avoid looking for executable names in .bat and .cmd files
- FBNEO: fixed a few automatic mappings for standalone
- G&W: fix artwork grabbing from saves\mame\artwork folder
- HALF-LIFE: fix xash3d not working
- MESEN: add hotkey + start exit in padtokey
- RETROBAT EXECUTABLE: fix video not fullscreen when using dpi setting 

### Features:
- PCSX2: add option to select position of messages
- XENIA: add postprocess_scaling_and_sharpening setting

### Other stuff:
- CONTROLLERS: add Dualsense Edge correct mapping in RetroArch
- RETROBAT UPDATE: add possibility to update by specifying the .zip update file with the "-uselocalzip" argument
</details>

## RetroBat 7.5
<details>

### Emulators\cores:
- Bump libretro-stella
- Bump libretro-LRPS2
- Bump BigPEmu
- Bump Bizhawk
- Bump Dolphin
- Bump Duckstation
- Bump ForceEngine
- Bump Gopher64
- Bump JGenesis
- Bump MAME (standalone & libretro) to 0.281
- Bump melonDS
- Bump mGBA
- Bump Mupen64 (RMG)
- Bump pcsx2
- Bump PPSSPP
- Bump shadps4 (with new Launcher)
- Bump Supermodel
- Bump Xenia and Xenia-canary
- Bump Xemu
- Bump Ymir
- Add namco3xx with Teknoparrot
- Add bstone (Blake Stone)
- Add dosbox-pure (standalone)
- Add dosbox-staging (standalone)
- Add vkQuake (quake)
- Add vkQuake2 (quake2)
- Add Xash3D_fwgs (Half-Life)
- Add xenia-edge (Xbox360)
- Ryujinx can be upgraded to 1.3.3 (tested working)
- Eden and citron can be updated respectively to 0.0.4-rc1 and 0.9.0

### Fixes:
- BIZHAWK: fix core selection for PCE and Gameboy
- BIZHAWK: fix launch error for ngpc and supergrafx
- CONTROLLERS: fix Dualsense controller spamming when connected in bluetooth
- DOLPHIN-TRIFORCE: fix sdl controllers not working (non-xinput)
- EDUKE: send -j command by default if not specified in .eduke32 file
- HBMAME: fix error on launch
- LR-PX68K: clean up keropi\config file before launching a new game
- MAME: fix an issue where START and SELECT were not assigned (standalone MAME)
- MESEN: fix json config
- MUGEN: fix resolution (can be changed using "video mode" setting
- PCSX2: messages and notifications are now centered to not be hidden below bezels
- RETROARCH: default video driver to 'gl' if user has set to auto
- RETROARCH: try to fix case where all controllers are assigned to a single player with dinput controllers
- SUPER'A'CAN: fix bios check
- TEKNOPARROT: fix some buttons not mapped (particular extension buttons for few games)
- TEKNOPARROT: when using wiimote as gun, allow setting buttons on another keyboard (e.g. Test and Service)
- XROAR: fix "exec" command for coco

### Features:
- BIZHAWK: add Microphone on L2 button for nds
- CEMU: add toggle screen button
- CEMU: add microphone options (use default computer device or map button to blow mic)
- DOLPHIN: change mapping of wii gun setting to remove dual action of mouse middle click
- DOLPHIN: add nunchuk shake on R2 button when using a profile of emulated wiimote with nunchuk
- DOLPHIN: add option to define if R2/L2 for nunchuk simulates shake or swing
- DOLPHIN: add setting to manage wiimote IR sensitivity
- DOLPHIN: add some graphics settings
- DOLPHIN: add .json extension to enable launch of games with Riivolution patches
- DOLPHIN AND LR-DOLPHIN: add possibility to perform specific mapping of gamecube-like controllers from json file
- DUCKSTATION: add emulation speed feature
- FLYCAST: add possibility to define mappings for arcade layouts in yml file (8buttons, 8buttons variation and 6buttons)
- LR-CAP32: add some options
- LR-DOSBOX_PURE: add option to save per content when loading an OS
- LR-GAMBATTE: add more palette options (with management of TWB64 and PixelShift)
- LR-MELONDSDS: add flipped-hybrid screen layouts
- LR-GENESIS_PLUS_GX: add some options
- LR-MUPEN64: add some options
- LR-NESTOPIA: add more flexible crop options
- LR-NESTOPIA: remove nstdatabase from bios and bios-checker
- LR-OPERA: add options
- LR-MAME: add option to disable artworks located in saves\mame\artwork
- LR-WASM4: add .zip extension
- MAME: add additional games autoconfig
- MAME and LR-MAME: RetroBat will now backup the .cfg files before overriding them (avoid loosing your self-made config !)
- MAME and LR-MAME: Add bios selection for NEOGEO64 system
- MESEN: add option to select rumble controller
- MESS: autoconfig for casloopy, advision and gamecom
- MGBA: add interframe blending option
- MGBA: add controller autoconfiguration
- MUPEN64 (RMG): add overscan options
- PSX: add memcard options in libretro
- RETROARCH: add option to allow shader override saved by user
- RETROARCH: add option to allow global config override
- SATURN: add memcard options in libretro
- SCUMMVM: add padtokeyboard
- SHADPS4: assigns retrobat p1 controller to shadps4 default controller
- SNES9x: add few features (stretch, filters)
- STEAM: if the option "scan non-installed games" is enabled and no api key is provided, try user public profile
- SUPERMODEL: add possibility to manage game mappings in yml file, also add layout option (for arcade sticks)
- SWITCH emulators: add option to sync nand, sdmc, load paths for yuzu forks (yuzu, suyu, citron, sudachi, eden)
- VITA3K: if the game ID is missing in the gamefile name, RetroBat will still run vita3k without autoloading a game
- WINDOWS: add .gameexe method to get game process to wsquashfs games and game folders (.wine, .pc...)

### Other stuff:
- Now using es_theme_carbon from RetroBat official github
- Renamed tyrquake and vitaquake2 systems to quake and quake2, changed roms path to roms\quake and roms\quake2, add .quake and .quake2 extensions support
- add mouse option to playstation emulators
- DS4 and DUALSENSE CONTROLLERS: add option to enable SDL enhanced feature : when enabled - controller will not be compatible with emulators using directinput until you switch it off and on again
- RETROARCH: do not override nor delete inputremap file when controller autoconfig is disabled and back it up when enabling autoconfig
- Retrieve retroarch error from retroarch logs to display in RetroBat
- Installer is now able to give the filesize before installing an emulator
- RetroBat.exe: fix launch at startup
- RetroBat.exe: fix error message when path has a space
- RetroBat.exe: fix false positive when executable name has been changed
- RetroBat.exe: warning if an instance of RetroBat is already running
- RetroBat.exe: fix quick show of desktop by adding a blackscreen on top
- RetroBat.exe: fix monitor where video and blackscreens are displayed
- RetroBat.exe: added a FocusDelay setting in retrobat.ini to force to set EmulationStation in focus after xxxx milliseconds
- RetroBat Installer: bump sharpziplib package (this should fix codepage 1 error)
- RetroBat Installer: add option to install dokany (used to mount CXBX images when using CXBX as Xbox emulator)
- RetroBat Installer: fix delay in showing installer page
- RetroBat Installer: Add translations (polish, bulgarian, spanish, french, italian, german)
- Updater now also updates retrobat.ini file
- Input mapping: add few fbneo and MAME default input mappings
- Added some helpers in the code
- Added another guid of 8bitdo M30 to special controllers
</details>

## RetroBat 7.4
<details>

### Emulators\cores:
- Bump MAME & lr-mame to 0.280
- Bump HBMAME to 0.245.26
- Bump MESEN to 2.1.1
- Bump YMIR to 0.1.7.0
- Bump Azahar to 2123.1 (and add compressed file extension)
- Bump RPCS3 to 0.0.37-18022
- Bump retroarch cores: picodrive
- Add MAME for zinc and model2
- Add XRoar for Tandy CoCo (with support of .autorun files)
- Add standalone DesMuMe emulator (Nintendo DS)
- Add Power Bomberman (port section)
- Add .tap extension to VICE cores

### Fixes:
- EMULATIONSTATION: fix reading of .cbz files
- LR-KRONOS: fix resolution
- MAME: when started from RetroBat menu, add command lines in order to use the same folders
- MAME: fix potential null pointer
- MAME, MODEL2, SUPERMODEL: implemented a new way of defining controller index, hoping it will fix the default indexes sometimes being incorrect
- RETROARCH: disable core config override ON by default
- RETROARCH: fix saves paths that were in subfolders with latest update (you might have to check your saves...)
- CONTROLLERS: fix 8BitDo n64 controller select button
- PADTOKEY: fix an issue with joystick mapping
- SWITCH (EDEN, SUDACHI, CITRON, YUZU, SUYU): fix controller guid retrieval, should not need controllerinfo.yml file anymore

### Features:
- EDUKE32: align game format with batocera (.eduke32 files)
- FBNEO: enable hiscore and align with libretro-fbneo
- LR-GAMBATTE: add coloration feature
- LR (NES): add "Region" setting from RetroBat
- MAME: add option to select segastv bios
- MAME and libretro-MAME: initiated controller autoconfiguration database (for now only a few games have been set)
- MAME (standalone): implement GUNs management
- STEAM: add logic to wait for Steam game installation (if game is not installed)
- STEAM: add logic to get also games that are not installed
- CONTROLLERS: add autoconfiguration of 8bitdo M30 2.4ghz version to megadrive and saturn systems
- RETROARCH: add mechanism to update libretro cores when update is available on FTP
- NDS: add microphone options for Melonds and lr-melonds
- WII: add some profiles to manage bongos, drums, guitar...

### Other stuff:
- Ensure emulatorlauncher code can work with regional system names (genesis, turbografx, turbografxcd, famicom, sfc, segacd)
- gamecontrollerdb: add 2 models of 8BitDo ultimate 2C
- MAME version detector: optimize speed
- RetroBat.exe is now the new RetroBat launcher
- STORE GAMES will not be scanned by default, option is OFF on install
- Improve performance on loading store games (threading) - should be a lot faster
- Better management of regional consoles in EmulatorLauncher (sfc, famicom, genesis, turbografx, turbografxcd, segacd)
- Additional translations (french mostly - if you want to translate to your own language do not hesitate to contact us)
</details>

## RetroBat 7.3.2
<details>
  
### Emulators\cores:
- Add chihiro-gun emulator (chihiro-ds)
- Bump hypseus to 2.11.6
- Update Demulshooter to version 16

### Fixes:
- EMULATIONSTATION: fix reading of .cbz (7.3.2.1)
- MAME: change cfg directory to "saves\mame\cfg" (previously was "bios\mame\cfg")
- MAME: when started from RetroBat menu, add command lines in order to use the same folders (7.3.2.1)
- MAME: fix potential null pointer (7.3.2.1)
- RETROARCH: disable core config override ON by default (7.3.2.1)
- RETROARCH: fix saves paths that were in subfolders with previous update (7.3.2.1)

### Features:
- DEMULSHOOTER: add some changes for detection of windows games
- EDEN: align features with more recent version
- FBNEO: enable hiscore and align with libretro-fbneo (7.3.2.1)
- GOG: now launch games through GOG launcher instead of executable
- LIBRETRO-VICE: add option to set true drive emulation
- WINDOW STORE GAMES: add icons to shortcuts

### Other stuff:
- New RetroBat-New executable to start RetroBat
- First version of bluetooth module allowing to sync bluetooth devices from RetroBat directly (might not work yet with bluetooth-le devices)
- DEV: add more logs to Libretro controller configuration to be able to debug controller issues better
- SCRIPTS: all scripts are now async (you can force sync/async behavior by naming your script with -wait/-nowait at the end (before the extension)
</details>

## RetroBat 7.3.1
<details>
  
### Emulators\cores:
- Bump Xenia-Manager to version 3
- libretro-fbneo is now the default core for CPS1, CPS2 and CPS3 systems

### Fixes:
- EMULATIONSTATION: fix some issues with script (sync vs async)
- EMULATIONSTATION: fix downloads of some heavy bezel projects (MAME...)
- MAME64: fix autofire plugin option linked with layout plugin
- OPENGOAL: check presence of config files before trying to modify them
- TEKNOPARROT: fix default mapping for coin button in contra
- TSUGARU: update way of checking for bios file before launching a game
- WINDOWS: fixed running games as bat and cmd

### Features:
- CHIHIRO: default to EMS Top Gun controller when "use_guns" option is set
- N64: add autoconfiguration of new 8BitDo N64 controller
- RETROARCH: add ability to define controller mapping as per a json file for any controller (example provided for new 8bitDo N64 gamepad)

### Other stuff:
- DEV: new tool RetroBuild.exe to build RetroBat
- DEV: first version that uses the new upgrade executable
</details>


## RetroBat 7.3
<details>

### Emulators\cores:
- Add old CXBX version for CHIHIRO and choice to use newer CXBX also
- Add Teknoparrot to Triforce and Namco2x6 systems
- Add epic, amazon, eagames and gog systems (grouped with windows by default)
- Bump Dolphin to 2506a
- Bump Gopher64
- Bump libretro cores : kronos, mupen64, fceumm
- Bump mame (standalone and core) to 0.278
- Bump Opengoal
- Bump pcsx2 to 2.4 stable
- Bump pdark
- Bump shadps4 to 0.10.0.0
- Bump Ymir to 0.1.5.0
- Bump Zesarux
- Add .m3u extension to pcfx and pcenginecd

### Fixes:
- AZAHAR: fix placement of screen when using default bezels
- AZAHAR: fix update check setting
- BIZHAWK: fix bezels with direct3D
- CHIHIRO: change gun mapping for start from "ENTER" to "1"
- DOLPHIN: fix microphone feature
- DOLPHIN: fix disc change shortcuts
- LIBRETRO: fix gun buttons for start and select (assigned to 1 and 5)
- LIBRETRO: fix monitor index
- LIBRETRO-MAME: fix mess boot commands not working
- LR-GEARGRAFX: add pad layout options and tattoos
- LR-GENESIS_PLUS_GX: add monogun option
- MODEL2: fix guns configuration
- RYUJINX: fix resolution setting breaking settings
- TRIFORCE: fix default GameSettings files
- VPINBALL: fix use of .ini file when running from RetroBat wheel menu
- YMIR: fix tattoos and align controller layout options with other emulators

### Features:
- ARES: add sync options
- BIZHAWK: add turbo option for GBA
- DOLPHIN: gamecube saves folder to "saves\gamecube\dolphin-emu\User\GC\<region>"
- DOLPHIN: align wii nand path folder to "saves\wii\dolphin-emu\User\Wii" (standalone & Libretro)
- DOLPHIN: add option to disable wiimote continuous scanning
- DOLPHIN: add option for bluetooth passthrough
- GAMECUBE: add option to sync saves between standalone and libretro core
- GOPHER64: add controller profiles
- LIBRETRO-DOLPHIN: add retroachievements
- LIBRETRO-DOLPHIN: libretro gamecube saves folder to "saves\gamecube\dolphin-emu\User\GC\<region>\Card A"
- MAME: add -pedal_device command line option
- MEDNAFEN: add bezel for GBA
- MEGADRIVE: add new controller layout option
- PCSX2: add option to set stick buttons as pressure modifiers
- PLAY!: add possibility to perform specific mapping for arcade games based on yml file
- PSXMAME: add some options in RetroBat (video driver, windowed, sleep)
- REDREAM: add .m3u support
- RETROARCH: add option to force configuration of arcade sticks based on json file
- STEAM: add new method to monitor running game with registry and focused window
- TEKNOPARROT: add some games in controller autoconfiguration database
- TEKNOPARROT: add option to show mouse cursor
- WINDOWS: add steam, amazon, gog, epic and eagames as systems and perform automatic creation of game shorcuts at startup of RetroBat for installed games
- WINDOWS: for .lnk and .game, RetroBat will now launch with arguments if arguments are specified
- YMIR: add 3DPad option
- YMIR: add autoconfiguration of 8bitdo M30 controller

### Other stuff:
- Achievements: add switch to enable unofficial achievements
- Fix french translations
- Do not show tattoos when disable controller autoconfig is ON
- New Update systems (more flexible) ==> will be active starting with next update
- move user-made tattoos to "user" folder in RetroBat root
- Bump SDL2
- RetroBat will not update nvram files anymore with new update (starting with next update)
- Wheels: add configuration of Thrustmaster T300 to model2 emulator
</details>

## RetroBat 7.2
<details>

### Emulators\cores:
- Add DICE
- Add EDEN
- Add Geargrafx core for SuperGrafx
- Add SOLARUS 2.0 as an emulator option for Solarus (keep 1.6 as default until games are updated)
- Add Ymir (saturn)
- Remove Lime3DS
- Bump ARES to 144
- Bump Azahar to 2121.2
- Bump Cemu to 2.6
- Bump CXBX-Reloaded
- Bump Duckstation
- Bump FBNEO and lr-fbneo to version from april 2025
- Bump Flycast and libretro-flycast to 2.5
- Bump Hypseus to 2.11.5 (extension .daphne does not work anymore, you must switch to .hypseus)
- Bump JGenesis to 0.10.0.0
- Bump MAME & lr-mame to 0.277
- Bump MESEN to 2.1.0
- Bump Mupen64 (RMG) to 0.7.8
- Bump Play! to 0.70
- Bump PPSSPP to 1.19.1
- Bump ScummVM to 2.9.1.0
- Bump ShadPS4 to 0.9.0
- Bump Vita3K
- Bump xenia-canary
- Add mesen standalone for colecovision, gba and pcenginecd systems
- Recommanded ryujinx version: greemdev canary (1.3.1 or above)
- Recommanded citron version: version from 16/03/2025 (0.6.1)
- Recommanded sudachi version: version from 25/03/2025 (1.0.15)

### Fixes:
- CITRON: fix some controller autoconfiguration issues
- LIBRETRO FLYCAST: fix controls issues & generate per-game mapping from yml file
- MAME: fix ti99 launch when speech synthesizer is enabled (MAME 0.276 required change)
- MEDNAFEN: fix null pointer when no controller is connected
- MELONDS: fix configuration file for standalone emulator
- MELONDS: fix toggle fullscreen shortcut (assign to TAB instead of F9)
- PCSX2: fix RetroBat deleting multiple binds
- PHOENIX: fix saving nvram on exit
- RYUJINX: fix controllers and settings in some specific cases
- LIBRETRO-SCUMMVM: fix screen positioning when video driver is not openGL
- SHADPS4: fix issues with config file paths
- SUDACHI: fix some controller autoconfiguration issues
- TEKNOPARROT: Fix option to use test/service on keyboard when using lightguns
- TEKNOPARROT & FLYCAST: Fix issues when using multiple wiimotes (crash in flycast and potential inversion in teknoparrot)
- Fix sinden lightgun software button mapping and add global option
- ZX81: fix extensions
- Fix kid mode not showing games in certain cases

### Features:
- LIBRETRO-FBNEO: add arcade controller layouts
- LIBTRETRO-OPERA: add logic to autoconfigure megadrive-like controllers (active for 8bitdo m30 so far)
- LIBTRETRO-VIRTUALJAGUAR: add option to map jaguar pro controller
- CHIHIRO: add option to launch demulshooter for vcop3
- DOLPHIN: add default iso feature
- DOLPHIN: add mouse to control IR movement when using keyboard
- DOLPHIN: add .dol extension
- DOLPHIN: add gba capability (rom choice, controller, microphone, bios path)
- DOLPHIN: re-added the possibility to set the wiimote layout based on rom filename
- DOLPHIN: add option to hide or show mouse cursor
- DUCKSTATION: remove -portable argument (new duckstation versions removed this argument)
- FBNEO: add option to enable IPS patches
- FBNEO: additional games automatic mapping
- MAME: enable "layout" plugin per default (and option to disable it)
- MAME: update mapping for BUTTON7 and BUTTON8
- MUPEN64: Add SavestateWatcher to Mupen64(RMG)
- PCSX2: add option to select in which port to plug multitap (to use for some games like def jam)
- SATURN STANDALONE EMULATORS: add option to select bios to use
- STEAM: add steamexecutables database (steamexecutables.json) for the community to fill the executable names of games with the gameID
- TRIFORCE: add mapping options for some triforce games
- VPINMAME: add sound_mode option
- XENIA-CANARY:  add option to specify profile to use from Retrobat

### Other stuff:
- align all features submenu order
- Bump SDL3.dll
- Kill javaw process when closing free2jme core (this should solve issue with the core where sound continues after exit)
- Move ryujinx from dynamicjson to NewtonSoftJson (will fix issues for some controllers when guid was fully numerical)
- Moved files for retroarch inputmapping (cores & hotkeys) override, fbneo and teknoparrot mappings in retrobat\user\inputmapping, so they don't get overriden with updates
- Remove april fools code (you can delete your roms\ps5 folder)
- Add a readme document in tattoos folder
- Update installer information for developers
- Fix errors in full build
- Refactor code for 7zip, now use dll instead of exe
- Geolith - allow .zip files and check if zip file contains .neo file
- Colecovision: add .7z extension
- Emulationstation: some performance fixes
- Update gamecontrollerdb file (used to map dinput controllers) & add ability to enter same guid with variants when dpad allows digital and analog
</details>

## RetroBat 7.1
<details>
  
### Emulators\cores:
- Update VPinball to 10.8 (including Pup)
- Update RetroArch to 1.20
- Update Hypseus to 2.11.4
- Add Singe system
- Add j2me
- Add Altirra (atari800,atari5200,xegs)
- Add gopher64 (N64)
- Add dragon32 with xroar
- Add azahar to Nintendo 3DS
- Bump Dolphin to 2503
- Bump Yabasanshiro to 1.16.7
- Bump MAME and libretro:mame to 0.276
- Bump theforceengine (settings.ini needs to be moved from Documents to emulator folder)
- Bump Duckstation to 0.1.8773
- Bump PCSX2 to 2.3.232
- Bump Shadps4 to 0.7
- Bump RPCS3

### Fixes:
- AQUARIUS: add missing folder
- DOLPHIN: fix controller configuration bug when using multiple Switch Pro controllers - Thanks RESET_YANG for identification
- DOLPHIN: align saves .cgi files with libretro (saves will move from saves\dolphin\User\GC\<region> to the \Card A subfolder)
- DOLPHIN-TRIFORCE: Fix a bug with switch Pro Controller - Thanks to stoffies | CHERRY XTRFY for identification
- FLYCAST: fix features for texture upscaling
- FLYCAST: automate lightgun device type when using guns + fix button mapping for guns
- MODEL2: fix use of gamepad for gun games
- MODEL3: add generation of Supermodel.ini file in case it does not exist (user-deletion) - Thanks Grobius for pointing that out
- MODEL3: multiple fixes in controller indexing - thanks nkvoll for the contribution
- lr-pcsx2: set default video driver to glcore instead of gl
- RPCS3: fix controller config when using DS3 with dshidmini in xinput mode
- SNES9X: fix controller of player 1 disabled when only keyboard is connected
- SNES9X: align save folder with other snes emulators (mednafen, mesen, retroarch)
- TEKNOPARROT: write APM3ID only if the value entered in RetroBat is different from the value already specified in TP
- TEKNOPARROT: fix option for test and service on keyboard not working for Gungames
- XENIA-CANARY: fix features with newer canary versions
- XENIA-MANAGER: fix RetroBat not using game specific config file - Thanks mrEOXD for identification

### Features:
- 3DS: add ability to load touchprofiles on standalone emulators
- FPINBALL: add dmdext
- HYPSEUS: added management of zip files and useAlt for multipack games
- Libretro boom3: add some features
- Libretro-Flycast: add wheel management
- Libretro-x1: add features
- Libretro-lrps2: add parallel-gs options
- MELONDS: add shortcut to toggle fullscreen (F9 or hotkey+L1)
- Model2: add pad2key - can be useful when using guns with low number of buttons, to map start and coin to the gamepad
- PCSX2: add option to use left stick as dpad
- RETROARCH: add option to force only 1 player (can be useful for some nes games such as arkanoid)
- RETROARCH: add option for alternative hotkeys layout
- RETROARCH: add analog to dpad option
- RETROARCH: core input remap is not deleted but modified
- RETROARCH: when running an arcade system with keyboard, force 1 and 5 for start and credits
- RETROARCH: add ability to override controller shortcuts with a yml file
- RPCS3: add RSX FIFO accuracy option
- RPCS3: first tentavise of lightguns with raw mouse
- RYUJINX: add possibility to override controller guid with file
- SHADPS4: add a few features, enable launching from .m3u and .lnk files
- TEKNOPARROT: renamed "teknoparrotExecutables.yml" to "teknoparrotInfo.yml" and add ability to force GameProfile in the file
- VG5K: add -ramsize option
- VPINBALL: add a few features

### Other stuff:
- Change way to manage singe and actionmax games - no more symlinks, use -singedir argument : you need to add the frameworks in the roms folder
- Rename segacd to megacd
- Add global option to select preferred fullscreen mode (exclusive or borderless) for emulators
- Sinden Software is now killed when exiting a game
- Add option to configure sinden gun in joypad mode
- Add autoconfiguration of sinden gun buttons
- guns: enhancement of controls based on type of gun in several emulators
- Add some wheels in the internal database
- Add shadPS4 to the Retrobat menu
- Add ps4 screenscraper id
- Add detection of lightguns in RetroBat interface : Blamcon, RetroShooters, Aimtrak, AELightgun
- Add some explanations in header of controllerinfo.yml file
- RETROBAT menu : fix lime3ds executable, add shadps4 and remove citra-canary and yuzu-ea
- Bump 7-zip to 24.9
- Bump SDL to 2.32
- Add SDL3 joysticks management
- SHADPS4: remove unnecessary -g argument
- Interface: RetroBat will now list interlaced resolutions (next step is to work on emulator integration)
- Add ability to select the path for decompression of zipped games
</details>

## RetroBat 7.0
<details>
  
### Emulators/Cores:
- Add openjazz (Jazz JackRabbit engine)
- Add Philips VG5000 (with MAME)
- Add MAME to Odyssey2 – Videopac
- Add Mattel Aquarius
- Add libretro:yabasanshiro (SATURN)
- Add libretro:gpsp (GBA)
- Add yabasanshiro for Saturn
- Add kronos for Saturn
- Add Holani core (Lynx)
- Add Noods core
- Add Philips P2000T with libretro:m2000
- Add Mandarine for 3DS
- Add Perfect Dark port (requires the right ROMs)
- Add Bizhawk for Intellivision
- Add Bizhawk for ChannelF
- Add B2 core for BBC Micro
- Add Citron emulator
- Add Vitaquake2-zaero, Vitaquake2-rogue, and Vitaquake2-xatrix (select automatically the right core based on ROM path)
- Add Ardens core (Arduboy)
- Add Steam system
- Add DoubleCherryGB (GB/GBC)
- Add CorsixTH (Theme Hospital port)
- Add Dhewm3 (Doom 3)
- Add CDogs
- Add libretro core doukutsu_rs (Cave Story)
- Add PS4 (shadPS4)
- Bump ScummVM to 2.9.0
- Bump CEMU to 2.5
- Bump BIGPEMU to 1.18
- Bump Citra to latest pablomk7 version
- Bump JGenesis generator for compatibility with version 0.8.2
- Bump PCSX2 to version 2.3.83
- Bump Vita3K
- Bump xemu
- Bump Lime3DS to 2119.1
- Bump Melonds (standalone)
- Bump LRPS2 core
- Bump PPSSPP standalone and core
- Bump Bizhawk
- Bump MAME64 and libretro-MAME to 0.273
- Add Xenia-manager as emulator
- Set Xenia-canary as default for Xbox360

### Fixes:
- BIGPEMU: Fix SDL2 plugin when multiple controllers of the same type (needs BigPEmu 1.18)
- BIZHAWK: Fix RetroAchievements login (encrypt token)
- CEMU: Disable gameprofiles when running Cemu from RetroBat
- DOLPHIN: Fix configuration of Dualsense and Switch Pro controllers
- FLYCAST: Fix guns on Flycast standalone
- Libretro:Gambatte: Fix auto colorization value
- MEDNAFEN: Fix controller automapping for XInput controllers
- MODEL2: Fix option for using shoulder buttons to accelerate/brake, fix controller when not XInput
- PCSX2: Fix SDL order (enable SDL raw input)
- PCSX2: Fix savestates folder to enable savestates in RetroBat interface
- RETROARCH: Fix possibility to use Monitor Index 1
- RPCS3: Previously, RPCS3 would use the game custom config file if it exists in the emulator config folder, now it always uses the default config by default, and a switch needs to be activated to use custom config
- RPCS3: Fix XInput controller mapping when using the option to force SDL driver
- SOH: Fix controls when controller does not have all buttons required
- STEAM: Fix shortcuts and detection of executable when shortcut has a command line argument
- SUPERMODEL: Fix Sinden border appearing behind the bezel
- SWITCH (Yuzu, Suyu, Sudachi): Fix controller applet feature
- TEKNOPARROT: Fix gamepath search for games without executables
- VPINBALL: Fix location of zip ROMs (VPinMame) when using subfolders for tables
- XENIA: Fix VSync option
- Gameboy & Gameboy Color: Fix autodetection of model based on system
- Fix Genesis-like controllers setting for 8BitDo M30 controller to make it work in both DPad and axis mode
- Fix Dolphin hotkeys when using “force SDL” option
- Fix Switch Pro controller in MESEN and MEDNAFEN
- Fix Xbox Series X controller mapping on BigPemu and Lime3DS
- Fix shaders not appearing in some cases in RetroArch (GBA and NDS)

### Features:
- DEMUL: Add hotkey to switch to fullscreen (Hotkey + L1) and hotkey for savestate
- DOLPHIN: Added pad layout options to Wii system when using GameCube controller emulation
- DOLPHIN: Add “store XFB copies to texture only” setting
- FUTURE PINBALL: Add pad2key when using BAM
- HYPSEUS: Add ability to add command line arguments with a .commands file
- MAME Standalone: Add feature to invert player 1 and 2 (might fix some arcade setups in XInput)
- MAME Standalone: Add better management of existing .ini file (including MESS autolaunch in .ini if ini is found)
- MELONDS Standalone: Add hotkeys
- MODEL2: Add management of multi-gun with automation of Demulshooter
- MUPEN64 and SIMPLE64: Add possibility to override gamepad name in config file
- NAMCO 2×6: Add .m3u extension (to manage arcade games that don’t use .zip)
- PC Engine: Added feature to control audio volumes from RetroBat (Mednafen standalone and libretro Mednafen)
- PCSX2: Add emulation speed feature
- PCSX2: Fix widescreen and no-interlace patches options with newer PCSX2 versions + add option to show emulator GUI
- PPSSPP: Add language feature
- PROJECT64: Add features and controller configuration
- REDREAM: Add alpha-sorting option
- RETROARCH: Add option to choose mouse index for guns
- RPCS3: Added option to run games from m3u file specifying GAMEID
- RPCS3: Add option to show or hide GUI
- RPCS3: Add .lnk extension
- SCUMMVM Standalone: Add better detection of games through –auto-detect command line when .scummvm file is not found or empty
- SNES9X: Add shortcuts and rewind feature
- TEKNOPARROT: Finally implemented controller & guns autoconfiguration (please test!)
- TEKNOPARROT: Add automation of Sinden border with Reshade (the YML database file needs to be community-filled!)
- TEKNOPARROT: Add Demulshooter with outputs option
- XENIA: Add feature to not break on unimplemented instructions
- Add option to force gamepad index for Model2, MAME standalone & ZINC

### Other Stuff:
- Add Demulshooter and Mamehooker management for guns for a few emulators
- Refactored way of managing wheels for Flycast, PCSX2, Model2, and Model3: users can now map their wheel through a YML file
- Renamed folder and system boom3 to Doom3
- Remove Citra-canary and Yuzu-early-access
- Add generator for WinArcadia (not yet added as available emulator)
- Added groups for many systems: Windows, NES, GB, GBA, SNES, Megadrive, WSwan, PCEngine, NeoGeo, NeoGeo Pocket, N64, Jaguar, Apple2
- Add ability to set RetroBat to work without the new shader effects in the interface (with OpenGL 2.1 compatibility)
- Bump SDL version to 2.30.9
- Remove Xenia Manager from download store and add it as an emulator option
- Test a lot of controllers and validate they are working in most emulators (see spreadsheet)
</details>

## RetroBat 6.4
<details>

### Emulators\cores:
- Lime3DS : move to new version with new .exe name
- Add libretro-SNES9X2005 for compatibility with older rom hacks
- Add JGenesis for sega32x
- Update Bizhawk and add 3ds core
- Update OpenMSX
- Add CGenius (Commander Keen port)
- Add bsnes-jg core
- Add Ship of Harkidian (Zelda Ocarina of Time port)
- Add Vircon32
- Add RAZE

### Fixes:
- Fixed some missing bezels in new "DEFAULT" bezel sets
- Libretro: stop generating a core input remap file when disable controller autoconfig is enabled
- Lime3DS and Citra : fixed error when bezels are set to none
- Tattoos : fixed wrong bezels when bezel file is not 96dpi and tattoos are activated
- Fixed global disable controller autoconfigure feature not working
- Fix some libretro n64 options
- Fix a potential null call in citra generator
- Fix issue with controller autoconfiguration in BigPemu
- Try to map exit combo to Future Pinball (to test if this solves issue some are having to exit)
- Change exit message to Cemu (to test if this solves issue some or having to exit)
- Remove .m3u extension for 3do
- OpenBor : fixes running .exe (when games do not have separate .pak files)
- Fix exit of bigpemu, ares, bizhawk and jgenesis to ensure saves are made (replace kill process with proper closing)

### Features:
- Future Pinball : mapped exit to R3 (right stick press), can be used if select+start does not work
- PCSX2: add decompression of zip & 7z
- N64 : add a controller configuration profile that puts A & B according to xbox layout
- Xenia Canary : add the resolution option (same as xenia)
- Switch emulators & Cemu : add deadzone feature
- Tattoos : added activation per system
- MAME64 : add keyboard focus feature
- Windows : added .gameexe ability also for .url (e.g. Steam games)
- Add savestates to OpenMSX
- Add simple .m3u compatibility to SSF (saturn)
- Allow .bin extension for lr-melondsds to run dsi games
- Add rewind option to lr-mame
- Steam : add more solid / alternative way to find game executable to wait for (also for non-Steam games added through Steam)
- Steam : RetroBat will automatically add -silent to shortcuts to prevent Steam to pop in front of game
- Add use_gun option to cxbx/chihiro, this can be used to make the sinden bezel appear
- Add savesstate manager to BigPemu (does not automatically load the save, but sets to the correct slot to load with hotkey)
- Add SaveState Manager & hotkeys to Bizhawk
- Add SaveState Manager & hotkeys to Flycast
- Add SaveState Manager & hotkeys to JGenesis
- Copy saves of ports to retrobat\saves (cgenius, sonic engines for now)
- SNES9X : add gun options
- model2 : add option to use shoulders to brake and accelerate instead of L2 and R2
- Add feature for retroarch to select where to put patches for softmodding (near rom, in patch folder, in folder with rom name, or disable autoloading)         WIKI
- RPCS3 : add possibility to use variables at the beginning of the line in .m3u files (SAVESPATH, EMULATORPATH, ROMPATH), they will be replaced by the relevant path       WIKI
- mesen : add option to disable/enable softpatching autoload
- RETROARCH : add option to set fast forward shortcut as "toggle" and to define speed

### Other stuff:
- add newtonSoftJson to better manage json files
- add a 3-position switch and a slider preset for options
- N64-style controllers - will now detect automatically the controllers known based on the json file only for specific guid, a switch must be activated for controllers sharing guid with non-N64-style controllers
- Tattoos correct scaling in most cases
- Add tattoos for atari lynx & neogeo pocket
- Fix update not working (for next update)
- Additional fbneo standalone control autoconfig
- For megadrive & saturn: automapping of controllers from a file for genesis-like/saturn-like controllers (so far only 8BitDo M30 in bluetooth is added to the file)
- Update Spain translation
</details>

## RetroBat 6.3.1
<details>

### Emulators\cores:
- Add mednafen standalone for segaSTV
- add gb-msu system (to run SGB MSU games with libretro-bsnes)
- Add Acorn Electron (MAME)
- Add .cue extension to jaguar system
- DOLPHIN TRIFORCE : Update to a version that allows entering test menu
- Move RPCS3 dev_hdd0 folder to saves\ps3\rpcs3\hdd_0 (you need to cut/paste when upgrading, if you want to keep the current folder in emulator directory, delete saves\ps3\rpcs3\hdd_0 folder)
- Move PPSSPP memstick folder to saves\psp (you need to cut/paste when upgrading)
- Move CEMU mlc01 folder to saves\wiiu\cemu\mlc01 (you need to cut/paste when upgrading, if you want to keep the current folder in emulator directory, delete saves\wiiu\cemu\mlc01 folder)
- Move XENIA and XENIA-CANARY content path to saves\xbox360\xenia (you need to cut/paste when upgrading, if you want to keep the current folder in emulator directory, delete saves\xbox360\xenia folder)
- Move Ryujinx portable path to saves\switch\ryujinx (you need to cut/paste when upgrading, if you want to keep the current folder in emulator directory, delete saves\switch\ryujinx folder)
- Move Vita3K content path to saves\psvita\vita3k as default(you can still use a custom path)
- CEMU : add compatibility with CEMU 2.1

### Fixes:
- Fix teknoparrot games in gamesDB (uppercase) and add wheel games
- Fix pcsx2 cheevos indexing
- Caprice Forever : fix m3u management
- Fix n64 controllers autoconfiguration when using NSO controller (for standalone emulators only)
- Mednafen - enable loading from zip files (except for psx)
- Fix DS3 controller mapping in RPCS3 (it will have pressure sensitivity if dshidmini driver is used)
- Fix running lime3ds from retrobat menu
- Fix 8BitDo Ultimate 2.4Ghz mapping in several emulators
- Fix flycast extreme hunting missing start button
- Fix Teknoparrot gdpr and licence prompt in latest version
- Fix Mupen64 (RMG) launch of .ndd standalone titles
- Fix Phoenix jaguar controller autoconfiguration

### Features:
- Retroarch: add custom relay server option in RetroBat
- PCSX2 : add network option
- PCSX2 : add options to map triggers to square and cross for driving games
- PCSX2 : add option to use folder for memory cards
- NDS : enhance bezels recognition based on screen layout
- Vpinball : allow backglass when only 1 screen connected
- XEMU : add Complex 1.03 as firmware option
- Lime3DS & CITRA : write rom path in the emulator settings
- MAME : add more cases of autoboot by reading hash files
- RPCS3 : add input/output options
- RPCS3 : add rumble feature
- 3DS : add .m3u file to be able to run installed apps
- XENIA-CANARY :  add framelimit feature
- add .m3u support for amigacdtv and pc98
- add .xbox360 extension to XENIA (same ways of working as .m3u)
- DOLPHIN : add option to run wii menu
- DOLPHIN : add lightgun specific per-game setting based on gamesdb.xml
- DOLPHIN-TRIFORCE : map test menu to R3 instead of L3+R3
- CEMU : add missing vsync options
- lr-flycast : add naomi2 default mapping per game
- Xenia-canary : add feature to turn on "apply patches"
- Add preconfigured nvmem files for Flycast
- Xenia : Add Xenia Manager to the RetroBat store ==> only this version will work well with RetroBat
- Mednafen : add hotkeys/shortcuts

### Other stuff:
- Add some logs here and there
- Add 4 types of bezels (default-curved, non-curved and night versions)
- Add xbrz-5X retroarch shader choice from Retrobat
- Cleaning of old XEMU code (ini file management)
- Emulators will now propose update if available when ran from RetroBat menu
- Retroarch : if no hotkey is set, hotkey actions will not be mapped by default
- Add custom relay server option in netplay settings
- Added controller tattoos (only for gb, gbc, gba, nds, 3ds, nes, snes, n64, gamecube, gamegear, mastersystem, megadrive, saturn, dreamcast, psp, ps1, ps2, pcengine, pcenginecd, supergrafx, pcfx, 3do, jaguar & jaguarcd for now)
- Align all NES emulators controller configuration to the same layout per default and same layout options
- Align all SNES emulators controller configuration to the same layout per default and same layout options
- Align all Megadrive/Genesis emulators controller configuration to the same layout per default and same layout options
- Align all Dreamcast emulators controller configuration to the same layout per default and same layout options
- Align all Gamecube emulators controller configuration to the same layout per default and same layout options
- Align all Mastersystem emulators controller configuration to the same layout per default and same layout options
- Align all N64 emulators controller configuration to the same layout per default
- Align all Saturn emulators controller configuration to the same layout per default and same layout options
- Align all gamegear emulators controller configuration to the same layout per default
- Align all GBA emulators controller configuration to the same layout per default
- Align all Gameboy & Gameboy color emulators controller configuration to the same layout per default
- Align all nintendo DS emulators controller configuration to the same layout per default
- Align all 3DS emulators controller configuration to the same layout per default
- Align all PCEngine, PCEngineCD, SuperGrafx and PC-FX emulators controller configuration to the same layout per default
- Align all 3DO emulators controller configuration to the same layout per default
- Align all Jaguar & jaguarCD emulators controller configuration to the same layout per default
</details>

## RetroBat 6.3
<details>

### Emulators\cores:
- Update Hypseus SINGE and include FrameworkKimmy for latest games
- Add OpenGOAL (Jak and Daxter 1 and 2 engine)
- Add Caprice Forever for AMSTRAD CPC & GX4000
- PPSSPP standalone is now the default for PSP
- Bump MAME to 0.267b
- Bump Retroarch to 1.19.1
- Bump Raine to 0.96.9
- Bump RPCS3 to 0.0.32-16617
- Bump Mednafen to 1.32.1
- Bump Vita3K to 0.2.0.3615
- Bump Play! to 0.65
- Bump Duckstation to 0.1.6937.0
- Bump PCSX2 to 2.0.2
- Bump Dolphin to 2407
- Bump Mupen64 (RMG) to 0.6.5
- Bump Xenia & Xenia-Canary
- Bump Flycast to 2.3.2-157

### Fixes:
- Fix potential null pointer in libretro guns autoconfiguration
- Fix EKA2L1 controller index assignment
- XEMU : change closing hotkey to send CLOSE instead of taskkill : this should fix saves corruption issue
- Lime3ds : add new executable name
- PC-ENGINE : default to 2-button pad
- libretro-Mupen64 : force vulkan when using parallel plugin
- Few fixes of default settings values for libretro cores
- RPCS3 : fix features for new version
- MEDNAFEN : fix psx & saturn controller error
- VPinball : fix -extminimized and -ini command lines not being passed to command line for new RC versions of VPinball
- Dolphin : change exit combo to send CLOSE instead of KILL - might fix wiimote disconnection issues some people had
- MAME & FBNEO : if game is vertical and no specific bezel is set, RetroBat will default to vertical arcade bezel
- CAP32 : fix running dedicated COMMAND from .m3u file by deactivating autorun when a command is present
- WINDOWS : .gameexe file to specify process to monitor does now work for any .lnk file

### Features:
- 3ds : Add bezels for side-by-side layout (also added capability to search for nds, but no bezel is yet available)
- Libretro nes cores : add palette options
- BigPEmu : set SDL as default input driver
- Citra & Lime3DS : enable bezels
- DOLPHIN: Add Retroachievements support (Gamecube & Wii)
- Duckstation: add new shaders
- HYPSEUS: management of .singe folders
- JGenesis: Add nes zapper option
- LR-FCEUMM & LR-MESEN: add turbo and core aspect ratio features
- LR-FCEUMM: fix overscan option
- Ryujinx : add option to force number of controllers that will be configured, this can avoid the gamepad screen to popup in Ryujinx (by default Retrobat was configuring as many players as the number of connected controllers)
- Ryujinx : add network features
- SINGE2: update ways of searching for .singe file and videofile
- XEMU : add option to select cerbios flashrom (needs 'Cerbios.bin' in retrobat\bios folder)
- NEC PC98 : add .cue extension
- RAINE : add features & controller autoconfiguration
- DOLPHIN : add aspect ratio setting for wii in sysconf
- Play! : added few missing features
- FBNEO : add games to autoconfiguration of controllers
- PCSX2 : add per game memory card option
- PCSX2 : add .m3u support (RetroBat will launch the file specified in first line of .m3u file)
- Add squashfs support to some emulators (dolphin, citra, lime3ds, duckstation, bigpemu, ppsspp)
- Add Retroarch turbo feature to few cores
- MODEL 3 : add option to use L1 and R1 for racing games instead of triggers for people with arcade cabinets without triggers
- CEMU : add button mapping to display Gamepad screen
- PCSX2 and PSX : add option to change controller mapping and use L2 and R2 for driving games (useful for Gran Turismo)
- SIMPLE64 : add selection of controller pak
- XENIA & XENIA-CANARY : add some features and fixed a few that have changed with xenia update
- FLYCAST : add network features in RetroBat menu

### Other stuff:
- Add animated bezels for RetroArch (only on few systems)
- Add Retroshooters guns detection
- Add MAME nvram preconfigured files
- Add TEKNOPARROT lightgun games in lightgun collection
- Add lowresNX scrapping capability (screenscraper)
- French translations rework
</details>

## RetroBat 6.2.1
<details>

### Emulators\cores:
- Add SINGE2 emulator for Daphne & ActionMax (SINGE games)
- Jgenesis : use -cli executable instead of -gui
- Updates : duckstation, Jgenesis

### Fixes:
- Fix "object reference not set to an instance of an object" error
- Fix missing 'reminiscence' and 'devilutionx' rom folders
- Fix RetroArch 'video_swap_interval' default value (was 1 instead of 0)
- Delete ps3.keys (was assigning R1 button to middle mouse)
- Fix TI99/4a information (year + name)
- Fix duckstation internal postprocessing filter options
- Fix PCSX2 mouse cursor (enable the option to set crosshairs to NONE)
- Fix missing END in hypinput.ini
- Fix .png extension for pico8 with retroarch

### Features:
- Renaming and reorganization of features for Mednafen
- Citra/Lime3DS : Add screen layouts + texture filter feature
- Add -outputs=win command line option to supermodel (for mamehooker)
- FBNEO : add on option to use alternative gamepad indexes if a dolphinbar is connected
- FBNEO : if controls mapping is not found for a rom in fbneo.yml, search the parent rom
- DUCKSTATION : add option to force BIOS to use
- BIGPEMU : add controller autoconfiguration (based on dinput)
- SUPERMODEL : add possibility to run in borderless window instead of fullscreen (can be useful for lightgun games)

### Other:
- Add casio loopy to screenscraper
- Maj WIKI (teknoparrot + new features)
- Align shortcut for MESEN & Ares to take screenshots to hotkey + R3
- Updated WIKI for symbian games
- Align hotkey + R3 for screenshots in some emulators
</details>

## RetroBat 6.2
<details>

### Emulators\cores:
- Add sudachi & suyu support
- Add Lime3ds support for 3ds
- Add DevolitionX (diablo engine)
- Add Sonic 3 AIR, sonic-mania and sonic retro (Sonic, Sonic 2 and Sonic CD) engines
- Add pocketCDG libretro core for Karaoke system (needs mp3 + CDG files)
- Add VC4000 system (MAME)
- Add casio loopy (MAME) (requires bios casloopy.zip)
- Add Aamber pegasus (MAME) (requires bios pegasus.zip)
- Update flycast to v2.3
- Update Ares to version 137
- Add Demul for cave system
- Add symbian games for EKA2L1 (games in .sis format need to be installed first in emulator
- Add reminiscence (flashback port) - necessitates game files
- Add Mesen for Master System, PC-Engine and Supergrafx
- Add jgenesis multi-emulator (nes, snes, gb, gbc, mastersystem, gamegear, megadrive, segacd)
- Update BigPemu, Cemu, Flycast & RPCS3

### Fixes:
- Disable "rewind" feature with ppsspp libretro core ==> the feature is incompatible and was generating black screen on many games
- Fix libretro-ppsspp language feature
- Fix FPinball features
- Fix Cemu and Ryujinx autoconfig for new XBOX controllers with updated firmware
- Fix Mame64 controller index autoconfiguration
- Fix openBor custom version exit error message
- Fix Mame2016 corrupted cheat.zip file
- Fix Dolphin borderless fullscreen being always overwritten
- Update MAME hash files with 0.264 files
- Fix citra controllers autoconfiguration
- Add option to disable controller auto-configuration to demul-old
- Switch : fix handheld mode
- lr-opera : fix BIOS selection
- lr-swanstation : fix ratio setting
- libretro-fbneo : fix overclock feature
- MAME : do not delete default.cfg anymore
- Fix keyboard auto-configuration for Mesen standalone
- RPCS3 : align features with latest version from 04/05/2024

### Features:
- lr-citra : add "virtual SD card" and option to disable hardware renderer
- lr-ppsspp : remove deprecated features
- Add Chihiro CXBX features
- Add pad2key to VPinball
- RPCS3 add option to force SDL driver for Xinput controllers
- Add shaders to Ares
- Cemu : Add option to use XInput api for XInput controllers
- Add ports options for MAME/MESS computers (mostly joysticks)
- Add new games to FBNEO standalone autoconfiguration (still many to add !)
- Add possibility to create a .gameexe file next to a windows shortcut (in windows games) to specify the game executable RetroBat should check before returning to ES
- Add possibility to create a .uwp file next to a windows shortcut to precise the name of the UWP App that is launched with the shortcut and let RetroBat find the right executable to monitor
- Add custom resolutions to ryujinx (0.5 and 0.Cool
- MESS systems : Add ability to add a boot command in a .autorun file (must be placed near the game rom file with the same name)
- DOLPHIN : add option to disable Gamecube controller when using real wiimotes (fixes control issues for games such as Goldeneye 007)
- MAME: add -output option (windows or network)
- Add choice of device for EKA2L1
- OpenBOR : add possibility to run specific versions that have a different executable name than openbor.exe
- PSXMAME - add analog to dpad option
- Add .zip and .7z extensions to BigPEMu, Bizhawk, Dolphin, Duckstation, Jynx, Mednafen and PPSSPP
- Add features to libretro pce, pcecd and pcfx cores (6-button pad + disable sprite limit)
- Add Retroachievements to Flycast standalone
- Add video driver option for BigPEmu

### Other:
- Enable disk spanning for installer
- Add option to install dependencies in RetroBat installer
</details>

## RetroBat 6.1
<details>

### Emulators/cores/systems:
- Add Othello multivision (with gearsystem)
- Add nokia ngage with eka2l1
- Add PSXMame for ZINC games
- Add Ikemen-GO
- Add gemRB engine (open-source implementation of Infinity Engine for Baldur's Gate type games)
- Add standalone fbneo emulator for fbneo system
- Add ability to run custom OpenBOR build (using rom filename & specific core option) : configuration is NOT automated with custom versions
- VPinball : compatibility with version 10.8
- Update Supermodel version
- Magic Engine can now be downloaded from RetroBat (you still need to purchase a key to get full functionality, RetroBat does not provide it)
- Bump RetroArch to 1.17

### Features:
- [WHEELS] First implementation : model2, model3, pcsx2, flycast (dreamcast) (currently supported wheels : Logitech G29 and experimental: G920, driving force GT and G923, Thrustmaster T300RS (gearstik only in model2 and model3))
- [CONTROLS] Magic Engine controllers autoconfiguration
- [CONTROLS] Add xinput driver option for MAME autoconfiguration with correct joystick orders
- [CONTROLS] Add logic to search per-game MAME cfg files first in saves\mame\ctrlr then in bios\mame\ctrlr when using "per-game" controller profile option
- [CONTROLS] Add option to use left analog joystick instead of dpad in SNES9X
- [CONTROLS] Add option to disable MOUSE in libretro:mame
- [CONTROLS] Dolphin : add management of Gamecube adapters from Raphnet and Mayflash (you need to connect gc pads in reverse order on mayflash (4 for player 1, etc.)
- [CONTROLS] Add autoconfiguration of N64 controller from Nintendo online shop for Ares, Bizhawk, Simple64 and Rosalie's Mupen64
- [CONTROLS] Add autoconfiguration of N64 adapters from Raphnet & Mayflash for Ares, Bizhawk, Retroarch, Simple64 and Rosalie's Mupen64
- [CONTROLS] Cemu : add wiimote horizontal controller profile
- [CONTROLS] Add gun option to libretro mame, mame2003_plus and mame2016 cores
- [CONTROLS] Enable raw input driver in Retroarch if use_gun is set and multiple gun devices are connected
- [CONTROLS] RetroArch & Flycast standalone: add individual game controller configuration for all arcade games and ability for user to manage through a file                   WIKI
- [CONTROLS] Add profile for lightgun for wii games with dolphin
- [FEATURES] MAME : add setting skip_warnings to 1 in ui.ini file
- [FEATURES] Add desktop resolution option to Teknopparot and Demul
- [FEATURES] Add .chd extension for PSP system
- [FEATURES] Add libretro-desmume features
- [FEATURES] Add .chd extension to amigacdtv
- [FEATURES] Add ability to run gemdos hdd images with hatarib core (using m3u and .GEM file)
- [FEATURES] Add crosshair feature for model2
- [FEATURES] Add 2 features in Vita3K emulator
- [FEATURES] Add Technicolor shader in RetroArch
- [FEATURES] Add features fo fbalpha, mame non-current cores.
- [FEATURES] Add "-output windows" option for MAME standalone (used for mamehooks)
- [FEATURES] Future Pinball : added camera type feature
- [FEATURES] Supermodel : add supersampling (needs a beefy gpu !)
- [FEATURES] Vita3k : enhancement with pref-path management, if setting your own emulator content path, RetroBat will use it, else it will use the emulator path
- [FEATURES] Retroarch : add support for new mitm-session argument (netplay)
- [FEATURES] Flycast (standalone) add option to use R1 and L1 instead of triggers
- [UPDATES] Update bios\PPSSPP assets for libretro-PPSSPP core
- [UPDATES] Update BIOS lookup and bios selection for PCSX2 (both standalone & libretro core) : bios must be placed in bios\pcsx2\bios and the list has changed
- [UPDATES] Update BIOS lookup for psx bios (default RetroBat is now psxonpsp660.bin)
- [UPDATES] Remove unnecessary file formats for MUGEN system

### Fixes:
- fix some features not correctly working in libretro ppsspp (e.g. anisotropic filtering)
- fix exit of chihiro / cxbx
- Vpinball & fpinball : fix .zip management
- fix screenshots being deleted on game exit
- fix controllers not autoconfigured with new versions of ryujinx & CEMU (ensure GUID calculation can match SDL 2.30 version with manufacturer name)
- Fix dolphin savestates combo with non-xinput controllers
- Fix MAME exit combo
- Fix model2 exit combo not saving NVRAM
- Fix supracan md5 bios check
- Fix mono-gun games in retroarch settings when multiple guns are connected
- disable teknoparrot update search when running from RetroBat
- Fix bios checking engine that did not work when the path contains twice /bios
- Remove obsolete aspect ratios for mame standalone (as these are only used in -window mode)
- Fix screen size for hypseus on high-resolution displays
- Fix shaders when using OpenGL driver on libretro cores that force glcore (use slang shader instead of glsl for these cores), also added ability to specify different glsl and slang shaders for a single RetroBat preset
- Fix PPSSPP standalone autoconfiguration of controllers for non-xinput devices (attention, PPSSPP has a bug that prevents non-Xinput controllers to work when a XInput controller is connected)
- Fix zinc start failing if controller does not have a required button
- cemu : allow gamepad button inversion also for non-xinput controllers
- Remove default colorization of GameBoy games with libretro:gambatte
- Fix launch of Dolphin Triforce emulator from RetroBat menu not working
- Fix one feature value not available anymore in new Ryujinx Avalonia UI
- Fix pcsx2 cheats path that had too many subpaths ('cheats\pcsx2\cheats\cheats' now is 'cheats\pcsx2\cheats')
- Fix XEMU not launching in fullscreen in some cases
- fix duplicate features naming (e.g. beetle_psx_hw video renderer)
- Fix retroarch 'custom' aspect ratio not applying
- Fix Mednafen standalone controller configuration (emulator is using dinput)
- Remove unnecessary extensions for MUGEN
- Vita3k no detection of .m3u file in some cases

### Interface:
- Fix issue of disconnection of gamepad in RetroBat interface when trying to affect controllers to users and having multiple controllers of the same type
- Fix network icon not being removed when choosing the option to hide it
- Fix display of gametime when duration is between 24 and 25 hours

### Dev stuff:
- Add method to get new SDL 2.30 guid value (with CRC) (still in progress, not fully functional)
- disable check for sinden FilterGraphWindow (camera activity) when searching for connected SindenLightguns
- Move core/system specific remaps to remap files instead of retroarch global mapping
- Add method to be able to manage in future game-specific options in scummvm (disabled for now)

### Project:
- New retrobat notice document
</details>

## RetroBat 6
<details>

### Dev stuff:
- Move RetroBat repositories to the project official github : https://github.com/RetroBat-Official ==> you can now create issues and we will follow and answer
- Move to new Screenscraper api and increase scraping speed
- Improve eboot.bin search in .ps3 folders
- Move RPCS3 controller configuration to SDL instead of WinMM
- Search amigaforever in Program Files directory if not found in retrobat\emulators folder
- Simplification of running steam games, no need for batch files anymore
- Add management of Microsoft gamepass games (needs a small trick to work)
- New RetroBat installer
- Prepare class for wheel detection (for future)
- Remove usage of .cmd file for ZaccariaPinball and PinballFX3 - now fully managed via EmulatorLauncher
- Prepare functionality to manage savestates for more standalone emulators (for future)
- Update Reshade
- code cleaning & refactoring
- New logo

### Fixes:
- Fix Retroachievements error
- Fix controller injection in supermodel and yuzu
- Fix hotkeys injection for pcsx2, dolphin, duckstation and mesen
- Fix camputers lynx autoboot command not working for libretro:mame (has been removed, command must be typed manually, refer to wiki)
- Fix features not appearing for some MESS systems
- Alignment of hotkeys for some emulators (refer to wiki)
- Fix Gamecube controller mapping for wii games supporting GC controller
- Fix using "Guide" button (PS on playstation controllers, Xbox button or Home on NINTENDO) as hotkey on rpcs3, pcsx2 and duckstation
- Fix CEMU & Dolphin vsync feature
- Citra & xemu : fix screenshotpath
- Fix Handheld mode on yuzu
- Fix some controller mapping on Dolphin
- Fix px68k cpu speed feature
- fix beetle_psx analog/digital switch messing with hotkey
- Fix fbneo neogeo_mode value injection
- Fix Retroarch hard sync option
- Fix pcsx2 & duckstation when playing with more than 4 players with only xinput controllers
- Fix libretro:mame autodetection of vertical games
- Tentative to fix XInput controllers order
- Aligned tos folder between libretro:hatari and hatari
- Fix Teknoparrot regression with newer TP version (gameprofiles issue)
- Fix crashes happening with incorrect bezel image
- Fix emulator download issue when emulator folder does not exist

### Interface:
- Many fixes (memory leaks, crashes, performance issues) : overall the fluidity and performance of the interface should increase
- Add new views in EmulationStation interface and ability to use post-processing shaders in themes (included already some effects in Carbon theme)
- Add possibility to use video splashscreen in EmulationStation
- Fix missing "hardware" tag for Switch console
- Fix year tag for WiiU was 2010 instead of 2012)
- Clean up bios check for numerous systems
- Aligned names for some features

### Guns:
- Fix gun support in multiple emulators (PCSX2, RPCS3, Flycast, Duckstation, SuperModel) & libretro:cores
- Added menu to manage gun options
- Add detection of Gun4IR guns in RetroBat
- Fix sinden lightgun border when width has decimals
- Add crosshair option to pcsx_rearmed


### New emulators / cores :
- Add Ares & Bizhawk for multiple systems
- Add Mupen64 (Rosalie's) and Simple64 standalone emulators (n64 and n64dd)
- Add Flycast (Dreamcast, naomi & Atomiswave)
- Add melonDS standalone (NDS)
- Add citra-canary (3DS)
- Add Namco 2x6 with Play emulator (also added on PS2)
- Add Zinc (Arcade)
- Add SSF (Saturn)
- Add Stella
- Add ruffle (flash)
- Add HBMame standalone (homebrew arcade)
- Add ZEsarUX (ZX Spectrum)
- Add arduous (arduboy)
- Add uzem (uzebox)
- Add libretro MelonDS DS
- Add lowresNX
- Add jynx (Camputers lynx)
- Add hatari standalone (atariST)
- Add Magic Engine (PCEngine & SuperGrafx)
- Add pcsx2 libretro core support
- Add libretro:hatarib core
- Add PinballFX, Pinball M & PinballFX2 support (steam versions & standalone)
- Add libretro:dinothawr
- Add libretro:xRick (Rick Dangerous)
- Add libretro:openlara (Tomb Raider port)
- Add gong libretro port
- Add fake08 (PICO8)
- Add Super Bros War (libretro port of Super Mario War)
- Add vitaquake2
- Add ecwolf (Wolfenstein 3D)
- Add libretro:boom3 (Doom 3)
- Add eduke32
- Add GZDoom
- Add The Force Engine (Dark Forces)
- Add SEGA S-TV with libretro:kronos
- Remove 4DO core

### Core system scope increases:
- MAME64 for AppleII & AppleIIGS system (additional BIOS required)
- Add mgba for gb, gbc and sgbAdd libretro:sameboy core for gb and gbc, allowing multiplayer with different cartridges (e.g. pokemon)
- Add mednafen for wswan, saturn, psx, lynx, gb, gba, sgb, ngp, ngpc, gamegear, pcfx and mastersystem
- Add mesen to snes, gb, gbc and sgb
- Add libretro:sameboy core for gb and gbc, allowing multiplayer with different cartridges (e.g. pokemon)

### Core/emulator updates:
- Update RetroArch to 1.16 (including core updates)
- Update most standalone emulators to newer versions (BigPEmu, Dolphin, Dolphin-Triforce, Cemu, Citra, CXBX, Xemu, Xenia, PCSX2, Duckstation, RPCS3, Vita3K, PPSSPP, mGBA, Mesen, Hypseus, Mame64, Future Pinball, VPinball, SNES9x, OpenMSX, ScummVM, ...)

### Features:
- Add Mega-bezels : sonkun, cyberlab, Duimon updated & koko-aio
- Add audio features to dolphin
- Add Apple2 controller type for MAME
- Add deekay palette to vice cores
- Add multi-disc (2 discs) management to AppleIIGS and apple2
- Add features for snes9x
- Add preemptive frames feature for supported cores
- Add RPCS3 features (CPU Blit, trophies, guns)
- Add features to PCSX2 : start in PS2 bios, choice of USB port for guncon
- Move xenia and xenia-canary saves folder to retrobat\saves\xbox360 folder
- Add .zip extension to psp (libretro)
- Add .woz extension for apple2gs & apple2
- Add dolphin post-processing filter option
- Add bezels and shader for solarus, redream, raine, mednafen
- Add additional TATE mode to FBNEO and TATE mode to libretro:mame
- Add features to PinballFX3 (nb of players, classic mode)
- Yuzu: add ASTC recompression feature & controller applet deactivation & option to disable fully retrobat settings injection
- Dolphin: add vertex rounding feature
- libretro_mednafen_psx_hw : add overclock feature
- mednafen standalone controller autoconfiguration & features
- Add MAME standalone controller configuration
- mesen controller autoconfiguration
- Demul controller autoconfiguration
- SNES9X controller autoconfiguration
- Hypseus controller autoconfiguration
- Kega-Fusion controller autoconfiguration
- Phoenix controller autoconfiguration
- Add redream features + controller autoconfiguration
- Add controller type choice to ryujinx (joycon, handheld, pro controller…)
- Controller autoconfiguration for CXBX
- PPSSPP standalone emulator controller autoconfiguration
- Add reshade to duckstation
- Add shader "sindenborder" for standalone controllers using reshade
- Add controller button inversion features for dolphin (core & standalone)
- Add features for m2emulator
- libretro:mame - add padtokey buttons to access to mame menu and to service menu
- Add automation of high scores for libretro:mame and mame64
- Add .prg extension for C64
- Add Xenia features for Forza Motorsport 4
- Add bezels to Xemu
- Add Duimon MBZ shaders to Bigpemu
- Add possibility to run dsi nand (.bin) files with MelonDS (multiple nand images can be managed)
- Add retroarch video filters
- Add retroachievements to PPSSPP standalone
- Add motion to simulate Wii movements for controllers with motion (Dualshock / Switch Pro)
- Add .ipf file support for AMIGA (you need to add the "capsimg.dll" file)
- Added management of .url game shortcuts for EPIC Game Launcher and Amazon Launcher (meaning RetroBat will find out the executable name and wait for it to close)
- Add savestates management in interface for some standalone emulators (dolphin, pcsx2, ppsspp, duckstation)
- Add some libretro hatari & hatarib features
- Add PGXP feature for compatible psx cores/emulators
- Use MAME bezels for FBNEO when mame bezel-project is installed
</details>

## RetroBat 5.3
<details>

### Fixes:
– Fix ryujinx feature injection
– Fix mame standalone ratio not working (disable keepaspectratio when ratio forced in features)
– Fix artwork path for mame standalone to align with libretro:mame path
– Fix bezels for libretro:dolphin wii system and put libretro:dolphin in 16/9 aspect ratio by default (for wii only)
– Fix BigPemu template to avoid error message when running jaguarcd titles for the first time
– Fix FBNEO hardcore retroachievements mode by disabling « allow-patched-roms » when hardcore is enabled
– Fix dolphin gamepad button inversion missing for X and Y (only A & B were reversed)
– Fix once and for all pcsx2 multiple screen…(cross-fingers)
– Fix use of Gamecube adapter for dolphin standalone
– Fix missing features for demul-old (user for gaelco)
– set default settings in retrobat.ini in case of invalid or null value
– Align dolphin HD texture pack with libretro:dolphin, this means the custom texture packs must be placed in \saves\gamecube\User\Load\Textures
– Fix libretro:mame per-game button remap naming
– Fix usage of .uae files for WinUAE
– Align Citra-QT sdmc and nand path with libretro:citra path
– Fix Bios check for atomiswave
– Fix vita3k vsync feature
– Fix missing CXBX language feature (same as XEMU)
– Fix missing .m3u extension for Sega-CD

### Interface:
– fix canonball system in ES system list (avoid duplicating « Ports » category)
– Fix game video in grid mode too small when in gamelist
– Fix HFSDB scraping delay issue
– Fix music volume issue after screensaver when volume set to 0
– Rename « Game focus » feature to « Keyboard focus » and make it available only for computer cores
– smooth transition from splashscreen to the interface
– Add preview images in RetroBat download store
– Hide console when running MAME and Ryujinx

### Updates of emulators\cores:
– Bump duckstation (and addition of RetroAchievements)
– Add mgba for gb, gbc and sgb
– Add WinUAE also for amigacdtv
– Bump libretro:ppsspp
– Bump libretro:vice_xpet
– Bump ppsspp emulator
– Add OpenMSX for MSX & colecovision (with support of SGM roms for colecovision and MSX laserdiscs)
– Add Zaccaria Pinball (steam only)

### New misc stuff:
– Add MSX turbo R system in MSX group
– Add GP32 to MESS systems
– Add gun support (1 player only) for pcsx2 and duckstation – compatible with guns that emulate mouse (e.g. wiimotes)
– Add features for BBC Micro to select Joystick type (mame & libretro:mame)
– Add features for TI99 (speech module and 32k ram) (mame & libretro:mame)
– Add possibility for FmTowns to load a floppy in addition to a cdrom
– Add ramsize feature for fmtowns (mame & libretro:mame)
– Add -multimouse command line feature for mame standalone
– Add option to play with more than 2 players in nosgba (3 and 4 players)
– Added values injected in rpcs3 (exit emulator when game finishes + prevent display sleep when playing)
– Add archimedes bios check & missing models
– Add StOoz zone & disable fullscreen features to Teknoparrot
– Actionmax is now a separate system (not integrated with Daphne anymore)
– Add feature to enable discord integration (for compatible systems)
– Add automatic controller configuration mechanism in RetroBat interface if controller is known in SDL database (NOTE! ==> this will delete your personal controller configuration in RetroBat)
– Add mgba features
– Add features to ryujinx and yuzu (docked mode, language…)
– Add language feature to RPCS3
– Add touchscreen pointer option for libretro:citra
– Add padtokey to mugen
– Add m3u multi-disk support to GSPlus (Apple2GS)

### Dev stuff:
– RetroBat.exe cleanup and enhancements
– Cleanup es_padtokey file
– Refactorization of yuzu options injection
– Review of language detection for some standalone emulators
– Changed method of searching EBOOT.BIN file for ps3 games
</details>

## RetroBat 5.2
<details>

### Fixes:
- Fixed A and B (south and east) button inversion when configuring a controller in EmulationStation
- Fixed OpenBOR controls injection
- Fix .tzx extension for ZXSpectrum (was incorrectly set in es_systems file)
- Fix duckstation memcards path setting (path was duplicated)
- Fix Retroarch device type injection using remaps (might consequently fix some device type injection for RetroArch cores)
- Fix snes9x features (audio interpolation values were wrong)
- Fix yuzu renderer selection (was always forced to vulkan)
- Fix yuzu motion not working
- Fix XEMU dvd_path issue for newer versions
- Fix RetroAchievements popups not displaying in first beta version
- Fix monitor index / bezels for pcsx2-QT (tentative, might not be completely solved yet)
- Fix missing 'disableautocontrollers' option for Supermodel (model3)
- Removed non-working .zip & .7z extensions from gba2players system
- Fix NEOCD default BIOS (CD-Z instead of UNIVERSE BIOS), improves load speed
- Fix cemu controllers (added feature to select controller type for player 1 and 2 as some games accept only 1 gamepad and some others require only pro controllers), also added options to use Real Wiimotes (with dolphinbar)

### Additional cores, emulators, systems:
- jaguarCD with BigPEmu
- Commodore PET (vice_xpet)
- Commodore CPlus/4 (vice_xplus4)
- Cannonball (outrun libretro port)
- wasm-4 (fantasy console)
- Atari XE Game System (mame - mess)
- Coleco Adam (mame- mess)
- Acorn Archimedes (mame - mess)
- Acrorn ATOM (mame - mess)
- emuscv core for scv system
- NO$GBA for GBA system
- libretro:parallel_n64 added to n64dd system (compatible with .ndd full NDD games only, not extensions)
- bump mame to 0.253
- bump rpcs3
- bump scummvm (standalone & core)

### Features:
- Add features for following emulators : nosgba, RPCS3, PCSX2 (resolutions & precaching of custom textures), Teknoparrot, xemu, yuzu, dolphin-triforce, dolphin, xenia (language), scummvm, cemu (controllers), mame standalone, bigpemu
- Add features for following cores : pokemini, picodrive, ppsspp, prosystem, puae, potator, bsnes & bsnes_hd_beta, quasi88, prboom, px68k, craft, swanstation, mrboom, stella & stella2014, same_cdi, sameduck, RACE, 81, vecx, TGBDual, vice (all vice cores), tyrquake, desmume, melonds, opera, 4do, a5200, pcsx_rearmed, parallel_n64, mgba, atari800, crocoDS, citra, caprice32, bluemsx, desmume, desmume 2015, dosbox-pure, handy, mame2003
- Added selection of softlist, media type and machine type for MESS systems (in libretro:mame and mame64)
- Add feature in Yuzu, Ryujinx to invert face buttons to match XboX controller layout
- Add custom textures feature for citra
- Add option to rotate screen in FinalBurn cores and flycast (TATE mode)
- Add option to select controller type in multiple cores (advanced settings>controls)

### Miscellaneous:
- Dolphin Load/ResourcePacks paths moved to \bios\dolphin-emu instead of \emulators\dolphin\user
- Inject hotkeys in pcsx2 & dolphin emulators
- Controllers injection : better detection of controller index through activation of SDL HINTs
- Added extensions : .chd (fmtowns), .hdf (AMIGA systems), .rpk (ti99), .dsk (coco), .nib (c64)
- Daphne : no need to use Windows Developer mode anymore for Hypseus
- Triforce : removed constant update check for those wanting to try latest triforce emulator
- BIOS check: bump ps3 bios check to 4.90 version, added Color Computer bioses, added apple2gs bios
- Add RETROBAT identification to default ambiance decorations pictures (bezels)
- Updated RetroArch recordings folder to \retrobat\records
- Improved bezel search logic (for game-specific bezels)
- Updated systems logos in RetroBat system menu
- New feature : turbo button (on FCEUMM core only for now)
- MESS system grouping review
- Correction of platforms in es_systems.cfg
- add guns option to mesen core
- New "cheats" folder for cheats (used for RetroArch and PCSX2) : \retrobat\cheats
- Bump to dokan2 for XBOX iso mount
- new pcsx2-qt.exe compatibility (for these who want to upgrade to latest nightly pcsx2.exe)
- Added retroachievements sound customization
</details>

## RetroBat 5.1.1
<details>

### Fixes:
– PinballFX3 generator now launching directly tables
– Fix crash when 2 identical controllers were connected
– Fix cps1 and cps2 features mix-up
– Fix unability to quit some emulators with HOTKEY + START because of game focus option automatically set to on
– Fixed rpcs3 joystick axis inversion for XInput and Dualshocks
– Fixed yuzu controller configuration to add possibility to choose joystick type
– Fix some shaders not working with model2
– fix RetroBat not displaying on second monitor issue
– fix missing PCSX2 feature “skip bios”
– fix ES navigation in vertical mode (L1 / R1 usage)

### Additions:
– possibility to run pcsx2 in bigpicture mode
– add cycle_exact feature for winuae
– add actionmax support to daphne/Hypseus
– add language selection for Wii

### Miscelleneous:
– Some cleaning of unused code and typo errors corrections
– Removed libretro:redream from Dreamcast emulators list
– Removed no$GBA from GBA system
</details>

## RetroBat 5.1
<details>

### New system:
– PS Vita

### New features:
– Xenia / Xenia-Canary (Xbox 360) (including controllers database for controller management)
– Commodore 64
– cemu (WiiU)
– Swanstation (psx)
– Supermodel (model3)
– Dosbox
– yuzu (switch)
– ryujinx (switch)
– picodrive (Sega)
– citra (3DS)
– dolphin (gamecube/Wii)
– demul (Sega Arcade)
– ScummVM
– Retroachievements on cap32 (Amstrad)
– Retroachievements on PS2 (with PCSX2-QT)
– Add Game Focus feature for keyboard systems (disables RetroArch hotkeys to prevent interference with game control)
– Add service menu feature for atomiswave (flycast core)
– Better handling of controls for fuse core (ZXSpectrum)
– Roland mt-32 now added to DosBox

### Cores:
– same_cdi
– Update prosystem core (atari 7800)

### Standalone:
– Vita3K
– PCSX2 updated to QT version
– Phoenix for 3DO & Jaguar
– BigPEmu for Jaguar
– Oricutron reworked for RetroBat
– Applewin reworked for RetroBat

### Miscellaneous:
– updated BIOS checks (neoCD, same_cdi, scummvm (audio))
– mame core usage for oric/atmos
– Controller autoconfiguration for Dolphin, Yuzu, Ryujinx, RPCS3, Supermodel, Citra & PCSX2-QT
– Addition of bezels & shaders with reshade for some standalone emulators (model2, Supermodel, BigPEmu, oricutron, daphne/Hypseus, Applewin, OpenBor, Mednafen, Simcoupe, GSPlus, ScummVM, Demul, Phoenix)
– Bump SDL to 2.26 and major rework on the way controllers are handled (for better autoconfiguration in future releases)
– New JSON library methods for better handling systems using json configuration file
– scummvm (standalone + libretro) and DosBox pure now accessible from RetroBat menu
– Correction & additions of mega-bezels
– Multiple fixes:
– pcsx2 paths
– mesen fullscreen start
– demul dreamcast game loading
– m3u usage for dolphin standalone
– 7zip games now working for netplay & retroachievements
– Retroachievements sign for grouped systems in EmulationStation
– FMTowns scraping
– Xenia download & licence_mask fix
– keyboard A & B inversion fix
</details>

## RetroBat 5
<details>

### New systems:
– Adventure Vision
– amiga 4000
– apfm1000
– Arcadia 2001
– Astrocade
– BBC micro
– Camputers Lynx
– Philips CD-I
– Color Computer
– CreatiVision
– FM 7
– Gamate
– Game.com
– Game Pocket Computer
– GameBoy Advance 2 players
– Game Master
– LCD Games
– Megadrive-msu
– Mega-Duck
– Neo-Geo 64
– PV-1000
– Super Cassette Vision
– Super Game Boy
– Super A’Can
– TI-99
– Tomy Tutor
– TV Games
– VSmile

### New features:
– New Retrobat integrated Updater & Emulators download/update functionnality
– New content downloader
– Add incremental savestate support
– Add support for lightguns and Wiimote Guns, new lightgun games collection and removal of «*lightgun*» rom folder
– Sinden Lightgun support
– Duimon’s Mega-Bezel pack support
– Support of zipped roms decompression
– Add image viewer to Retrobat
– Autodetection of best mame version when set to auto
– XInput drivers for libretro
– Add: support for Retroachievements “Challenge” indicator

### Cores:
– a5200
– fbalpha (current)
– fceumm
– gearcoleco
– imageviewer
– mame2000
– mame2010
– swanstation

### Standalone:
– 3DSen (emulator not provided)
– Hypseus (fork of Daphne)
– no$gba (gba 2 players)
– pcsx2 1.7 SSE4 and AVX2 versions
– pcsx2 1.6 version moved to pcsx2-16 folder (pcsx2 folder used for 1.7 version)
– PinballFX3 (through Steam integration)
– ScummVM
– Yuzu early access

### Miscellenaous:
– moved all bioses to \bios folder and updated bios list md5 checks
– Add new music theme
– New version of Batgui.exe (not all functionalities have been ported yet)
– Group system features into submenus in Retrobat advanced configuration menu
– Option to invert A and B buttons
– Removed arcade system, replaced with individual system folders
– 64dd folder renamed n64dd
– New SDL version
– Additional features directly accessible from Retrobat to avoid setting
up the features in the emulators (PS3, PS2, Yuzu, scummvm, dolphin, ….
and many others)
– New Website
– New Wiki
</details>

## RetroBat 4.0.2
<details>

- fix missing logo for Nintendo 64DD in Carbon Theme
- fix Supermodel.ini for Supermodel emulator (Model3) to use proper mapping for controllers
- fix MAME standalone binary mispelling
- add missing script to enable update detection
- Add mame2016 Libretro core for Arcade systems
- Add bsnes Libretro core for Sufami and GameBoy systems
- Update BatGui
- Bump RetroArch to v1.9.6
- Update Libretro cores
- Update Duckstation
- Update Cemu
- Update RPCS3
</details>

## RetroBat 4.0
<details>

### New Supported Systems:
- Apple II gs (Gsplus).
- FM-Towns (Tsugaru & MAME64).
- Oric Atmos (Oricutron).
- Sharp X1 (Retroarch).
- EasyRPG (Retroarch).
- Tyrquake (Retroarch).
- Tic80. (Retroarch).
- Teknoparrot.
- Flash Player. (Thanks to AureyoBoss)
- Löve.
- Pico8 (retro8 et pico8).
- Add Supervision (Retroarch).
- Add Channel-F (Retroarch).

### New Features:
- Add a Gui 'BatGui' to facilitate the use of Retrobat.ini + other features. Thank to Reppa.
- Redefining Controls
- Random intro video.
- Launch RetroBat automatically when Windows starts.
- Activate / Deactivate controllers autoconfiguration be by system and not only globally.
- Model2 / Model3: Reshader management (Supermodel & Model2emu).
- Model2 / Model3: Add support for bezels (Supermodel & Model2emu).
- Dolphin: Add support for bezels (Standalone).
- FM-Towns: Add support for bezels (Tsugaru).
- AppleII gs: Add support for bezels (Gsplus).
- PS2: Add support for bezels. (PCSX2 Standalone).
- Neo.Geo CD: Add support for shaders (Raine).
- Neo.Geo: Add support for shaders (Raine).
- New Save State "Slot" system integration in ES (Retroarch).
- Automatic language detection for EmulationStation and Retroarch.
- Add new options for NETPLAY.
- Add background music. (*.mp3 & *.ogg)
- Add DuckStation (Standalone) (Playstation)
- Add Kodi multimedia Player.
- Add Kega-Fusion emulator (Standalone)
- Add MAME64 standalone.
- Add support for RyujinX (Standalone) (Switch)
- Add WINUAE standalone. (Amiga)
- Add Dosbox Pure core (DOS) (Retroarch)
- Add MESEN emulator (nes)
- Add RetroAchievment integration
- Add PADTOKEY function (A kind of Xpadder / JoyToKey integrated into ES)
- Add XEMU emulator (Xbox)
- Add a user manual directly accessible from Retrobat (ES)
- New integrated RetroBat update system
 
### New settings options on EmulationStation for:
Cores :
   atari800
   citra (3ds)
   dosbox pure (dos)
   flycast (dreamcast, naomi, atomiswave)
   gambatte (gameboy, gameboy color)
   genesis plus gx (master system, megadrive, megacd)
   genesis plus gx wide(screen) (master system, megadrive, megacd, 32x)
   mame
   mame2003 plus
   mednafen psx hw (ps1)
   pcsx rearmed (ps1)
   mednafen saturn (saturn)
   mesen (nes)
   mupen64plus (n64)
   pcsx rearmed (ps1)
   potator (supervision)
   ppsspp (psp)
   picodrive (master system, megadrive, megacd, 32x)
   snes9x (super nes, super nes msu 1)
   fbneo (arcade, neogeo, neogeo cd)
   kronos (saturn)
   puae (amiga)

Standalone :
   raine (neogeo, neogeo cd)
   pcsx2 (ps2)
   dolphin (gamecube, wii, wad)
   fpinball
   vpinball
   openbor
   duckstation (ps1)
   daphne (laserdisc)
   supermodel (model3)

### Misc:
- Standalone emulators updated.
- Bump to RetroArch 1.9.5
- The roms folder "n3ds" is now "3ds"
- The "Model2" games must be in the "roms\model2" folder and not "roms\model2\roms"
- Yuzu: Auto-fullscreen re-works on new versions of Yuzu.
- Dolphin Standalone: Added missing buttons on auto-config (L & R).
- Add support for ".ps3" files like on Batocera (experimental).
- Cave Story: Add support for *.exe extension (Retroarch).
- Several minor fixes.
</details>

## RetroBat 3.1
<details>

Compared to the latest stable release (RetroBat v2.1) :
- 100+ supported consoles, handheld, arcade and computers systems.
- RetroBat use Batocera ES build for Windows instead of EmulationStation FCAMOD.
- A new setup GUI to download, install and configure EmulationStation, RetroArch and the standalone emulators.
- Bump to RetroArch 1.8.9 SDL 2.0.12, compatibility with RetroArch ANGLE.
- retrobat.exe: a new launcher for ES and a manager of the global settings (replace retro.bat scripts).
- emulatorLauncher.exe: an advanced emulators launcher allowing integration of their features and options into the EmulationStation menu: RetroArch, RetroArch Angle, AppleWin, Cemu, Cxbx-Reloaded, Daphne, Demul, Dolphin, Dolphin WX, DOSBox, Future Pinball, M2Emulator, Mednafen, mGBA, OpenBor, PCSX2, PPSSPP, RPCS3, SimCoupé, Solarus, Supermodel and Visual Pinball are concerned.
- Configure your controllers in EmulationStation and they will also be configured for all the emulators managed by emulatorLauncher. Close emulators easily with hotkeys.
- Change video modes, screen ratio, decorations, shaders and more directly from the ES menu. You can apply this globally, per systems or per games.
</details>

## RetroBat 2.1
<details>

- RetroBat is now compatible with 64 bit AND 32 bit Windows x86 computers.
- Bump RetroArch to 1.8.4.
- Hotkeys are enabled in RetroArch configuration.
- Added compatibility with Kodi.
- Added compatibility with many standalone emulators: m2emulator (Model 2), cemu (Wii U), citra (3DS), Future Pinball, Mednafen (nes, snes, megadrive, pcengine, pcenginecd, playstation), mGBA (Game Boy Advance), Raine (Neo Geo CD), snes9x (Super NES) and Visual Pinball.
- Added launchers for Visual Pinball and Future Pinball to make them portable (by Fabrice Caruso).
- Added runcommand.exe module instead of batch scripts to launch emulators from RetroBat config menu in EmulationStation. Emulators command parameters can be modified in runcommand.ini. Runcommand.exe can read m3u files to launch Wii U and PS3 games.
- Added compatibility with Theodore libretro core (Thomson computers) and Kronos (Saturn).
- Added compatibility with Megadrive Steam Uncompressed ROMS with .68K extension.
- Some bugs fixes.
</details>

## RetroBat 2
<details>

- Scripts were rewritten from scratch for more efficiency.
- RetroBat Setup detect if EmulationStation, RetroArch, Libretro Cores and 7-Zip are installed and install  them automatically if needed.
- RetroBat Launcher detect if setup directory has changed and run RetroBat Setup to fix it.
- Install and update software separately.
- Install and update themes for EmulationStation.
- RetroBat Scripts can be updated in RetroBat Setup.
- Debug options.
- Launch video as introduction before EmulationStation. Use emulationstation.exe --video (vlc) instead of ffmpeg core.
- Read settings from emulationstation.cfg to set ES resolution fullscreen or windowed.
- Enable JoyToKey in emulationstation.cfg.
- Enable video intro in emulationstation.cfg.
- Add launcher for OpenBOR and RPCS3 (thank to Fabrice Caruso).
- Add in ES systems list: OpenBOR, MUGEN, PS3, Apple II, Famicom Disk System and SG-1000.
- Fixed some issues and bugs.
</details>
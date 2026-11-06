# retrobat padtokey override

This directory can be used to store your own PadToKey profiles (controller buttons sending keyboard keys or mouse actions).
Profiles created or edited for a system in EmulationStation (CREATE / EDIT PADTOKEY PROFILE) are saved here.

File names:
- <system>.keys          => profile for a whole system, for example amiga500.keys
- <system>.<core>.keys   => profile for one core / emulator of a system only, for example amiga500.puae.keys

Profiles for a single game are saved next to the game, in the roms\<system> folder:
- <game>.keys            => for example roms\amiga500\Turrican.keys
- padto.keys             => inside the folder of a game that is a folder

RetroBat uses the first profile found, in this order:
1. the game profile (roms\<system>\<game>.keys)
2. user\padtokey\<system>.<core>.keys, then user\padtokey\<system>.keys
3. emulationstation\.emulationstation\padtokey (same names)
4. system\padtokey (same names)

Original files are located in system\padtokey.
Original files are overwritten with each RetroBat update,
files located here will not be updated.
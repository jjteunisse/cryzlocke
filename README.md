# About
The **Cryzlocke** project aims to realise multiplayer Nuzlocke runs for Pokémon Crystal. In order to do so, users run a Lua back-end which is coupled with a collective web front-end.

The project is currently in its (very) early stages, and is based upon our succesful application of this concept to Pokémon Emerald ("MP Nuzlocke"). These previous efforts are being kept private, for now.

# Setup
This section explains how to set up the project.

## Player steps
1. Download the latest VBA-RR release from [here](https://github.com/TASEmulators/vba-rerecording/releases). The version we used at the time of writing is 
`VBA-rr-svn480.LRC4-xp140.7z`.
1. Retrieve a Pokémon Crystal ROM from your preferred source. This is a grey area, we won't tell you where to get it exactly.
1. Run the VBA-RR executable and open the Pokémon Crystal ROM. Afterwards, navigate to _Tools > Lua Scripting > New Lua Script Window... > Browse..._ and open `/src/cryzlocke.lua`. Afterwards, press Run and you're good to go.

## Developer steps
1. To enable local testing, download the latest Lua 5.1 release from [here](https://luabinaries.sourceforge.net/download.html). The version we used at the time of writing is `lua-5.1.5_Win64_bin.zip`. VBA-RR explicitly uses Lua 5.1 rather than newer versions, so we're using it as well to avoid conflicts.
1. The project expects the Lua release to be placed under `/bin/lua/` and the VBA-RR release to be placed under `/vba/`. Among others, this excludes the files from source control.
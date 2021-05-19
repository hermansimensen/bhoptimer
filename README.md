[![Discord server](https://discordapp.com/api/guilds/389675819959844865/widget.png?style=shield)](https://discord.gg/jyA9q5k)

# !!! THIS IS A DEVELOPMENT VERSION, USE AT OWN RISK !!!
### If you're to use this DEV BRANCH, make sure to recompile all of the other external plugins you're using alongside bhoptimer with the newest includes from this version (scripting/include/shavit.inc). Otherwise you might (or will) end up getting your console spammed with errors and plugins being partially not functional or not working at all.

### Build status
[![Build status](https://travis-ci.org/shavitush/bhoptimer.svg?branch=master)](https://travis-ci.org/shavitush/bhoptimer)

[AlliedModders thread](https://forums.alliedmods.net/showthread.php?t=265456)

[Download](https://github.com/shavitush/bhoptimer/releases)

# shavit's bhop timer

This is (nearly) an all-in-one server plugin for Counter-Strike: Source, Counter-Strike: Global Offensive, and Team Fortress 2 that adds a timer system and many other utilities, so you can install it and run a proper bunnyhop server.

Includes a records system, map zones (start/end marks etc), bonuses, HUD with useful information, chat processor, miscellaneous such as weapon commands/spawn point generator, bots that replay the best records of the map, sounds, statistics, segmented running, a fair & competitive rankings system and more!

[Mapzones Setup Demonstration](https://youtu.be/OXFMGm40F6c)

# Requirements:
* Steam version of Counter-Strike: Source, Counter-Strike: Global Offensive, or Team Fortress 2.
* [Metamod:Source](https://www.sourcemm.net/downloads.php?branch=stable) and [SourceMod 1.10 or above](https://www.sourcemod.net/downloads.php?branch=stable) installed.
* A MySQL database (preferably locally hosted) if your database is likely to grow big, or if you want to use the rankings plugin. MySQL server version of 5.5.5 or above (MariaDB equivalent works too) is highly recommended.
* [DHooks](https://github.com/peace-maker/DHooks2/releases)

# Optional requirements, for the best experience:
* [eventqueuefix](https://github.com/hermansimensen/eventqueue-fix)
  * Some booster fixing and scaling booster delays by timescale. (Use this instead of `boosterfix`)
* [Bunnyhop Statistics](https://forums.alliedmods.net/showthread.php?t=286135)
  * Used for scroll styles and also required for TF2.
* [SteamWorks](https://forums.alliedmods.net/showthread.php?t=229556)
  * Used to grab `{serverip}` in advertisements.
* [DynamicChannels](https://github.com/Vauff/DynamicChannels)

#  Installation:
Refer to the [wiki page](https://github.com/shavitush/bhoptimer/wiki/1.-Installation-(from-source)).

# Required plugins:
`shavit-core` - completely required.  
`shavit-zones` - completely required.  
`shavit-wr` - required for `shavit-stats`, `shavit-replay`, `shavit-rankings` and `shavit-sounds`.

# Recommended plugins:
* [MomSurfFix](https://forums.alliedmods.net/showthread.php?p=2680743) ([github](https://github.com/GAMMACASE/MomSurfFix))
  - Makes surf ramps less likely to stop players. (Ramp bug / surf glitch)
* [RNGFix](https://forums.alliedmods.net/showthread.php?t=310825) ([github](https://github.com/jason-e/rngfix))
  - Makes slopes, teleporters, and more less random. Replaces `slopefix`
* [Showtriggers](https://forums.alliedmods.net/showthread.php?t=290356) ([github](https://github.com/1ci/showtriggers))
  - Allows players to toggle trigger visibility.
* [ShowPlayerClips](https://forums.alliedmods.net/showthread.php?p=2661942) ([github](https://github.com/GAMMACASE/ShowPlayerClips))
  - Allows players to toggle player clip visibility.
* [shavit-mapchooser](https://github.com/mbhound/shavit-mapchooser)
  - Fancy map chooser plugin to add some timer specific options for the nominate and rtv menus.
* [shavit-ssj](https://github.com/Nairdaa/shavit-ssj)
  - Speed of Sixth Jump + more, customisable settings with cookies remembering user prefered settings.
* [shavit-jhud](https://github.com/blankbhop/jhud)
  - Jump HUD for bhoptimer. !jhud for settings.
* [shavit-firstjumptick](https://github.com/Nairdaa/bhoptimer-firstjumptick)
  - Displays what tick the player first jumps at upon leaving the startzone. Very useful for strafe maps, where you tryhard to cut that tick or two. !fjt to enable.

* TODO: `paint`, `mpbhops`, `ljstats`, `bash2`
### CS:GO
* [NoViewPunch](https://github.com/hermansimensen/NoViewPunch)
  - Removes the viewpunch from landing in CS:GO.

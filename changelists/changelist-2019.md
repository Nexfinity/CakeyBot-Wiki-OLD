# Changelist - 2019

## 12/31/2019

#### Fixed

* Fixed an issue where queue wouldn't show the current playing song if items were in the queue

#### Added

* Added playlist/queue saving! You can now save everything in your queue and load it up at a later point!
  *  Usage: `!playlist <save | load | delete> <name>`
  * This feature will allow you to have a playlist of songs from multiple sources, rather than ONLY YouTube or ONLY Bandcamp.

## 12/30/2019 - DJ Role Support

#### Changed

* AFK messages can now be deleted by clicking a trashcan emoji
  * This only removes the message that the bot sends, it doesn't unset the user from AFK
  * If Cakey Bot doesn't have the correct permissions for this feature, AFK messages will show as they did before
* `!slowmode` now accepts human readable times \(i.e. 1h5min3s\)
* `!clearqueue`, `!remove` and `!playskip` now require Server Moderator permission / DJ Role

#### Added

* Support for "DJ" role instead of Server Moderator permissions on music commands
* Added Cakey Bot's definition of a "Server Moderator" to the [FAQ](../setup/faq.md#what-is-considered-a-server-moderator).

## 12/28/2019 - Soundcloud Support Added

#### Changed

* Updated how roles are parsed in commands \(You can now use ANY one of these three things for role input: ID, Name, Mention\). Affects the following commands/features:

  * Self Roles command
  * Role Info command
  * Role Management module

  Note:  `!setting autorole` & `!setting muterole` commands still require you to ping/mention the role

#### **Added**

* Re-Added video thumbnails to `!np` command
* Added localization to Audit Log module
* Added Soundcloud support to music
* Added Direct URL MP3 file support to music

## 12/26/2019 - Bandcamp Support Added

#### Changed

* Updated usage info for `!remove`
* Improved string censor to prevent false censoring \(i.e. on words like "canal"\)

#### Added

* Bandcamp support added for music
* Vimeo support added for music
* Mixer support added for music
* Added a `!clearqueue` command \(Aliases: `!cq`, `!clqueue`, `!emptyqueue`\)
* Added a plural check to the global warnings in `!userinfo`
* Added `!slowmode <time> <opt:channel>` command - Updates slowmode for the provided channel \(if not provided, it uses the channel the command was ran in\)
* Added `!role <add | remove> <user> <role>` command - Adds or removes a role from someone
* Released Emoji Management module. \(Incomplete\)

## 12/24/2019 - Command Info Overhaul

#### Fixed

*  Fixed an issue in `!cmdhelp` where null values could mess up formatting
* `!dc` now functions again while a song is playing

#### Changed

*  Reduced `!purge` rate limit \(30s =&gt; 7s\)
* `!userinfo` now shows global warning count for a user

#### Added

* Added `!suggest` as alias for `!suggestion`
* Added module name to `!cmdhelp`
* Added command usage to `!cmdhelp`
* Added command usage info for every command
* Added command aliases to `!cmdhelp`
* Added `!sban` as alias for `!softban`
* Added `!faq` and `!assistance` as alias for `!help`
* Added the ability to pass a command name into the `!help` command to get info similarly to `!cmdhelp`

## 12/23/2019 - Bulk Message Delete Support

#### Fixed

* Fixed an issue where muting a user could fail due to role positions
* Fixed missing player in `!play` command
* Misc. Bug Fixes

#### Changed

* Better handling and less null issues when moving the bot between different channels
*  Improved error handling for `!lyrics` command when no lyrics are found

#### Added

* Added BulkMessageDelete to audit log

## 12/18/2019

#### Fixed

* Fixed several typos in the music module, all the updates recently made me overlook some stuff
* Misc. Bug Fixes

#### Added

* Many more strings added to localization \(Still plenty to do like core module and audit log, but it's getting there\)

## 12/16/2019 - Music Improvements

#### Fixed

* Cakey Bot should now also automatically resume when a discord shard disconnects
* Overall music quality should be better and have less stuttering

#### Changed

* `!dc` now allows disconnects if no song is currently playing if multiple users are in the VC
* Improved error messages when a music track fails to load

#### Added

* Added sentry.io logging to lavalink to help me identify errors with music quicker
* Added sentry.io logging to Victoria to help with the above logging
* `!leavecleanup` command. You can now remove items from the queue if users are no longer in the voice channel.
* `!playtop` is now an alias for `!playskip`

## 12/15/2019 - Music Looping

#### Fixed

* Several other bugs that came up on sentry.io
* Multiple music issues were resolved and several typos/incorrect titles were fixed. `!np` command now has more info
* Fixed an issue where the `!move` command caused the player to disconnect
* Fixed an issue where AutoSummon and `!move` could cause incorrect errors to be thrown after bot restarts

#### Changed

* Made `!s` and alias of `!skip` instead of `!search` \(This seems to be the more common expectation of that alias\)
* Improved join/move behavior of the bot overall \(Weird unexpected behavior could cause the bot to be disconnected or moved and this wasn't handled properly previously\)
* Cakey Bot no longer self-deafens when joining voice channels

#### Added

* Song Requested is now shown on the `!np` and `!queue` commands
* Users are now able to force-skip the currently playing if they are the ones who added it, regardless of current vote skips or lack of moderator permissions
* You can now loop your favorite songs with `!loop`!


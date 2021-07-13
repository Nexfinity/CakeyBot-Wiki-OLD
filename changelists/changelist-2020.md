# Changelist - 2020

## 12/29/2020

#### Added

* Released more [Advanced Placeholders](../setup/placeholders-variables.md#advanced-placeholders):
  * Released `{require:}` placeholders - You can now specify specific channels/users where a command can be used.
  * Released `{not:x}` placeholders - You can now specify specific channels/users where a command can not be used.

## 12/28/2020

### Added

* Released more [Advanced Placeholders](../setup/placeholders-variables.md#advanced-placeholders):
  * `{deleteafter:x}` - Delete the response after X amount of seconds. Replace the x with a number between 1 and 9.
  * `{confirmdelete}` - Add a trashcan reaction to the response that deletes it after it is clicked. \(Similar to AFK messages\)
  * `{respond:#channel}` - The channel that the command will send the response to

## 12/27/2020 - Slash Commands!

### Added

* Released new slash commands:
  * /b64decode
  * /b64encode
  * /video
  * /wiki
  * /coinflip
  * /ping
  * /setting
  * /help
  * /invite
  * /docs
  * /dashboard
  * /debug
  * /prefix
* Added new "Flag" type to auto responder. The new flag `Contains Files` will trigger auto responder if any messages contains files \(i.e. documents, images, videos, etc\)

## 12/25/2020 - User Gateway Screening

### Changed

* Cakey Bot will now wait until users pass Discord's new gateway screening before adding the Auto Role.
  * This will prevent users from completely bypassing it

### Fixed

* "View Usage" & "Placeholder Reference" both open in new tabs now
* Auto Responder now correctly pre-fills the "Flags" field
* Implemented a patch to fix the high latency on Shard \#4

## 12/22/2020 - V3 Website Design

### Changed

* A new website design! It now matches the new web dashboard and designed to look a bit cleaner. This is the first step and I will be greatly overhauling the design and layout to match the new theme as time goes on. This initial update was just to match the styling to that of the web dashboard.
* Updated Korean and Swedish translations

### Added

* Added first "[Advanced Placeholder](../setup/placeholders-variables.md#advanced-placeholders)": `{delete}`

## 12/19/2020 - Among Us Gif

### Changed

* Improved how Cakey Bot interacts with external APIs. This should lower the number of problems & will now send an error message when a problem occurs instead of just silently failing.
  * Note: It takes a few seconds to actually load/generate.

### Added

* Added new `!amongus [user]` command. ;\)

## 12/14/2020 - Automatic Dehoist

### Fixed

* Fixed the "Channel" for auto mod violations in audit log messages.
* Fixed a translation error in the `!8ball` command.
* Fixed literal boat load of bugs ;\)

### Changed

* Modified the default word blacklist in auto mod for less false positives and reduced default number of blacklisted words.
* Reverted some changes that broke `!tempmute`, `!tempban` & `!reminder`.

### Added

* Added "Auto Dehoist" to auto mod. Works just like `!dehoist` but applies automatically when a user joins the server or changes their nickname.

## 12/9/2020 - Image Analysis

### Fixed

* Fixed an issue where "Logs" on the web dashboard would not sort correctly on initial load

### Added

* Added new `!requests` command. Displays all songs in the queue that you have requested.
* Added new `!analyzeimage` command. Analyzes the image and tags common objects in it.
* Added the ability to set the verification role on the web dashboard.

### Removed

* Removed ability to toggle modules using the `!setting` command.

## 12/8/2020 - Auto Mod Release

### Added

* Released Auto Mod publicly again after fixing some critical bugs
* Added two new Text Manipulation commands! They are `!bold <text>` and `!boldscript <text>`

## 11/27/2020 - Improved AFK Statuses

### Changed

* Updated `!afk` command so that running `!afk none` will remove your AFK status.

### Added

* Added option to disable users setting `!afk` statuses per-server _\[Web Dashboard\]_
* Added option to set a max AFK time limit. _\[Web Dashboard\]_
  * By default, AFK statuses will be permanent until the user or an admin removes the status
  * You can set a max time limit between 1 minute and 1 week, after which the AFK status will be disabled automatically for users.

## 11/26/2020 - Music Queue Update

### Fixed

* Fixed `!musicsetup` command
* Misc. Bug Fixes

### Changed

* Improved auto mod to check for new bypasses _\[BETA Feature\]_
* `!userinfo` command embed color now matches the highest colored role of the user \(or default bot color if none\)
* Updated documentation to match new dashboard layout/settings

### Added

* Music Queue
  * Cakey Bot will now display/sync the current music queue on the web dashboard!

## 11/18/2020

### Changed

* \#feedback channel on the [Support Discord](https://discord.gg/Y3VdQAD) has been renamed to \#suggestions \(Use `!suggestion <title> | <description>` to post suggestions now and use \#support for bug reports.\)

### Removed

* Removed `!feedback` command. Bot now directs people to use the [Support Discord](https://discord.gg/Y3VdQAD).

## 11/14/2020

### Changed

* Auto Mod has now been relocked to BETA testers due to it clearly not being release ready.

## 11/12/2020 - BETA Program Returns

### Fixed

* Fixed an issue where Cakey Bot may lag/reconnect when bulk deleting messages
* Fixed an issue where some users could not properly authenticate to the new dashboard
* Fixed a bug where Github Previewer would show even when disabled
* Fixed a bug where Auto Mod would not work even when enabled

### Changed

* Disabled prefix/language caching for now

### Added

* Started up Cakey Bot BETA Testing program again
* Added `BETA`, `WIP` \(Work-In-Progress\), and `New` badges to the navigation sidebar of the panel.
  * WIP are non-BETA features that are currently in development. They may be buggy or incomplete. \(Similar to BETA features but do not require BETA access\)
* Added toggle for generic web URL check on web dashboard

## 11/11/2020

### Fixed

* Fixed a bug where Auto Mod wouldn't work on most servers
* Fixed multiple issues with Github Previewer
* Fixed an issue where some songs would fail to play/skip
* Misc. Bug Fixes
* Updated Auto Quoter to only work on links/URLs from the server they are copied from

### Added

* Added `!yoink` as alias for `!grab`
* Added underscores to `!dehoist`
* Started work for auto-resume on music when shards reconnect \(1/2\)
* _\[Internal\] Added ability to toggle 'Limited Mode' during major outages in the core_

## 11/6/2020 - Github Code Preview

### Added

* Added Github Code Previewer

## 11/5/2020 - Message Auto Quoter

### Fixed

* Fixed an issue where server data was not syncing with the database correctly \(This caused incorrect server icons and member counts for the web dashboard\)
* Implemented a patch to prevent duplicate custom commands/auto responders
* Misc. bug fixes \(Including fixing music\)

### Added

* Added Auto Quoter \(You can toggle this via the web dashboard\)

## 11/2/2020 - Dashboard V2 Update

### Added

* Responsive Design \(MUCH better tablet/phone support\)
* Localization support \(Change panel language\)
* Fullscreen toggle
* Improved/cleaner UI design \(looks nicer overall, including animated icons \) 
* Ability to edit custom commands/auto responders
* Enabled the ability to configure auto mod settings

### Changed

* Instant data refresh \(no more needed to manually refresh pages to see your changes\)
* Improved feedback/notifications/errors \(You now get a fancy pop up when you make changes or encounter issues\)
* Improved tables \(They are now paginated, sortable and can be searched!\) \(They also load much faster\)
* Improved security \(Won't go into details here\)
* Faster load times 
* Confirmation dialogs for sensitive actions and hover tooltips for various actions

### Planned

* Light Mode addition
* More features overall \(Basically all the stuff that's been sitting on the "planned" list due to lack of a decent dashboard\)
* This new dashboard is much cleaner and easier for me to code on. Which means I can add new stuff quickly and easily
* Updating main website to match dashboard UI
* Live data-sync between bot/website \(i.e. view music queue on website or send embeds from the dashboard\)

## 10/23/2020

### Fixed

* Tons of bug fixes \(like literally a ton\)
* Fixed error message for purge when there are no valid messages to delete
* **Fixed music, seems it may have been broken for a day or two**

### Changed

* Improved the results of the `!gif` command
* Updated acceptable time format for `!giveaway` command, works just like `!reminder` now

## 10/18/2020

### Fixed

* Fixed \[join \| leave \| ban\] arguments being case-sensitive on the announcements command
* Fixed an error message in the announcement command where it wasn't auto-filling the custom prefix

### Changed

* Updated how roleplay commands mention users \(This should fix the invalid mentions for mobile users\)

### Added

* Added another fallback for user avatars \(Affects many core components of the bot where user avatars are used\)

## 10/5/2020 - More Audit Logs

### Fixed

* Fixed Join/Leave announcements \(They will now work with [Basic Placeholders](../setup/placeholders-variables.md#basic-placeholders) as intended\)
* Improved voice channel join checks \(Now checks for user limit AND permissions\)

### Added

* New [audit log](../tools-and-utilities/audit-log.md#audit-events)[ events](../tools-and-utilities/audit-log.md#audit-events)!
  * Invite Created
  * Invite Deleted
  * User Joined/Left/Swapped voice channels

## 9/29/2020 - Image Manipulation Update

### Fixed

* Fixed formatting issue on all Roleplay commands.
* Fixed `!invert` Command
* Fixed `!greyscale` Command
* Fixed moderation commands not working on some users in large servers

### Changed

* Updated `!fact` Command - **New Usages:**
  * `!fact` - Displays a random fact that you probably didn't know.
  * `!fact [dog | cat | panda | fox | bird | koala | kangaroo | raccoon | elephant | giraffe | whale]` - Displays an animal-specific fact.

### Added

* Added `!pokedex <pokemon>` Command - Displays info about the provided Pokemon.
* Added `!meme` Command - Displays a random meme!
* Added `!whale` Command - Displays an image of a random whale!
* Added `!raccoon` Command - Displays an image of a random raccoon!
* Added `!kangaroo` Command - Displays an image of a random kangaroo!
* Added `!facepalm` Command - Displays a facepalm gif.
* Added `!wink <user>` Command - Wink at someone ;\)
* Added donation information to `!about`, `!help`, & `!vote` commands.
* Added `!blurple` Command - Tints the given image blue/purple.
* Added `!brightness` Command - Brightens the provided image.
* Added `!threshold` Command - Makes the image absolute black and white.
* Added `!sepia` Command - Makes the given image sepia colored.
* Added `!red` Command - Tints the given image red.
* Added `!green` Command - Tints the given image green.
* Added `!blue` Command - Tints the given image blue.
* Added `!pixelate` Command - Pixelates the given image.
* Added `!blur` Command - Blurs the given image.
* Added `!triggered` Command - Makes a triggered gif from the provided image.
* Added `!rainbow` Command - Makes the provided image rainbowfied.
* Added `!glass` Command - Puts a glass overlay over the provided image.
* Added `!wasted` Command - Makes the provided image into a GTA-styled wasted screen.
* Added `!ytcomment <text>` Command - Generates a fake YouTube comment with the provided text.
* Added `!moviedb` Command - Pulls movie information from The Open Movie Database.

## 9/28/2020 - The Movie Update

### Fixed

* Role, Channel and User mention placeholders should now work properly in Custom Commands/Auto Responder

### Added

* Added `!imdb <query>` Command - Pulls various information from IMDb.
* Added `!trailer <query>` Command - Gets a TV/Movie trailer from IMDb for the provided query.

## 9/25/2020 - The Animal Update

### Fixed

* Fixed several issues with Music Embeds
* Fixed an issue where `!covid` sometimes didn't send a response due to rate limits

### Added

* Added error message for Overflows on the `!math` command
* Added `!uptime` Command - Displays the current uptime of Cakey Bot
* Added `!bing` Command - Searches Bing for the given query
* Added `!bgg` Command - Gets info about the specified board game
* Added `!fox` Command - Displays an image of a random fox
* Added `!panda` Command - Displays an image of a random panda
* Added `!redpanda` Command - Displays an image of a random red panda
* Added `!koala` Command - Displays an image of a random koala
* Added `!pikachu` Command - Displays an image of a random Pikachu!

## 9/23/2020 - The Anime Update

### Added

* Added `!anime <name>` command
* Added `!manga <name>` command

## 9/20/2020

### Fixed

* Fixed join/leave/ban announcements sending when set to "none" \(They will now no longer send as intended\)
* Removed `!rank` as alias for `!role` \(Conflicts with too many other bots\)

## 9/19/2020

### Fixed

* Fixed music embed message
* Fixed `!musicsetup` command

## 9/16/2020

### Fixed

* Added an error message when Cakey Bot fails to create or find a suitable mute role on `!mute` & `!tempmute` commands
* Improved error handling/null values for Custom Commands and Auto Responder
* Fixed minor bugs with Music Embed and `!purge` command
* Improved error handling for `!play` and `!playskip` commands
* Disabled checking for custom commands in DMs
* Patched commands not sending when Discord fails to trigger "Typing" events

## 9/2/2020

### Added

* Added new `!grab` command to send the currently playing song's info to your DMs. \(Great way to save a good song for later\)

## 8/30/2020

### Changed

* Updated trivia timeout \(10s =&gt; 15s\)
* Trivia errors and timeout will now show the correct answer

## 8/27/2020 - The Trivia Update

### Fixed

* Fixed an issue where `!purge` wouldn't upload message log to pastebin
* Updated `!persistentrole` to actually add/remove the role when making it persistent

### Changed

* Exclude deafened people from voteskip counts

### Added

* Added new `!discrim <value>` command that will give you a list of users that have the same discriminator
* Added new `!trivia` minigame command with over 400 questions! \(More coming soon ;\) \)
* Added video url to song request channel queue list
* Added Bitchute as source for music core
* Added experimental support for Twitch VODs/Clips
* Added support for more Direct Web URL files! \(.OGG, .FLAC, & .WAV\)

## 8/26/2020 - Improved Auto Responder

### Changed

* Custom Commands & Auto Responders are now separate and have their own pages on the panel.
* The layout and options for the tables and command creation popups have updated slightly to reflect these changes
* Both Custom Commands & Auto Responder are grouped on the "Auto Responder" module, so if you toggle that module, you'll toggle both of these

### Added

* Auto Responder now has the ability to set a few extra "Flags"
  * Exact Match - Default behavior, looks for exact match strings
  * Contains - Will search entire message to see if it contains this string/trigger
  * Begins With - Will check to see if the message begins with this string/trigger
  * Ends With - Will check to see if the message ends with this string/trigger
* Added placeholder support to Auto Responder & Custom Commands. You can view these [here](../setup/placeholders-variables.md#basic-placeholders).

## 8/4/2020

### Fixed

* Fixed some issues with Cakey Bot not handling permissions correctly. \(Specifically when trying to delete messages\)

### Changed

* Updated all language files

### Added

* Added uptime info to `!about` command

### Removed

* Removed support for mixer from music \(Mixer shut down July 22nd apparently\)

## 7/29/2020 - The Verification Update

### Fixed

* Fixed a bug where messages would not be properly translated for the Role Management module
* Fixed an issue where certain embeds, errors and messages were not displaying correctly. \(i.e. a success message showing up as an error\)
* Usual misc. bug fixes

### Added

* Added a new role verification command. Read more [here](../tools-and-utilities/verification-role.md).

## 6/10/2020 - The Equalizer Update

### Added

* New 14-band equalizer command for music \(`!equalizer <band> <gain>`\)
  * View current equalizer values by running the `!equalizer` command without any arguments.

## 6/3/2020

### Fixed

* Potential fix for mod commands failing in large servers
* Fixed `!purge` commands breaking with negative numbers
* Fixed an issue where Cakey Bot would still try to run a command even if Cakey Bot couldn't send messages to the given channel
* Improved handling of missing custom commands

## 6/2/2020

### Added

* Cakey Bot will now display "Cakey Bot is typing...." when a command is ran. \(Similar to normal users in discord\)

## 5/30/2020

### Fixed

* Misc. bug fixes to `!image` and music commands

## 5/21/2020

### Fixed

* Improved error handling for `!covid` command
* `!image` command will now properly display errors instead of not returning any data

## 5/15/2020

### Fixed

* Fixed some TypeReader errors which would cause commands using a user mention to not work
* Fix error handling for the `!image` command
* Fixed an error where Music Embeds would not update properly
* Fixed an issue where adding super long songs or a ton of songs to the queue would mess up queue messages due to super long play times

### Changed

* Updated the `!poll` command to not throw errors if the message is deleted while being processed
* `!image` command will now function even if _some_ data is missing \(for example a title or source url\)
* \[[Caketropolis](https://discord.com/invite/V73eTwK)-Specific\] Increased the ping detection limit in \#shard-info to 1,500ms

## 5/14/2020 - Silent Moderation

### Added

* You can now use moderator commands silently.
  * See more information [here](../tools-and-utilities/moderation.md#silent-actions).

## 4/27/2020 - Temporary Moderation

### Fixed

* Fixed `!unban` command

### Added

* Added `!tempban <user> <time> [opt:reason]` command
* Added `!tempmute <user> <time> [opt:reason]` command

## 4/24/2020

### Fixed

* Fixed `!reverse` command
* Fixed `!ping` command

## 4/20/2020

### Fixed

* Fixed `!bird` command
* Fixed `!image` command

### Changed

* Increased `!gif` command cooldown \(1s =&gt; 3s\)
* Updated error messages on roleplay commands to use embeds

## 4/17/2020

### Fixed

* Fixed an incorrect message in the music embed system

### Changed

* Update delays on commands that use reactions to prevent triggering Discord API rate limits
* Increase rate limit on `!poll` command \(1s =&gt; 15s\)
* Updated logs on website to be color coded to find specific events easier
* Enabled `Self Deafen` for music to save on bandwidth
* Increased the resume timeout for music \(10s =&gt; 60s\)
  * This should help with resuming music automatically when a shard restarts. Any feedback on whether this is working or not is appreciated as I can't force a shard to reconnect to test it manually
* Improved error handling for the `!unwarn` command

### Added

* Added support for images in `!quote` command
* Added new `{accountage}` variable for join/leave messages
* Added new `!clearwarnings` command to delete ALL warnings from a user. **\(Note: This is irreversible\)**
* Added new `!locate` command to display the current voice channel that Cakey Bot is playing music in

## 4/12/2020

### Changed

* Slightly darkened the background for the server query banner
* Increased cooldown on `!ping` command \(1s =&gt; 5s\)

## 4/10/2020 - 4/11/2020 - The Covid Update

### Fixed

* Fixed an issue where some music messages would be posted to the \#cakey\_songrequests channels 
* Fixed an issue where some commands would throw "unknown errors" when a module was disabled 
* Fixed an issue where Cakey Bot would try to check if a DM message was a "Song Request" channel 
* Fixed an issue where Cakey could failed to get a valid music track but still try to play it
* Fixed incorrect titles on some error messages
* Fixed an issue where Cakey Bot would fail to add a server to the database if the server name contained special unicode
* Fixed an issue where Cakey Bot wasn't properly syncing servers in the database

### Changed

* Updated `!togglemention` command to work if discord doesn't have a valid value set
* Updated `!setting module` to not completely break if Cakey Bot doesn't have external emoji permissions
* Updated Auto Mod warnings to self-delete after 5 seconds
* Improved error checking for disabled modules
* Prevented the ability to run commands in \#cakey\_songrequests channels
* Pushed some more translations live
* Converted all error messages to fancy embed format with same design
* Updated strings in newer commands to used localized variants

### Added

* Added the ability to use an image banner instead of custom text for join/leave announcements. More info can be found [here](../tools-and-utilities/join-leave-ban-announcements.md#image-banner-announcements).
* Added new `!covid <country>` command to keep up-to-date with the COVID-19 pandemic.
* Cakey Bot will now inform you if the the bot is missing 'required permissions' via DM when first invited to a server.

### Removed

* Removed `!blurple` command
* Removed `!gstats` command

### Other

* Cakey Bot is now an Officially Verified Discord Bot!

## 3/28/2020 - Reminders!

### Added

* Reminders
  * Maximum time limit for reminders is 1 month
  * You can not currently list/remove reminders, this functionality will be added later.
  * You can more more information and usage details [here](../tools-and-utilities/reminders.md).

## 3/19/2020 - Song Request Channel

### Fixed

* As usual fixed several misc. bugs including one that would prevent Cakey Bot from working in servers if the bot was removed and then re-invited!

### Changed

* Improved/added localization to several music strings
* Updated the "30 seconds until bot disconnect" message to self-delete if Cakey Bot has permission to do so

### Added

* Added a Song Request channel feature!
  * Control your music and view a real-time updated queue list in a dedicated music text channel!
  * Tired of using commands to add new songs? Just type your song name/url into the channel and it'll be auto-queued!
  * Prefer using commands? That's fine! If you have the music embed setup, it'll automatically update with song/queue info even if you keep using commands!
  * More information including usage and setup can be found [here](../music/song-request-channel.md).

## 3/18/2020

### Fixed

* Misc. bug fixes and QOL changes
* Fixed an issue where the website would not load "Invite Bot" pages if the bot wasn't in the selected server

### Added

* Song Request channel
  * You can view more information about this [here](../music/music-basics.md#song-request-channel).

## 3/6/2020

### Fixed

* Fixed an issue where the server logo would fail to load or would load an incorrect logo
* Fixed an issue on custom commands where using dropdown menu options would toggle/delete the very last command, not the one you're trying to update
* Fixed the `!msg <id>` command output
* Internal - Fixed an issue causing some logs to not log correctly

### Changed

* Updated the `!quote` command to be functional and useful
  * Description: Displays a quote of the given message id in the provided channel.
  * Usage: `!quote <channel> <message id>`

### Added

* Added documentation to the [custom commands](../tools-and-utilities/custom-commands.md#using-emote-emotes-in-commands) section explaining how to use emoji/emotes in them
* Added music support for Vlare.tv AND MP4 web URLs

## 2/25/2020 - Spotify Music Support

### Added

* Experimental support for spotify music added!

## 2/23/2020

### Added

* Added cooldown time for `!dehoist` \(1s =&gt; 7s\)
* Added new `!unnick` command
* Banned member messages in audit log will now display the user's last known nickname \(if one exists\)

### Fixed

* Fixed an issue where the days on `!serverinfo` would contain a really looong decimal

## 2/19/2020 - Improved Documentation

### Added

* Updated documentation regarding bot permissions, made required perms more obvious when inviting the bot for the first time
* Added localization support for Romanian!

## 2/8/2020

### Fixed

* `!banlist` will now show user discriminator, user id and overflow user count
* Misc. bug fixes

## 1/31/2020

### Fixed

* Fixed articles not showing up on `!wiki`
* Fixed multiple words not working on `!wiki`

## 1/30/2020

### Changed

* Updated translations for Turkish and Korean

## 1/27/2020

### Changed

* Anyone can now use the trashcan/delete feature on AFK messages, not just the pinger

## 1/22/2020

### Changed

* Updated `!image` command
  * SafeSearch is now disabled in NSFW text channels
  * Now uses PNG file type for more results \(Previously jpg\)
  * Can now handle results when total is &lt; 10

## 1/21/2020

### Fixed

* Fixed the `!image` command
* Fixed an issue where two commands used the same name \(`!emoji`\)
  * `!emojis` - List emojis and their ID in the server
  * `!emoji <action>` - Create, Modify and Delete emoji in the server

### Changed

* Update translations for Arabic, German, Greek, Italian, Korean, Swedish, Turkish & Dutch

## 1/20/2020 - Added Booster Info

### Fixed

* Fixed the `!wiki` command
* Fixed the `!steam` command
* Misc. bug fixes

### Added

* Added a new `!boosters` command to display a list of the users boosting the server along with the number of days they've been boosting
* Added a new `!msg <id>` command to display raw message info - useful for discord bot developers

## 1/19/2020 - The Giveaway Update

### Fixed

* Auto-Trim `!math` error messages to 200 characters to prevent spam
* Fixed a bug causing Audit User Left to not be sent
* Fixed the `!warn` command displaying the wrong target username

### Changed

* Updated `!debug` to correctly use channel permissions instead of server permissions for proper debugging
* Disabled the looping message when a song ends
* Overhauled `!debug` command to show optional and required permissions

### Added

* Delay the auto role for 10 min if the server is set to high verification
* Automatically redirect users to the docs/setup after invite
* Re-Added `!giveaway` command w/ bug fixes and corrected permission checks
* Added a permission check while adding channel overrides when creating a new mute role

## 1/18/2020

### Fixed

* Fixed `!fact` command

## 1/16/2020 - The Math Update

### Added

* Added a `!math` command. To see a list of features you can check out [this page](../other-misc/math-command.md).

## 1/14/2020

### Fixed

* Misc but fixes

### Changed

* Updated multiple languages with new translations

## 1/11/2020

### Fixed

* Fixed multiple issues/bugs with Auto Mod
* Fixed misc. bugs

### Changed

* Updated Turkish, Swedish Greek with new translations
* Converted more strings to use localization
* Released more customization options for Auto Mod

## 1/10/2020

### Changed

* Arabic, German, Italian & Korean updated with new translations

### Added

* Released Auto Mod for public testing. Limited customization.

## 1/8/2020

### Changed

* German & Korean languages updated w/ new translations

### Added

* Added multiple aliases to `!unwarn` and `!warnings`
* Started testing Auto Mod features, join our discord to help test it out!

## 1/7/2020 - Localization Improvements

### Added

* Added Italian as an available language
* Added updated translations for Greek and Swedish

## 1/6/2020 - Add Arabic Support

### Added

* Added Arabic as an available language

## 1/4/2020 - The Playlist Update

### Fixed

* Fixed role count on "User Left" audit log message

### Changed

* Updated `!rewind`, `!ff` and `!seek` to accept human readable time strings
* Prevented live streams from being saved to playlists
* Improved error checking for `!playlist` commands

### Added

* Added the ability to run the `!help` command in DMs
* Added a `!playlist list` to list all of your currently saved playlists

## 1/3/2020

### Changed

* Fixed "Requester" being displayed wrong on the `!queue` command
* Fixed an issue where `!queue` and `!np` commands wouldn't work after a song has looped
* Updated Swedish, Korean and Greek languages with new translations

### Added

* Added `!repeat` as alias for `!loop`
* Added a `!docs`/`!faq` command for direct URL to docs
* Added a `!panel`/`!dashboard` command for direct URL to web dashboard

.
# Changelist - 2022

## Sept 16th - Category Specific Channels

#### Added

* Added new Category Specific Channels!
  * YouTube URLs Only
  * Reddit URLs Only
  * Twitter URLs Only
  * GitHub URLs Only
  * Videos Only
  * Images Only
  * GIFs Only
  * Files Only
  * Emotes & Stickers Only
  * Counting Only

## Sept 22th - Music Title Blacklist

#### Fixed

* `/play` command errors now use a proper error embed rather than plain text

#### Changed

* Updated Auto Mod URL whitelist to be case-insensitive
* Updated Auto Mod URL blacklist to be case-insensitive
* Updated Auto Mod word blacklist to be case-insensitive
* Song request channel will now auto fast forward to timestamp if included in YouTube URL (Similar to `/play` command)

#### Added

* Added new Music title blacklist

## Sept 19th - Audit & music Improvements

#### Changed

* Increased Spotify album track limit from 20 to infinite on `/play` command. (For premium servers)
* Increased Spotify playlist track limit from 100 to infinite on `/play` command. (For premium servers)

#### Added

* Added sponsor block support to music (For premium servers)
* Added emoji changed to Role Modified audit log event.
* Added icon changed to Role Modified audit log event.
* Added channel overwrite changes to Channel Modified audit log event.

#### Removed

* Removed `/weather` command.

## Spet 18th - Channel Mix Filter

#### Added

* Added new `/filterpreset vibrate`
* Added new `/filter channelmix <LeftToLeft> <LeftToRight> <RightToLeft> <RightToRight>`

## Sept 16th - Verify Command Bug Fix + New Filter Presets

#### Fixed

* Fixed an issue where `/verify` would fail to respond to the command even on success
* Fixed `/filter timescale` success message showing incorrect variable names

#### Added

* Added new filters to the `/filterpreset` command
  * Chipmunk
  * Darth Vader
  * Slow Mo
  * Speed

## Sept 15th - Feed Embed Colors & New EQ Presets

#### Fixed

* Fixed not being able to set band #0 on equalizer
* Fixed equalizer success messages showing `#Zero`, `#One` for bands instead of `#0`, `#1`
* Fixed "Est. time until play" showing the incorrect time when adding tracks to the queue
* Fixed an issue where the `/filterpreset` command could be used by non-premium servers
* Fixed an issue where the `/eqpreset` command could be used by non-premium servers

#### Changed

* Descriptions for filters will now show the default value
* `/equalizer` now shows default values if no bands have been set instead of an error message

#### Added

* Added the ability to set custom embed colors on all social feeds!
* Added new presets to the `/eqpreset` command
  * Electronic
  * Soft
  * Pop
  * Ear Rape

## Sept 14th - AFK V2 + Premium Chat Bot

#### Changed

* Command prefix setting has been moved from `Bot Settings/Core` to the `Custom Commands` page since it only affects custom commands now.

#### Added

* Added a toggle to prefix user's nicknames with `[AFK]` when they are AFK
* Added a toggle to remove a user's AFK message/status when they send a message or join a VC
* Added a new AI chat bot system `[Premium-Only Feature]`

## Sept 12th - Improve Music Sources

#### Fixed

* Fixed a typo in the `/purge` command
* Re-added BassBoost preset to `/filterpreset`

#### Added

* Added music queue looping!
* Added support for Spotify albums
* Added support for YouTube Music playlists
* Added additional music artwork fallback images

## Sept 11th - Play File Support for Music

#### Fixed

* Pushed a fix where `/purge` wouldn't show a success message if audit log wasn't configured

#### Changed

* Merged `/gif <query>` into the `/search gif <query>` command to make room for the new `/playfile` command.

#### Added

* Added new `/playfile <file>` command so you can listen to tracks you have downloaded on your PC/phone!

## Sept 9th - Premium Music Updates

#### Fixed

* Fixed Premium Music Bots not working

#### Changed

* Synced missing features to the music bots:
  * Duration included in "added to queue" message
  * Added the new `/sortqueue` commands
  * Added the player action history on `/nowplaying` command
  * Added the player control buttons on `/nowplaying` command

## Sept 6th - Tags V2

#### Changed

* `/tags create <tag>` now checks if a tag exists before creating it.

#### Added

*   Tag creation and management uses a new tiered permission system!

    * Manage Own: Admins - Manage All: Admins
    * Manage Own: Mods - Manage All: Admins
    * Manage Own: Mods - Manage All: Mods
    * Manage Own: Users - Manage All: Admins
    * Manage Own: Users - Manage All: Mods
    * Manage Own: Users - Manage All: Users

    The permissions default to `Manage Own: Admins - Manage All: Admins` so that only admins can create/manage tags by default meaning you'll have to manually enable tag creation for users if you want to use tags in your server.

## Sept 6th - Music Player Action History

#### Changed

* Moved `/dehoist` command to `/dehoist all`

#### Added

* Added new "Player History" to the `/nowplaying` command!
  * This will show the last 5 events applied to the current music player and who made the actions.
* Added new `/dehoist single <user>` sub-command
* Added new `/dehoist role <role>` sub-command

## Sept 4th - Shipping QOL

#### Changed

* `/weather` command now has a country flag icon for the country
* `/ship` now has a compatibility percentage calculated
* `/ship` no longer allows you to ship yourself with yourself

## Aug 28th - Now Playing Controls

#### Added

* Added button controls to `/nowplaying`!
  * Rewind (-10s) => Play/pause
  * Fast forward (+10s)
  * Volume down (-10)
  * Toggle mute
  * Volume up (+10)
  * Loop song
  * Stop & clear queue
  * Skip song

## Aug 25th - New Audit Events

#### Added

* Added new "User Kicked" audit log event
* "User Banned" and "User Kicked" audit log events will now show which moderator kicked/banned the user as well as the reason.
  * This requires Cakey Bot to have access to Discord's Audit Logs otherwise it'll just show that the user was banned/kicked without additional info

## Aug 24th - Song Request Channel V2

#### Fixed

* Fixed song only playing for X amount of seconds before randomly disconnecting
* Fixed queue embed not showing the currently queued songs correctly/not updating
* Fixed messages sent by Cakey Bot in the song request channel not being deleted properly (including join related messages)
* Fixed songs not auto-skipping to the next one in the queue on song end if enqueued via song request channel
* Fixed a bug that allowed users to control the song request channel via reactions/buttons if they were not in the same voice channel with the bot

#### Changed

* Upgraded song request channels to buttons (instead of reactions)
  * When clicking an existing reaction or clearing all reactions on the music embed, it'll auto migrate
  * When using the `/setup songrequest` command, it'll create using the new buttons

## Aug 23th - YouTube Social Feed

#### Added

* Added new YouTube social feed notifications for new video uploads!
  * Note: Due to limitations with how infrequently YouTube's RSS feed updates, it can take UP TO 30 minutes after the video upload for Cakey Bot to "notice" the video and send the alert in Discord.

## Aug 19th - Audit Log Improvements

#### Changed

* Bulk Message deletions will now save a transcript of the bulk deleted messages
* Deleted messages that contain an image now use a more reliable method for storing the image in the log
* Updated `/purge between` so that the message ID order does not matter anymore.

## Aug 11th - Auto Mod Bug Fix

#### Fixed

* Auto Mod now actually triggers on the minimum value rather than Minimum + 1

## Aug 10th - Max Volume Increase

#### Changed

* Increased max `/volume` for music (100 => 200)

## Aug 5th - QOL Improvements

#### Changed

* The `/tag <tag>` command now makes use of Discord auto-complete system
* The `/tags edit <tag>` & `/tags delete <tag>` commands now make use of Discord auto-complete system
* Moved `/ticket createembed` command to `/setup createticketembed` (Added docs for this as well)
* Changed `/ticket createticket <opt:desc>` command to `/ticket new <opt:desc>`

## Aug 4th - Roleplay QOL

#### Fixed

* Fixed an issue where `/queue` & `/warnings` would say "failed to respond" but actually sent a response

#### Changed

* `/rp` commands will now mention the user rather than showing a plain username

## July 29th - Bug Fixes + New Command

#### Fixed

* Reasons for non-silent moderation commands will now show as expected.
* Fixed some false positives with the new phone number auto mod check.
* Fixed an issue where warning audit logs would be missing the hashtag between usernames/discriminators.
* Fixed an issue where some slash commands would be shown only to the original user and not to the entire chat
* Slash commands/interactions will now properly display in your selected language like old text commands did (if you have a non-english language set on the web dashboard for your server)

#### Changed

* Merged `/verify setup` & `/musicsetup` into a single `/setup <verifyrole | songrequest>` command.

#### Added

* Added new `/movemsg <messageId> <newChannel>` command.

#### Removed

* Removed `/pokedex` command.

## July 28th - Phone Number Auto Mod

#### Added

* Added new 'phone number' check to auto mod

## July 27th - Slash Command QOL Updates

#### Fixed

* `/purge` commands will no longer show a "failed to respond" error message
* `/purge` result messages now properly send to the log channel instead sending in the channel where the command was ran

#### Changed

* Updated `/playlist list` & `/playlist delete` so they can be used while music is not playing.
* User playlists are now global and not linked to a specific server.
* `/unwarn` will now send a DM to the user notifying them of the removal.
* Modified the parameters of `/unwarn <user> <id>` to `/unwarn <id> <opt:isSilent>`
* All moderator commands that can provide a reason now include a `isSilent` parameter instead of using the old "-s"/"-silent" method in the reason itself.
* YouTube songs will now jump to the specified time if the URL contains a `?t=453` timestamp.

#### Added

* Added a new `/remove keyword <keyword>` sub-command to remove all tracks in the queue whose title contains the specified keyword.
* Added a new `/remove user <user>` sub-command to remove all tracks in the queue that were added by the specified user.
* Added new `/sortqueue <title | author | length> <asc/desc>` command to re-sort the queue.
* Added new `/sortqueue reverse` command to re-sort the queue in reverse.
* Added new `/sortqueue swap <firstIndex> <secondIndex>` command to swap two tracks around in the queue.
* Updated `/playlist list` & `/playlist delete` so they can be used while music is not playing.
* Added new `/playlist rename <name> <newName>` sub-command to rename user playlists.

#### Removed

* Removed `{prefix}` placeholder for auto responder/custom commands.
* Removed `/rp poke` sub-command due to API being removed.

## July 26th - Music Updates + Bug Fixes

#### Fixed

* Fixed an issue where Cakey Bot would not work in Discord servers that had a newer 19-digit length server ID
* Misc. Bug Fixes

#### Changed

* `/pause` now works as a toggle and will resume if the song is currently paused. (Instead of having to type `/resume`)

#### Added

* The anti-phishing module in the auto moderation now includes several popular IP-grabbing URLs in the blacklist.
* Added an optional `shuffleQueue` parameter to the `/play` command to shuffle the queue after queueing a new song/playlist.
* Added an optional `count` parameter to `/skip` to skip more than one song at a time.
* Added an optional `playTop` parameter to `/play` to insert a song at the start/top of the queue instead of the end.
* Added new `/remove first` sub-command to remove the first track in the queue.
* Added new `/remove last` sub-command to remove the last track in the queue.
* Added a new `/lockqueue` command that will prevent the queue from being modified by non-DJs/moderators. (This will disabling skipping, removing, jumping to, and shuffling but will still allow users to add new songs.)

## July 21st - Query & Slash Command Fixes

#### Fixed

* Fixed `/query` showing incorrect information for PE/Bedrock servers
* Fixed wildcard contains flag for auto responder not working properly with literal `?` triggers.
* Fixed an issue where `/play` would return an incorrect error response

#### Removed

* Removed the `/join` command. Cakey Bot will auto-join when running the `/play` command.

## July 3rd - Command Removal

#### Removed

* Removed `!togglemention` command
* Removed `!togglehoist` command
* Removed `!rolecolor` command
* Removed `!bing` command
* Removed `!covid` command
* Removed `!video` command
* Removed `!staff` command
* Removed `!vote` command
* Removed `!xkcd` command
* Removed `!fakebots` command
* Removed `!premium` command
* Removed `!inviteinfo` command
* Removed `!quote` command

## June 30th - 8D audio

#### Fixed

* Fixed default values for some audio filters
* Fixed audio filters not properly disabling

#### Added

* Added new `!8d` audio filter for music `[Premium command]`
* Added new `!reverb` audio filter for music `[Premium command]`

## June 28th - More music sources and Echo filter

#### Added

* Added support for `.mkv` files for Direct URL source
* Added new `Echo` music filter. Usage: `!filter echo <delay> <decay>`
* Added a ton of new support music sources:
  * Apple music
  * OC Remix
  * Get Yarn
  * Clyp It
  * Reddit
  * Mix Cloud
  * TikTok _**(Experimental, works on most videos)**_

## June 2nd - Text-In-Voice + Music Filters

#### Changed

* Fined tuned all music filters to sound a bit better

#### Added

* Cakey Bot now supports Text-In-Voice channels
* Added new "bandpass" filter

## June 1st - Massive Music Rewrite - Part 1

#### Fixed

* Fixed inactivity disconnect after 30 seconds
* Fixed `!join` saying it lacks permissions when it joins anyways
* Fixed `!move` just disconnecting Cakey Bot
* Fixed `!nowplaying` now highlighting the song title link incorrectly
* Fixed missing emoji on the FinishedPlaying/NowPlaying message
* Fixed `!lyrics` not working
* Fixed being able to go into negatives with `!rewind`

#### Changed

* Moved TrackEnd code into player & fix now playing messages when a track ends (much more reliable)
* Slightly increased `!lyrics` cooldown to prevent abuse
* Decreased audio buffer size (Filters/volume changes take effect faster)

#### Added

* Added support for voice text channels (sometimes fails due to DNet bug will be fully functional in a few days)
* Added ability for DJs/Admins to force move cakey while playing music

## May 30th - Auto Role Fix

#### Fixed

* Fixed an issue where Cakey Bot would spam auto roles when modifying a user's roles

## May 28th - Anime Fixes

#### Fixed

* Fixed `!anime` command
* Fixed `!manga` command

#### Changed

* Prefixes are now case-insensitive

## May 25th - FMBot Bot Scrobbling

#### Added

* FMBot's Bot Scrobbling feature now works with Cakey Bot's music. ([https://fmbot.xyz/](https://fmbot.xyz/))

## May 21st - More Support Tickets

#### Changed

* Ability to open up-to \~500 support tickets (Discord max channel limit) \[Previously was limited to \~150]

## May 20th - Misc Bug Fixes

#### Added

* Added more URLs to phishing URL

#### Fixed

* Debug inspect will now send the output as a file if the content is longer than 2k characters (Reported by @CelticTrinculo )
* Fixed hierarchy related error messages (Reported by @CelticTrinculo )

## May 17th - Confirm Delete Fix

#### Fixed

* Fixed `{confirmdelete}` placeholder

## May 16th - Support Fixes

#### Fixed

* Re-wrote the entire Support Ticket category creation process so it should be much more reliable (Discord caching messed with it a bit)

#### Changed

* Swapped Cakey's default auth link to in-app
* Added in-app auth to all Cakey music bots

#### Removed

* Removed `!steam` command
* Removed `!moviedb` command
* Removed `!timezone` command
* Removed `!fortune` command
* Removed `!modmenu` command
* Removed `!imdb` command
* Removed `!trailer` command

## May 9th - Timestamp QOL

#### Changed

* Updated all visible timestamps to use Discord's localized timestamp system
  * `!warnings`, `!userinfo`, `!serverinfo`, `!inviteinfo`

## May 2nd - Banner Fixes

#### Fixed

* Join/leave banners have been restored and are now functional again.

## April 17th - Bug Fixes

#### Fixed

* Fixed transcripts not showing any messages for embeds or file attachments on support tickets
* Fixed auto mod invite false positives with channel/message links
* Fixed Cakey Bot's DM/group chat detection

#### Changed

* Improved layout/formatting for `!serverinfo` and `!userinfo` commands (Also removed deprecated fields)
* Audit message deleted will now directly attach any deleted images to the audit log message for persistent storage instead of relying on third parties (Imgur)

## April 14th - Responder Bug Fixes

#### Fixed

* Fixed webhook detection for auto responder

## April 12th - Higher Ticket Limits

#### Changed

* Increased number of open tickets a server can have (50 => 150)
  * This limit was due to category channels only being able to have up to 50 channels each, Cakey Bot will now create "Support Tickets 2" and "Support Tickets 3" as needed.
  * If this becomes insufficient, I'll increase the limit again for larger servers.

## April 9th - Custom Embeds

#### Added

* You can now attach a custom embed to your auto responders and custom commands!
* To create an embed, log in to our web dashboard and navigate to the "**Embed Editor**" page which will take you to: [https://cakeybot.app/dashboard/public/embed-editor](https://cakeybot.app/dashboard/public/embed-editor). Once on this page, you can customize the embed to your heart's content and copy the browser URL. You then take the browser URL you copied and paste it into the embed or custom command of your choice in the "**Embed URL**" input field.
* Note: For the time being custom embeds will be limited to Premium servers only.

## April 5th - Song Thumbnails

#### Fixed

* Cakey Bot now supports Stage channels again
* Re-added thumbnail preview support for `!nowplaying` commands
* Song request channel image should now update to resolved track image again

## March 26th - Query Bug Fix

#### Fixed

* Fixed `!query` for MCPE/bedrock servers

## March 22nd - Timeout Improvements

#### Changed

* Update `!timeout` command max duration to 28 days

## March 14th - Reply Placeholder

#### Added

* Added new `{reply}` placeholder for custom commands/auto responder to "reply" to the message that triggered it.

## March 13th - Radio Streams

#### Added

* Added new `!radio` command to easily queue up live radio streams without finding the direct URL. (If you have suggestions for more, post them in 「🌟」feature-requests )
  * Note: You can still use direct URLs for live radio if you wish

## March 11th - Music Fixes + Spotify Playlists

#### Fixed

* Fixed single-song Spotify URLs not loading
* Fixed `!nowplaying` showing the incorrect source (Will be applied on next restart)

#### Changed

* Disabled the ability to use playlist URLs in `!search` command (Since it's designed to only load a single song anyways)
* Patched an exploit where `!playlist` command allowed users to bypass premium restrictions on music
* Moderation commands now include use-specified reason in the audit log entry

#### Added

* Added "stayed for" property to audit user left event
* Added support for Spotify playlist URL loading
* Added reason support for `!timeout` command

## March 6th - Social Feed Features

#### Added

* Added new `!timeout <user> <time>` command.
* Modified social feed limits (read up in 「📣」website-updates )
* Added the ability to have social feeds ping a specific role
* Ability to set custom embed color for social feeds coming soon

## March 5th - Reddit Fixes

#### Fixed

* Multiple fixes for Reddit social feed

#### Changed

* No longer require channel ID for any social feed

#### Added

* Added support for "Link Posts" on Reddit feeds
  * Images for "Link Posts" will properly be embeded inside of Discord as a preview

## March 2nd - Auto Responder Fixes

#### Fixed

* Auto Responder webhook trigger should now be functional again
* Fixed an issue where Twitch/Reddit feeds would not send at all

#### Changed

* Custom Commands/Auto responder `{not:}` & `{require:}` placeholders are now checked before all other placeholders. (This means `{delete}` no longer triggers if you have a `{not:}` placeholder)

## Feb 25th - Auto Mod Punishments

#### Added

* Added new auto mod punishment type: `Delete & Timeout User (1h)`
* Punishment type now shows on the auto mod log entry

## Feb 21st - More Trivia Questions!

#### Added

* Added 500 new trivia questions!

## Feb 20th - Auto Mod Fixes

#### Fixed

* Mass capitalization, Duplicate character and duplicate word checks should now work properly with "min character" and "min percent" properties
* Discord invite link check should now properly detect Discord invites again (the anti-phishing module broke this by accident)

## Feb 15th - Image Manipulation/Banner Fixes

#### Fixed

* Fixed join/leave image banners not working
* Fixed `!query` banners not working
* Fixed `!pride` command not working

#### Added

* Added support for canary URLs to auto quoter

## Feb 14th - Misc. Bug Fixes

#### Fixed

* `!trivia` now properly disables answer buttons after being clicked
* All Image Manipulation commands support messages with multiple attachments/images
  * Currently it only applies to the first image/attachment
* Fixed a ton of misc. errors and bugs

#### Changed

* Uploaded completed Arabic translations

## Feb 3rd - Fixed Webhooks/Social Feeds

#### Fixed

* Twitch and Reddit social feeds should now send as expected again

## Feb 2nd - Phishing Improvement

#### Changed

* Cakey Bot will now ignore URLs on the phishing check if the URL is added to the dashboard whitelist (if you have false positive triggers)

## Jan 26th - Fixed Error Messages

#### Fixed

* Fixed error messages not displaying (ratelimits, missing permissions, module disabled, multiple matches, etc)
* Fixed typereader not working with plain user IDs on commands

## Jan 25th - Error Message Bug Fixes

#### Fixed

* Fixed multiple bugs with `!warnings` if the user has left the server or doesn't share _any_ servers with Cakey Bot.
* Fixed error messages not showing on invalid server/guild users

#### Added

* Fully pushed caching for server settings on Cakey Bot. This means some changes on the web dashboard may take up to 5 minutes to apply in your server.
  * Some settings (like auto responder, custom commands, tags and auto moderation) will all still update live/instantly.

## Jan 9th - Silent Moderation QOL

#### Changed

* "-s" and "-silent" will be stripped from the reason
* "\[SILENT]" will be prefixed before the reason so that you know the action was done silently (without sending a DM to the user)

Remember, if you run the command in a public channel, some users may still see that you took the action, silent just prevents Cakey from sending a notice DM to the infracted user.

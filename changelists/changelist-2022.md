# Changelist - 2022

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

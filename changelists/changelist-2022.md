# Changelist - 2022

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

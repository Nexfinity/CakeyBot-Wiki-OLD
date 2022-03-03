# Changelist - 2022

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

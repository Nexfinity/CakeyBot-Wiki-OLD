# Changelist - 2022

## Jan 26th - Fixed Error Messages

#### Fixed

* Fixed error messages not displaying (ratelimits, missing permissions, module disabled, multiple matches, etc)

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

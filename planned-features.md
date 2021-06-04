# Planned Features

{% hint style="info" %}
Note: Just because a feature is listed here does NOT guarantee that it will be implemented. This is just a general TO-DO list and can be changed at any time without notice. Some features that are not on this list may also be implemented/added.
{% endhint %}

## In Progress

* Auto Message \(Send automated messages on a specific interval\)
* Commands to manage/update multiple users at once
  * `!massban <user1> | <user2> | <user3> | etc`
  * `!masskick <user1> | <user2> | <user3> | etc`
  * `!masspersist <role> <user1> | <user2> | <user3> | etc`
  * `!masswarn <reason> | <user1> | <user2> | <user3> | etc`
  * `!massmute <user1> | <user2> | <user3> | etc`
* Custom image banners for join/leave `[Premium]`
* Fix github previewer not working when line count range is &gt;10
* Investigate/fix tempmute/tempbans
* Handle expiring premium plans

## General Features

* Reaction/Button Role System
* Ability to modify reason for warns \(mods their own, admins any\)
* Starboard
* Mod Cases
* Tags
* Auto Purge
* Auto Punish
* Reddit/youtube/twitch/twitter/rss subscriptions

## Music Features

* `!autoplay` - Auto play the given song or stream while queue is empty
* `!movesong` - Moves a song around in the queue \(Modification of shuffle\)
* Add `!lockqueue` command
* Add ability to list your custom playlists
* Have a global "default" playlist that loads random NCS song playlist and shuffles it
* Have YouTube videos skip to time if included in URL
* Have bot auto disconnect if queue ends and no song is re-queued within 30s
* "autojoin" function, so that the bot automatically joins a certain channel whenever someone joins it, in case the bot its not at that channel yet.

## Support Ticket System

* `!new` - Creates a new ticket/channel @ pings given support role
* `!close` - Closes the support ticket
* `!tadmin` - Various admin commands for ticket system

## Web Dashboard

* Have support tickets displayed
* Embed builder and sender
* Allow vars on custom commands \(include $1, $2, $1+\)
* Voice-Text channel linking
* Have option to allow custom commands to overwrite default command behavior
* Properly re-sync database \(Remove ~828 invalid guilds\)


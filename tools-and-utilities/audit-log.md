# Audit Log

## Overview

Cakey Bot has a very detailed feature-rich audit log, in addition to logging all of the events in the **Events** section below Cakey Bot also includes "Jump To" and "Perma-Link" features for some events. Audit Log not only logs highly detailed information for events but it can also log information for events that discord and most other bots don't log. For example, Cakey Bot logs both when a user boosts and when they quit boosting as well as permanent links for deleted images.

## Enable/Disable Logging

In order to start logging you will need to designate a text channel as the log channel. You can do this by selecting a channel in the [Web Dashboard](https://cakeybot.app/dashboard/public/) on the "Audit Log" page. In order to disable logging, simply select "none" in the channel dropdown list.

{% hint style="warning" %}
Cakey Bot will need access to Send/Read messages in the channel you designate as the audit log.
{% endhint %}

## Audit Events

* User Joined
  * Shows Account Creation Date
* User Left
  * Shows Server Join Date
  * Lists every role the user had
* Message Deleted
  * Includes any attached images from the deleted message
  * Includes logs of deleted system messages including when users delete their own join message
  * Displays if the deleted message was a reply to another message and includes the content from that original emssage
  * Shows message author & message content
* Message Modified
  * Includes "Jump-To" button
  * Shows before/after message content
* Bulk Message Deletes
  * Bots are able to bulk delete messages, causing this event to trigger instead of the normal "Message Deleted" event
  * Unlike most bots, Cakey Bot will include a transcript of all of the bulk deleted messages.
* User Updated (Nickname changed)
  * Shows before/after nickname
* User Updated (Roles changed)
  * Shows role name + if it was added/removed
* User Updated (Voice channels)
  * Shows when a User Joined/Left/Swapped voice channels
* User Banned/Unbanned
* User Kicked
* Server Updated (Nitro Boost)
  * Shows before/after boost count
  * Shows Current Tier level
* Role Created/Deleted
* Role Updated
  * Shows before/after permissions
  * Shows before/after name
  * Shows before/after properties (hoisted, mentionable, color, etc)
* Channel Created/Deleted
* Channel Updated
  * Shows before/after permissions
  * Shows before/after name
  * Shows before/after properties (slow mode, topic, isNSFW, category, etc)
* Invite Created/Deleted
* Thread Created/Deletion
* Thread Updated
  * Shows before/after name
  * Shows before/after properties (slow mode, auto-archive time, isLocked, isArchived, etc)
* Stage Started/Ended
* Stage Updated
  * Shows before/after name
  * Shows before/after permissions
  * Speaker changes

## Special Events

* Server Boost
  * When a member boosts your server, Cakey Bot will log the old and new boost value as well as the current boost tier.
  * This event is also fired when a boost is removed from the server.
* Warnings
  * When a moderator uses the `/warn` command it will log the usage to the audit log
* Purges
  * When a moderator uses the !purge command it will log the amount of messages and the purge type to the audit log
  * If Cakey Bot has not hit the rate limit yet, purge will also include a Pastebin perma-link to all of the messages that were purged.

## Additional Information

* Message Deletion
  * Cakey Bot only caches the last 100 messages per channel. If a message is deleted past that, Cakey Bot will not be able to show the content of that message.
  * Cakey Bot will not log who deleted the message.
  * Cakey Bot will provide a separate URL if the message contains an image. (If it's possible to do so)
  * Cakey Bot will not show the content of deleted embed messages.
* Member Join
  * Cakey Bot will display the date that the user created their account.
    * This is useful for tracking and finding newly created alternate accounts.
* Member Left
  * Cakey Bot will display a list of any roles that use had when they left.
  * Cakey Bot will display the date of when the user joined the server.

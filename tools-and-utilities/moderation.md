# Moderation

{% hint style="warning" %}
Many commands in this module require higher-level permissions such as **`Manage Channels`**, **`Manage Messages`**, **`Manage Roles`**, **`Ban Members`** and **`Kick Members`**.
{% endhint %}

## Features

* Dehoisting Members
  * Ability to manually or automatically dehoist users who use special characters in their usernames/nicknames to show at the top of the user list.
* Kick Members
  * Ability to kick members with an optional warning.
* Ban Members
  * Ability to ban members with an optional warning.
  * You can also ban people temporarily using the `/tempban` command
* Purge/Clear/Clean Messages
  * Ability to purge the last X amount of messages in a channel.
  * Advanced purge commands allow you to purge messages from bots only, specific users, between specific time frames and more!
* Mute Members
  * You can assign mutes to members with an optional reason.
  * You can either use a custom mute role or let Cakey Bot generate a default mute role.
  * If you have multiple mute roles Cakey bot will either use the first valid one or the one specific set in Cakey Bot's configuration.
  * You can also mute people temporarily using the `/tempmute` command
* Warn Members
  * You can place a warning on users with a specific reason
  * Warnings get logged to your [Audit Log](audit-log.md) if one is setup
  * You can see how many warnings a user has gained, as well as their reasons and who warned them each time.
* Silent Actions
  * You can mute, kick, ban and warn users silently using "-s" or "-silent" anywhere in the reason section of the command.
* User Reports
  * You can set a channel on the Web Dashboard where user reports are sent. Normal users can make reports with the `/report <text>` command.
* Plus so much more!

## Auto Moderation

If you are wanting Cakey Bot to automatically handle moderation you can check out [this section](auto-moderation.md) for more information.

## Warnings

You can warn users with a given reason using the `/warn <user> <reason>` . It will place a warning on their account which you can then view later with the `/warnings <username>`. Warnings will record the date the warning was received, the reason as well as the moderator who made the warning. Warnings will also automatically post to your [Audit Log](audit-log.md) if you have one set up for Cakey Bot. If you want to remove a specific warning from a user you can simply do `/unwarn <user> <warning ID>`.

## Muting

When you run the `/mute <user>` command, Cakey Bot will assign a mute role to that user preventing them from chatting/speaking in voice channels. Now, You might be asking "What role does Cakey Bot use for this?". This depends on a few factors:

1. If you have set a mute role in the web dashboard, Cakey Bot will use that role.
2. If you have not manually set a mute role, Cakey Bot will scan for any role with the name "Muted", if it finds one it will use that role.
3. If Cakey Bot does not find a "Muted" role, it will generate a brand new role with appropriate permissions

{% hint style="info" %}
Note: In order for Cakey Bot to mute a user several things must happen. Cakey Bot must have **`Manage Roles`** permission and Cakey Bot's highest role must be higher than the Mute role and the muted user's highest role.
{% endhint %}

## Temporary Mutes

You can also mute people temporarily. It works exactly like normal muting above and requires the same setup/permissions but it will automatically remove the mute after the specified time. You can temporarily mute someone by using the `/tempmute <user> <time> <opt:reason>`command.

## Silent Actions

When you run most moderation commands on a user, they send a DM/Notification to the user via private messages. There are some instances where you may not want this capability. You can cancel sending a DM notification by adding `-s` or `-silent` anywhere in the "reason" section of the command.

For example: `/warn TestSubject -s Spamming the chat` will add a warning to the user but will not send a DM to them.

## Advanced Purge Filters

You can purge any amount of messages (up to 100) by typing `/purge <amount>`. This will delete the specified number of messages as long as they are not older than 2 weeks and are not pinned.

You can also filter what types of messages you want to delete by typing `/purge <type> <amount>`. You can view a list of advanced filters below:

* Links (Any well-formatted URL/Link)
* Invites (Discord invite links)
* Images (Any messages that have an image/file attached)
* Mentions (Any messages that contain at least 1 user mention)
* Embeds (Any messages that contain an embed)
* Self (Any messages that were sent by Cakey Bot)
* Bots (Any messages that were sent by a bot)
* Components (Any messages that have buttons or selection dropdowns)
* User (Any messages that were sent by the specified user)
  * **Special Format:** `/purge user <user id>`
* Until (Deletes every message between the command and the specified message ID)
  * **Special Format:** `/purge until <message id>`
* Between (Deletes every message between the specified message IDs)
  * **Special Format:** `/purge between <message id> <message id>`

{% hint style="warning" %}
Sometimes Cakey Bot will purge fewer messages than the number you specify. This could be due to a few reasons:

* There are not enough messages that meet the specified filter
* Some messages may be older than 2 weeks within the specified amount
* Some messages may be "pinned" within the specified amount
{% endhint %}

## Username Dehoisting

Username dehoisting gives you the ability to manually or automatically dehoist users who use special characters in their usernames/nicknames to show at the top of the user list.

### Manually Dehoist

You can manually dehoist users by typing the `/dehoist` command in Discord. There are a few different types of dehoisting you can do:

* All
  * This will dehoist every user in the server. Note that this command may take several minutes to complete, especially in a large server.
* Single \<user>
  * This will just dehoist that specific user.
* Role \<role>
  * This will dehoist all users who have the specified role.

### Automatically Dehoist

You can setup automatic dehoisting by logging into our [web dashboard](https://cakeybot.app/dashboard/public) and going to the "Auto Mod" page. Once on the page, simply enable the "Auto Dehoist" feature and Cakey Bot will start automatically dehoisting users.

{% hint style="info" %}
Note: Auto Dehoist will only apply to new users in the server or suers who change their nickname AFTER the feature has been enabled. For existing users you will need to manually dehoist them. After existing users have been dehoisted, auto dehoist will take affect for new nickname changes.
{% endhint %}

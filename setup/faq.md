# FAQ

{% hint style="info" %}
If you can't find the answer to your question you can contact us on our discord [support server](https://cakeybot.app/discord).
{% endhint %}

## How do I invite Cakey Bot to my server?

{% hint style="warning" %}
You will need **`Manage Server`** or **`Administrator`** permission to add Cakey Bot to your server.
{% endhint %}

You can invite Cakey Bot using this [Discord OAuth URL](https://cakeybot.app/invite). If you do not want the bot to have **`Administrator`** permissions you can change them after you invite the bot like you would any other role/user.

To view a list of require/optional permissions you can check out [this section](setup.md#inviting-cakey-bot).

## Why isn't Cakey Bot responding to any commands?

1. Type `@Cakey Bot#2608 help`. If Cakey Bot responds, you have the correct permissions but were using an incorrect prefix. The help command you just ran will show you what the current prefix is.
2. Check the channel permissions to see if Cakey Bot has Send/Read permissions for the channel. You can either check permissions manually or use the `!debug` command. **This is the most common reason why Cakey Bot doesn't respond.** 
3. Make sure that Cakey Bot is online. Discord might be having issues or Cakey Bot may be restarting to apply new updates/content. 
4. If none of these steps work you can join our discord [support server](https://cakeybot.app/discord) here for direct help from our developers.

## What is the default prefix and how can I change it?

The default prefix is `!` \(exclamation point\). To change the prefix you can either use the `!prefix <new prefix>` command or modify it in the [web dashboard](https://cakeybot.app/dashboard/public/).

{% hint style="info" %}
If you forget what you set your custom prefix to you can always check it using the `!prefix` command or by mentioning/tagging Cakey Bot.
{% endhint %}

## Where can I find my User/Channel/Role/Server ID?

You can find an extremely detailed and easy to follow guide [here](https://support.discord.com/hc/en-us/articles/206346498-Where-can-I-find-my-User-Server-Message-ID) written by Discord.

## What is considered a server moderator?

Some commands in Cakey Bot are restricted to "Server Moderators". Cakey Bot considers anyone with the permissions listed below as a "Server Moderator".

* Administrator
* Manage Server
* Manage Channels
* Manage Messages
* Mute/Ban/Kick Members

{% hint style="info" %}
Some music commands also require a "Server Moderator". Any music commands that require this permission will also accept users who contain a role named "DJ" to run the command as well.
{% endhint %}

## Why is Cakey Bot offline in my server but online in other servers?

Cakey Bot may be working on some servers, but not on others. This is because the Cakey Bot is shard based and runs on multiple shards that each have a set amount of servers \(or servers\) on them.

## What sources can I listen to music from? Do you support YouTube/Twitch/Spotify?

Cakey Bot supports many different sources including Twitch and Youtube!

You can view all of our current and planned music sources on [this page](../music/supported-sources.md).

## Can I use special variables/custom content in join/leave/ban announcements or custom commands?

Yes! We have a list of variables that you are able to use in both of these features. To see our full list of variables you can check out [this page](placeholders-variables.md) that is dedicated to custom variables.

## How does user muting work in Cakey Bot?

When you run the `!mute <user>` command, Cakey Bot will assign a mute role to that user preventing them from chatting/speaking in voice channels. Now, You might be asking "What role does Cakey Bot use for this?". This depends on a few factors:

1. If you have set a mute role in the web dashboard, Cakey Bot will use that role.
2. If you have not manually set a mute role, Cakey Bot will scan for any role with the name "Muted", if it finds one it will use that role.
3. If Cakey Bot does not find a "Muted" role, it will generate a brand new role with appropriate permissions

{% hint style="info" %}
Note: In order for Cakey Bot to mute a user several things must happen. Cakey Bot must have **`Manage Roles`** permission and Cakey Bot's highest role must be higher than the Mute role and the muted user's highest role.
{% endhint %}

## Why does Cakey Bot deafen itself in voice channels?

Cakey Bot server deafens itself to prevent itself from receiving your audio. This doesn't have any effect on the functionality of the bot and it can play music even if it is server deafened.

This significantly reduces Cakey Bot's bandwidth usage \(since we don't receive what you say in a voice channel\), as well as Discord's bandwidth \(as they don't need to send it\).

This also protects your privacy, as we don't receive any audio from your voice channel.

If you are having trouble playing music, Cakey Bot being deafened will not affect that.

## Why can’t I see my server on the web dashboard?

Make sure you’re logged into the correct Discord account, then refresh the website.

{% hint style="warning" %}
You will need **`Manage Server`** or **`Administrator`** permission to configure Cakey Bot on your server.
{% endhint %}

## How do I set up custom commands/auto responder?

You can set up custom commands using our web dashboard. For more information, you can check out [this section](../tools-and-utilities/custom-commands.md#setup).

You can set up the auto responder using our web dashboard. For more information, you can check out [this section](../tools-and-utilities/auto-responder.md#setup).

## How do I set up audit logging?

You can set up audit logging by checking out [this section](../tools-and-utilities/audit-log.md#overview).

## How do I set up join/leave/ban announcements?

You can set up announcements by checking out [this section](../tools-and-utilities/join-leave-ban-announcements.md).

## Cakey Bot's music is Laggy/Glitchy/Distorted/Not Playing

Sometimes, Cakey Bot's audio may not play or may sound laggy/glitchy/distorted. The vast majority of the time, this is caused by **Discord's Voice Servers**.

The easiest way to fix it is to switch your voice server region to a different one and then to switch it back. This will assign you a new server within that region. If this doesn't work, you can temporarily change it to another region and leave it set to it.

For a tutorial on switching your server region, [click here](https://support.discordapp.com/hc/en-us/articles/216661717-How-do-I-change-my-Voice-Server-Region-).

## Is Cakey Bot open source?

Not currently, though we may look into this option in the future.

## How do I become a BETA tester?

There's a few steps required to become a BETA tester.

1. Join our [Support Discord](https://cakeybot.app/discord).
2. Assign yourself the tester role using the buttons in our [\#server-info-and-rules](https://discord.com/channels/408424043482447872/408434189256359937/848972083684835380) channel.
3. Become an active tester and earn the "Active Tester" role
4. Read the [\#request-beta](https://discord.com/channels/660164229092999183/780131612499247134/780132537162399755) channel to apply

## Why isn’t Auto Mod deleting messages?

The following are some possible reasons why Auto Mod isn’t deleting messages:

* Auto Mod may be configured to ignore admins/mods. Check this setting in the web dashboard.
* The Auto Mod module is not enabled.
* Cakey Bot doesn’t have **`Manage Messages`** in the channel/role permissions.

If none of these seem to be the cause of this issue, please head over to our [support server](https://cakeybot.app/discord).

## Why can’t I purge messages older than 14 days in a channel?

Discord doesn’t allow bots to purge/delete messages that are older than 14 days old. [Learn more here](https://wiki.dyno.gg/purge-14-day).

## Why won't Cakey Bot assign the Auto Role?

You have to move Cakey Bot’s role above the role you’re trying to manage by going to Server Settings -&gt; Roles and dragging Cakey Bot's role above any roles you want Cakey Bot to manage.

To learn more about role hierarchy, [click here](https://support.discordapp.com/hc/en-us/articles/214836687-Role-Management-101).

## Why isn't Audit Log working on my server?

* Check if the module is disabled via the [Web Dashboard](https://cakeybot.app/dashboard/public/).
* If the module is enabled, check if Cakey Bot can Read and Send Messages in the log channel, as well as Embed Links. To quickly check if Cakey Bot has those permissions, run `!debug` in the channel.
* Lastly, check if a channel has been set for Audit Log by running `!setting log`

If none of these seem to be the cause of this issue, please head over to our [support server](https://cakeybot.app/discord).

## Why does Cakey Bot automatically leave my server when invited?

Cakey Bot may automatically leave servers for a few reasons. Some of these are listed below:

* The server is blacklisted from Cakey Bot
  * If servers abuse Cakey Bot too much, the server \(and/or server owner\) can be blacklisted from using the bot
* The server is a "Bot Hell"
  * Some servers will have hundreds/thousands of bots but only a handful of users. Bots in these servers are generally spammy and pointless which adds unnecessary load to Cakey Bot.
  * Cakey Bot will attempt to DM the server owner if this happens.


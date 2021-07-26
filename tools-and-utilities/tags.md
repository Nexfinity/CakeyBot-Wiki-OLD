# Tags

## Overview

This module allows you to setup a variety of "tags" that users can list and use to output pre-determined strings of text. This is useful for creating public FAQ responses without making a bunch of [Custom Commands](custom-commands.md). Also, you can configure tags to be modified by different permission levels, unlike Custom Commands which can only be modified by server admins. The different permission tiers are listed below:

* Anyone - Anyone can add, delete and modify any tag.
* Tag Owner - Anyone can add tags, but they can only delete or modify tags that they created. \(Server admins can always modify/delete ALL tags\)
* Server Mods - Anyone considered a "Server Mod" can create, delete and modify any tag.
* Server Admins - Anyone with the "Administrator" permission node can create, delete and modify every tag.

{% hint style="info" %}
**Note:** These permissions only affect creating, deleting and modifying tags. ALL users will be able to USE every tag regardless of who created the tag.
{% endhint %}

## Setup/Manage Tags

1. Login to our [web dashboard](https://cakeybot.app/dashboard/).
2. Go to "Tags" [here](https://cakeybot.app/dashboard/public/tags).
3. Click the "Add New Tag" button
4. Fill in the required information. All tags will require a name and a response.
5. Click "Create"

Once you have created tags, you can also modify them here.

## Limitations/Restrictions

* You can't have duplicate tags with the same name
* Tags are also limited to Discord's message character limit
* Messages sent by bots or webhooks will be ignored
* @User, @Role and @Everyone/@Here mentions are completely disabled in tags

## Using Emoji/Emotes in Tags

Emoji/Emotes CAN be used in Tags. However, it requires slightly more work due to how discord parses emotes. Normally in Discord, you could just type `:lel:` or `:smile:` to get an emote, however in Cakey Bot, neither of these will work. In order to get valid emojis you have to send the emojis in discord but place a backward slash in front of it to get the emote's full ID. Like so: `\:lel:` or `\:smile:` which will produce these results: `<:lel:408424717217693717>` or for Unicode emoji: `😄` . Once you have the full emoji id or the raw Unicode output, you can paste these into Cakey Bot's web dashboard and they should work as long as Cakey Bot is in a server that has that custom emote in it.

{% hint style="info" %}
It is worth noting that Cakey Bot can use emojis in between servers \(similar to nitro users\). So if you have an emoji in Server \#1, you can use that emoji in a custom command in Server \#2 if Cakey bot is in both of those servers.
{% endhint %}

### Using Images in Tags

To use images in responses, you can simply just type the image URL/link like you would in a normal message. If you have the file on your local machine/PC but no URL/link, you can upload it to an image hosting website \(such as [Imgur](https://imgur.com/upload)\) and paste the URL they provide into the response. Cakey Bot should automatically embed the image in Discord's client if it's a valid URL/image.


# Custom Commands

## Overview

This feature allows you to set up custom commands that Cakey Bot can handle. For example, you can make your own command called `!support` which will post a message informing your users where they can get support for your server.

## Setup

{% hint style="warning" %}
You will need **`Manage Server`** or **`Administrator`** permission to manage servers and custom commands.
{% endhint %}

1. Login to the web dashboard on the [main website here](https://cakeybot.app/auth.php).
2. Click on the server you want to edit custom commands on.
3. Go to the "Custom Commands" page.
4. You can then create, delete and edit any commands on this page. You can get an overview of any triggers that are available below. You can also use our [custom placeholders](custom-commands.md#basic-placeholders) in your commands as well!

{% hint style="info" %}
The command trigger will use a custom set prefix if you have changed Cakey Bot's prefix.
{% endhint %}

## Limitations/Restrictions

* You can't have duplicate triggers with the same name
* Custom Commands are also limited to Discord's message character limit
* Messages sent by bots or webhooks will be ignored

## Using Emoji/Emotes in Command Responses

Emoji/Emotes CAN be used in Custom Commands. However, it requires slightly more work due to how discord parses emotes. Normally in Discord, you could just type `:lel:` or `:smile:` to get an emote, however in Cakey Bot, neither of these will work. In order to get valid emojis you have to send the emojis in discord but place a backward slash in front of it to get the emote's full ID. Like so: `\:lel:` or `\:smile:` which will produce these results: `<:lel:408424717217693717>` or for Unicode emoji: `😄` . Once you have the full emoji id or the raw Unicode output, you can paste these into Cakey Bot's web dashboard and they should work as long as Cakey Bot is in a server that has that custom emote in it.

{% hint style="info" %}
It is worth noting that Cakey Bot can use emojis in between servers (similar to nitro users). So if you have an emoji in Server #1, you can use that emoji in a custom command in Server #2 if Cakey bot is in both of those servers.
{% endhint %}

### Using Images in Command Responses

To use images in responses, you can simply just type the image URL/link like you would in a normal message. If you have the file on your local machine/PC but no URL/link, you can upload it to an image hosting website (such as [Imgur](https://imgur.com/upload)) and paste the URL they provide into the response. Cakey Bot should automatically embed the image in Discord's client if it's a valid URL/image.

### Placeholders/Variables

Custom Commands will work with BOTH **Basic Placeholders** & **Advanced Placeholders**. Placeholders can be included in the response section and can modify the behavior/output of the response. You can find the full list of supported placeholders [here](../other-misc/placeholders-variables.md).

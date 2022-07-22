# AFK Messages

## Overview

AFK messages allow you to automatically display a message to users who ping you. This allows you to explain why you might not be responding or when you'll be back. AFK messages have a 100 character limit to prevent abuse and you are unable to use clickable links/user mentions in the message. Currently AFK messages are permanent and will last until you or a server admin removes it.

{% hint style="info" %}
If Cakey Bot has the appropriate permissions \(**`Add Reactions`** and **`Manage Messages`**\) any AFK message will have a trashcan reaction added to it. When clicked, it will delete the AFK message in order to keep the channel clean.
{% endhint %}

## Setting an AFK Message

You are able to set your own AFK message by typing `/afk <message>`. If you ever forget what you have your AFK message set to you can always type `/afk` without any message and it'll show what message you currently have set. \(If one is set\)

{% hint style="warning" %}
Your AFK message will not be sent if a BOT mentions you or if you mention yourself.
{% endhint %}

## Removing an AFK Message

{% hint style="info" %}
Users who have the **`Manage Server`** permission node can force remove a user's AFK message using the `/unafk <user>` command.
{% endhint %}

You are able to remove your own AFK message by typing the `/unafk` command.

## Extra Configurations

You can also configure AFK messages further by using our [Web Dashboard](https://cakeybot.app/dashboard/public). There are two main options you can change:

1. AFK Module Status
   * This toggles whether or not users can set AFK statuses in your server
2. Max AFK Time
   * This sets how long the user's AFK status will be active before being automatically removed.
   * This can be anywhere from 1 minute to 10,080 minutes. \(1 week\)
   * If you want AFK statues to be permanent, you can just set this value to -1.
     * This is the default value for all servers.

You can also view all AFK users [here](https://cakeybot.app/dashboard/public/afk-list).


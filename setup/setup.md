# Setup

## Inviting Cakey Bot

{% hint style="warning" %}
You will need **`Manage Server`** or **`Administrator`** permission to add Cakey Bot to your guild.
{% endhint %}

{% hint style="info" %}
While Cakey Bot's invite link defaults to **`Administrator`**, it does not require this permission to function. It's just to make setup simpler for those who don't want to spend time on channel/role-specific permissions.
{% endhint %}

You can invite Cakey Bot using this [Discord OAuth URL](https://discord.com/oauth2/authorize?client_id=288163958022471680&permissions=8&redirect_uri=https%3A%2F%2Fdocs.cakeybot.app%2F&response_type=code&scope=bot+identify+guilds+applications.commands). If you do not want the bot to have **`Administrator`** permissions you can change them after you invite the bot like you would any other role/user.

#### Required Permissions:

* Send Messages
* Read/View Messages/Channels
* Use External Emoji
* Add Reactions

#### Optional Permissions:

* Connect/Speak/Voice Activity \(For Music commands\)
* Manage Roles/Channels/Emoji/Server \(Server Management commands\)
* Kick/Ban/Mute/Manage Nickname/Manage Messages/Manage Roles \(Moderation commands\)

#### Wildcard Permissions:

* Administrator - If you don't want to worry about specific permissions you can just grant Administrator.

{% hint style="warning" %}
It is not recommended to freely give out Administrator permission. It would just make setting up the bot simpler. Cakey Bot has many built-in safeguards to prevent the bot from being abused by users if the bot has Administrator so it is safe to grant, just not a recommended practice to do so.
{% endhint %}

## Per-Guild Settings \(Web Dashboard\)

{% hint style="warning" %}
You will need **`Manage Server`** or **`Administrator`** permission to customize Cakey Bot in your guild.
{% endhint %}

After you invite Cakey Bot, most commands/features will work right out of the box \(assuming it has the correct permissions\). However, there are some more advanced features that you can enable. Some of these features include but are not limited to: multiple languages, custom prefix, custom commands, audit logging, etc. 

You can access the web dashboard [here](https://cakeybot.app/dashboard/public). All of Cakey Bot's most advanced features can be configured through the web dashboard.

You can configure advanced features like the ones listed below in the web dashboard:

* Bot Prefix
* Default music volume
* Bot Language
* Modify Module-Specific Configurations
* Setup Custom Commands/Auto Responders
* Setup Auto-Moderation
* View Guild Stats
* View Music Queue
* View Audit Logs
* View User Warnings
* View Persistent and Temporary Roles

and more!

## Per-Guild Settings \(Setting Command\)

{% hint style="warning" %}
You will need **`Manage Server`** or **`Administrator`** permission to customize Cakey Bot in your guild.
{% endhint %}

To configure/modify the most settings you will need to use the [Web Dashboard](https://cakeybot.app/dashboard/public/). However, you can use `!setting prefix <new prefix>` to set the prefix within the guild. \(The prefix can also be set via the web dashboard if desired.\)


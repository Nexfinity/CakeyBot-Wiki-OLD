# Troubleshooting

## Basic Troubleshooting

### When adding Cakey Bot, I can't see my server in the list!

* Are you signed into the correct account?
  * If you can't find your server in the drop-down section, this can be caused by various reasons. First, you should make sure that you're signed into the correct account. If you're not, then press the blue **Not you?** button.
* Do you have permissions in the server you want to add Cakey Bot to?
  *  If you're **100%** sure that you're signed into the correct account, then you should make sure that you have the correct permissions. In order to add a bot, you need to have a role with the `Manage Server` or `Administrator` permission. If you're the server owner, you have those regardless, of course.
* Open an incognito tab and invite Cakey Bot from there.
  *  If you're sure that **you're signed into the correct account** and **you have permissions on the server that you'd like to add Cakey Bot to**, then you should open an incognito tab and invite Cakey Bot from there. You can find instructions in the table below, if you don't know how to do that.

| Browser | Windows/Linux | MacOS |
| :--- | :--- | :--- |
| Chrome | CTRL+Shift+N | CMD+Shift+N |
| Firefox | CTRL+Shift+P | CMD+Shift+P |
| Opera | CTRL+Shift+N | CMD+Shift+N |
| MS Edge | CTRL+Shift+N | CMD+Shift+N |
| Explorer | CTRL+Shift+P | N/A |
| Safari | N/A | CMD+Shift+N |

* Why is this necessary?
  * Because Discord caches data into cookies, it retains old account information and glitches out the bot invite screen. By using an incognito/private browsing window, it forces Discord to use a fresh session which fixes the glitch and allows you to select a server from the drop-down menu.

### When adding Cakey Bot, Discord asks me to verify my e-mail address.

![](../.gitbook/assets/ss5.jpg)

Discord requires you to verify your e-mail account to add bots into your servers. Head to the User Settings and verify your e-mail there.

### I can't invite Cakey Bot on my mobile device!

*  For any issue with inviting Cakey Bot on mobile devices, see the [Mobile Troubleshooting](troubleshooting.md#mobile-troubleshooting) section.

### Cakey Bot isn't responding to my commands!

* If Cakey Bot isn't responding to commands, try the following:
  1. Make sure Cakey Bot is showing as online.
     * If Cakey Bot is offline, try kicking the bot out of your server and inviting it again. If after doing that Cakey Bot is still showing as offline, you may skip to step 4.
  2. Make sure you're using the correct prefix. You can type `!prefix` to get the prefix.
     * You can learn how to change Cakey Bot's prefix by heading to the [Prefix Setting](faq.md#what-is-the-default-prefix-and-how-can-i-change-it) section!
  3. Make sure Cakey Bot has the permissions to read and send messages in the channel.
     * You can give the `Administrator` permission to Cakey Bot to make this easier.
  4. Take a look at our [\#status-and-outages](https://discord.com/channels/408424043482447872/697929149356179516) channel on our official [Cakey Bot Discord](https://cakeybot.app/discord) server to see if there are any issues going on. You can also check out our NEW [status page](https://cakeybot.statuspage.io/).
  5. If the above methods do not work, please choose option 3 in our [\#support](https://discord.com/channels/408424043482447872/730159265209253908) channel on the [Cakey Bot Discord](https://cakeybot.app/discord) server to receive assistance from a member of our Support Team.

## Audio Troubleshooting

### Cakey Bot left the voice channel while not playing anything

* For performance reasons, Cakey Bot leaves after a while of being alone or unused in a voice channel. This helps Cakey Bot save resources while no one is listening to it and keeps the music quality consistent for all users at any given time!
* Don't worry though, as long as you are in a voice channel, just type `!join` to make Cakey Bot rejoin your channel!

### Cakey Bot will not play audio or the  laggy/buggy 

* As you are using Cakey Bot, you may encounter some issues with the audio that is played. This can be due to a few reasons: the Discord voice node you are on could have failed, or it could be an internet connection issue.
* If you are encountering these issues, you can check out [this section](faq.md#cakey-bots-music-is-laggy-glitchy-distorted-not-playing) in order to resolve these issues.



### Cakey Bot forgets the playlist I queued after it leaves

* Due to technical reasons, Cakey Bot will clear/reset the queue when it leaves the voice channel.
* To get around this we suggest creating a YouTube/Spotify playlist of the songs you wish to re-queue.

{% hint style="info" %}
If your queue contains audio from multiple/different sources, you can create a Cakey Bot playlist using the `!playlist` command.
{% endhint %}

### Cakey Bot is responding to commands but not joining the voice channel

* If you find that Cakey Bot is responding to your commands but not joining a voice channel use the following method:
  1. Move to a different voice channel.
  2. `!join` the bot into that voice channel.
  3. Move back to the original voice channel.
  4. `!join` the bot back into the original voice channel.
* If the above method does not work, try changing the server region of your server or kicking & reinviting Cakey Bot to your Discord server.

## Mobile Troubleshooting

### The screen to add Cakey Bot to my server is gray and nothing is showing!

* If you are on mobile and you find that you cannot add Cakey Bot because the link to add Cakey Bot produces a gray screen, please try first heading to [**https://discord.com/login**](https://discord.com/login), logging in and then using the invite link again.
* **If that does not work**, we recommend using a desktop device to invite Cakey Bot.

{% hint style="info" %}
**In short:** You may want to try refreshing the website to add Cakey Bot or use a desktop device!
{% endhint %}

### I met the error "Not supported within the Android app", what should I do?

* If you encounter this error when inviting Cakey Bot, try opening an **Incognito Tab** and copy this link into the search bar: [https://cakeybot.app/invite](https://cakeybot.app/invite)
* [Click here](https://support.google.com/chrome/answer/95464) to learn how to open an Incognito Tab.


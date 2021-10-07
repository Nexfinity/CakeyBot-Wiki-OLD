# Basic Usage

{% hint style="warning" %}
In order to use music Cakey Bot will need **`Connect`** and **`Speak`** permissions for any voice channels you want to listen to music in.
{% endhint %}

### Overview

Cakey Bot can play music from multiple sources which you can view a full list of [here](supported-sources.md). In order to listen to music you will need to follow the steps below.

1. Join a voice channel that Cakey bot has access to join/speak in
2. Type `!join` or `!play <song>` \(The `!play` command will auto-summon Cakey Bot\)
   1. You can also use the `!move` command if no one else is using the bot
3. If you typed !join or !move in step two you will now need to type !play &lt;song&gt; in order to start playing a song

If no song is currently playing when you add one, it will start to play instantly. If a song is currently playing, your song will be added to a queue that will play through automatically.

{% hint style="info" %}
If you play a live stream, other songs in the queue will not be played until either the live stream ends or until someone skips the live stream.
{% endhint %}

### Requirements

Cakey Bot requires at least **`Connect`** and **`Speak`** permissions to function. You will also need to be in a voice channel to summon Cakey Bot to it. If Cakey Bot is currently being used by users in another channel you will not be able to summon it to your channel. Many commands in Cakey Bot excluding `!join` and `!dc` require a song to be playing in order to be used. If a song is not playing an error message will be displayed. Some commands can not be used while a live stream is playing, to use these commands you will have to wait until the live stream ends or skip the live stream.

### Default Volume

By default, Cakey Bot's volume will be set to 50 when playing music. You can change the volume using the `!volume <amount>` command but the volume will revert to 50 if the queue runs out of songs or the next time you use Cakey Bot. You can however change the default volume on our [web dashboard](https://cakeybot.app/dashboard/public/) from 50 to any number between 0 and 100.

### Sound Bites

Cakey Bot also has a pre-made list of fun sound bites you can play outside of music. You can view a full current list of sound bites by running the `!soundbite` command and can play the specified sound bite by running `!soundbite <name>`.

{% hint style="warning" %}
Sound Bites are separate from regular music and will cause Cakey Bot to leave the voice channel and clear any ongoing music queue.
{% endhint %}

### Multiple Music Bots

Cakey Bot has additional bots that you can invite that are designed specifically for music playback! You can find the invites to these bots on our premium page [here](https://cakeybot.app/dashboard/public/premium). Note that you must have premium enabled on the server in order to invite these additional music bots.

### Supported Sources

Cakey Bot supports many different sources including Twitch and Youtube!

You can view all of our current and planned music sources on [this page](supported-sources.md).


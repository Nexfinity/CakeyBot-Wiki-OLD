# Song Request Channel

{% hint style="warning" %}
This feature requires slightly more setup to enable. To add this feature to your discord you must have **`Manage Server`** permissions. Also note that Cakey Bot requires the following permissions as well: **`Create Channels`**, **`Add Reactions`**, **`Manage Messages`** 
{% endhint %}

### Setup

In order to setup this feature you must have **`Manage Server`** permissions. You can then run the `/musicsetup` command in any channel that Cakey Bot has access to read/view messages in. If you and Cakey Bot both have the required permissions, a new channel called _`#cakey_songrequests`_ will have been created. In this new channel you will see a fancy embed with 6 emoji reactions added to it and a block of text with more information under it. Do NOT delete either of these messages. If you do, you will need to delete the channel and run the setup again.

![](<../.gitbook/assets/SS5 (2).JPG>)

{% hint style="success" %}
You can freely rename and move the song request channel into other categories after it's created without any issues as Cakey Bot uses the channel ID to update the messages.
{% endhint %}

### Usage

The song request channel is very simple to use. In order to use it, you (or whoever is attempting to use it) must be in a voice channel that Cakey Bot can view/join. Once you are in a voice channel, you can either post a song name or a URL/Link to a valid music source and Cakey Bot will automatically search for and add the song to the queue. When it has done so, it will also update the embed picture/content. As you add/remove items to/from the queue, the queue message under the embed will also update.

{% hint style="info" %}
You don't have to use the _`#cakey_songrequests`_ channel in order to make use of the embed system! As long as you have the embed/song request channel setup, it will always update with the current song/queue info regardless if you use the channel or if you use regular commands.
{% endhint %}

### Common Issues

{% hint style="danger" %}
Do NOT run commands in the _`#cakey_songrequests`_ channel. Some commands may work, but since the channel takes ANY input as a song request, it will consider your command to be a song request. This could potentially queue up multiple tracks for the same request.
{% endhint %}

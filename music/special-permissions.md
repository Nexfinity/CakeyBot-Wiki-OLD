# Special Permissions/Conditions

### Overview

Some music commands require special permissions or can only be used in specific instances. This page was designed to help demystify these special cases and list the special permissions and conditions

Most commands require a song to be playing/not paused. Some commands are also unable to be used while a live stream is currently playing. In these cases commands will inform you that they are unable to be used why.

### Disconnect Command

Many users have abused the disconnect command as a way to bypass vote skip restrictions. In order to use the disconnect command you must be in the same channel as Cakey Bot and meet one of the conditions below.

* Have [Server Moderator](https://cakeybot.app/faq.html) permissions
* Have a "DJ" role
* Be the only person in the voice channel

### Skip/Vote Skip Command

By default anyone in a voice channel can skip songs regardless of the number of users in the voice channel. You also have the option to enable "vote skipping" which requires more than 50% of the users in the voice channel to vote to skip the song. If you run the command after you have already voted to skip, it will cancel/remove your vote to skip. There are some cases where you are able to force-skip the currently playing song regardless of the number of votes. In order to do this, you must meet one of the conditions below.

* Have [Server Moderator](https://cakeybot.app/faq.html) permissions
* Have a "DJ" role
* Be the only person in the voice channel
* Be the user who added the currently playing track

### Move Command

This command is blocked for regular users to prevent a user from "stealing" the bot from other users who may be listening to Cakey Bot. In order to move Cakey Bot to a different voice channel, Cakey Bot must either not be playing any music OR the user running the command must meet one of the conditions below.

* Have [Server Moderator](https://cakeybot.app/faq.html) permissions
* Have a "DJ" role

### Play-skip/Remove/Clear Queue

These are normal/generic commands but they can be easily abused by members who are wanting to troll those listening to music. In an effort to prevent trolls from abusing these commands they require at least one of the conditions for the user to be true.

* Have [Server Moderator](https://cakeybot.app/faq.html) permissions
* Have a "DJ" role

### Live Streams

Some commands can not be used while a live stream is playing. If you try to use one of these commands while a live stream is playing you will be notified with an error message. In order to use these commands you will either need to wait until the stream ends or use the `!skip` command to go to the next song in the queue. (or stop playing if the queue is empty)

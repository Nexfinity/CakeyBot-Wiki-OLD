# Changelist - 2021

## 7/25/2021 - TTT Fixes

#### Fixed

* Added a note to `!ttt` games displaying how long until they expire
* Automatically expire deleted `!ttt` games
* Fixed issues with new Twitch Feeds
* Increased ratelimit/cooldown of all moderation commands from 1s =&gt; 2s due to abuse

#### Added

* Added new placeholder `{random:min:max}` Which generates a random number between the min/max. Replace "min" and "max" with a number between 0 and 999,999,999. Note: Your minimum number must be smaller than your maximum number.

## 7/24/2021 - Social Feeds! \(Twitch\)

#### Added

* Released first social feed tracking type! \(Twitch live alerts\)
  * You can configure it on the web dashboard under "Social Feeds" and select the "Twitch Feeds" tab
  * Reddit, RSS, and Youtube alerts are planned
  * Non-premium users are limited to a maximum of 3 feeds per type, premium get unlimited
* Added new `{quote:#channelid}` placeholder. Which will quote the last message in the provided channel. Replace "channelid" with the ID of the channel

## 7/21/2021 - Minor Bug Fixes

#### Fixed

* Users can now view their own warnings without explicitly providing their user id as a parameter in `!warnings`

#### Changed

* Fixed some issues with `!ttt`
* Fixed join/leave DMs

## 7/18/2021 - More Music Fixes

#### Fixed

* Fixed music embed/song request channel buttons not working
* Fixed music not auto-skipping on song end \(again\)

## 7/16/2021 - Music Fixes

#### Fixed

* Fixed Cakey Bot not properly disconnecting when all users leave the voice channel
* Fixed Cakey Bot not automatically skipping to next song when one ends

## 7/15/2021 - Button AFK

#### Fixed

* Upgraded AFK responses to user a button instead of reactions \(More reliable, requires less permissions\)
* Fixed skip message not sending while using music embed/song request channel
* Updated translation strings to latest version

## 7/14/2021 - MAJOR Audit Log Overhaul

#### Fixed

* Fixed music translations/localization
* Fixed an issue where some music titles would mess up the url/link formatting

#### Changed

* Bot settings will now save if Cakey Bot is kicked/removed
* Major audit log overhaul
  * You can now toggle individual audit log events on/off so you can see events that are important to you
  * You can now send individual events to different channels so you can group them by priority or have certain logs public \(or for certain staff ranks\)
  * You can now change the embed color for each event to make them better stand out
  * Re-enabled the voice channel user state event \(shows when users join, leave and swap voice channels\)
  * Added the ability to exclude certain roles or channels from being logged \(This one is a WIP and will be out later tonight\)

## 7/12/2021 - Misc Fixes

#### Fixed

* Fixed word blacklist not working in auto mod
* Updated `!google` command to censor titles/descriptions in non-NSFW channels
* Fixed `!reminder` not be able to accept emoji

## 7/10/2021 - Auto-Updating Localized Timestamps

#### Fixed

* Fixed `!covid` not showing the specified country name on output results

#### Changed

* Converted `!giveaway` and `!remindme` commands to use Discord's new localized relative timestamps \(Auto-updating in each user's timezone\)
* Increased giveaway's max time limit \(1 hour =&gt; 1 day\)
* Updated `!giveaway` to not spam update every 10 seconds \(Cleaner audit logs, more accurate time, and less rate limit issues/delays\)
* Updated `!tempban` and `!tempmute` to also use these new placeholders

#### Added

* Added missing selection dropdown to "help" slash command
* Added the additional premium cakey bots to "invite" slash command

## 7/8/2021 - Auto Mod Improvements

#### Added

* Added custom server-specified word blacklist for auto mod \(web dashboard\)
* Added the ability to whitelist websites/URLs from the website blacklist on auto mod \(web dashboard\)

## 7/7/2021 - Snipe Command Toggle

#### Added

* Added toggle to web dashboard for `!snipe` command \(disabled by default\)

## 7/6/2021 - Advanced Purge Returns!

#### Fixed

* Fixed `!remindme` and `!tempmute` commands
* Fixed `!snipe` command

#### Changed

* Re-enabled advanced purge filters and fixed related issues
  * Added new "Components" filter to delete messages that contain buttons OR selection dropdowns
  * **NOTE:** "Between" and "Until" filters are still buggy and are currently disabled.

## 7/3/2021 - First Weekly Update

#### Changed

* Updated `!setting` command to display information about configuring advanced features
* Split "Announcements" role into 3 roles \(Announcements, Bot News, and Website News\) so you can subscribe to news thats important to you
* Updated `!ttt` AI to block more potential moves
* `!fact` command will now show a drop down to select a fact type instead of provided a random "general" fact if you don't specify a type when running the command
* `!invite` now shows all Cakey bots that can be invited \(Music bots and BETA bot\)
* `!help` now has a drop down menu to easily grab URLs/links to useful pages or documentation for features
* `!rps` command will now show a dropdown menu to select a move if you fail to provide one
* `!snipe` now pulls the message for the current channel instead of the entire server \(this prevents accidentally leaking deleted messages from private channels\)

#### Added

* Added new "General" category to the `!fact` command

## 7/2/2021 - Volume Increase

#### Fixed

* Fixed `{delete}` placeholder

#### Changed

* Max music volume increased to 300%

## 6/29/2021 - Avatar Improvements

#### Changed

* Updated `!avatar` command to provide links to multiple file types and sizes

## 6/28/2021 - Minor Improvements

#### Fixed

* Fixed/updated welcome DM
* Tons of general bug fixes and performance improvements

#### Added

* Added fancy position bar for `!nowplaying` command
* Added DM Feedback poll for server owner when Cakey Bot is removed from a server

## 6/25/2021 - Bug Fixes

#### Fixed

* Fixed an issue where Audit Log wouldn't work when you updated a News channel
* Fixed an issue where custom commands/auto responders would fail if a user provided an invalid `{choose}` placeholder
* Fixed a ton of other misc. bugs/issues. \(Mostly with slash commands\)

#### Changed

* Updated `!banlist` to use pastebin if there's too many users to display in-discord
* Updated `!banlist` command to have an additional optional argument to only output the user IDs with no usernames. \(`!banlist <true/false>`\)
* Added additional check for "UseExternalEmoji" on AFK messages

## 6/22/2021 - TTT Upgrades

#### Changed

* Upgraded `!ttt` AI to actively block player wins

## 6/21/2021 - Music Changes

#### Fixed

* Fixed missing error messages with slash commands for music

#### Changed

* Song titles are now trimmed to 50 characters
* Song titles can now be clicked and link to the original song URL
* Song requester now actually pings/mentions the user
* Updated overall formatting of music strings a bit

## 6/20/2021 - Achievement Banners + Music Upgrades

#### Fixed

* Fixed an incorrect URL while typing `!afk list`
* Fixed an issue where `/afk` wouldn't show your currently set AFK message
* Fixed AFK messages not supporting unicode based text \(like emotes or korean language\)
* Fixed `!skip` vote counts
* Fixed `/remindme` allowing optional parameters
* Fixed check/x emotes on slash commands

#### Changed

* Changed `!search` command description

#### Added

* Added new `!achievement <text>` command which generates a Minecraft achievement using the provided text
* Added new `!clap <text>` command which adds some ![:clap:](https://discord.com/assets/9fa091f676e4451ee5946fed948cb8fe.svg) to your text
* Added new `!xkcd <opt:id>` command which grabs the comic for the provided ID or the latest comic if no ID is provided
* Uploaded new translations for korean and swedish
* Added `!forceskip` and `!fs` as aliases to the `!skip` command
* Added slash commands for music:
  * Including: `/join`, `/play`, `/queue`, `/nowplaying`, `/disconnect`, `/skip`, `/volume`, `/pause` and `/resume`

## 6/18/2021 - Premium Overhaul

#### Fixed

* Fixed an extra `>` bracket that was on ban audit log messages

#### Changed

* Updated `!google` to actually return first google result
* Cryptocurrencies are no longer accepted
* Credit/Debit card is now handled by PayPal \(You don't have to create an account\)
* Stripe credit/debit card is no longer accepted
* PayPal subscriptions will now auto-renew monthly
* Added bulk discount \(If you buy for 11+ servers, you only pay $4/mo per server\)
* Updated FAQ and other related elements to reflect this change
* Added ability to select a custom number of servers \(1-99\)
* Updated premium page to show separate buttons for "PayPal Premium" and "One-Time PayPal Donations"
* "Next Charge" will now show "Expires On" or "Renews On" depending on the type of payment
* Current servers will now display which of your premium plans is applied to it and when that plan expires/renews
* Premium subscriptions now show the source type the payment came from
* PayPal subscriptions now automatically apply your premium subscription after purchase

#### Added

* Added `!snipe` command

## 6/17/2021 - Web Optimizations

#### Fixed

* Fixed hover tooltip for premium custom join/leave banners \(previously used the query tooltip\)

#### Changed

* Optimized several web dashboard pages to improve page load speeds

## 6/16/2021 - New Placeholder \(Buttons!\)

#### Changed

* Updated `!rolelist`, `!channellist` and `!emojilist` commands to use pastebin if there's too many to list in a Discord message

#### Added

* Added `!persistrole` as alias to `!persistentrole`
* New placeholder! Add link buttons on custom commands/auto responders `{linkbutton:(text)[url]}`. Read more [here](https://docs.cakeybot.app/setup/placeholders-variables#link-url-buttons).

## 6/15/2021 - Web Dashboard + Locale Updates

#### Fixed

* Fixed an issue where the Premium page would not load if you hadn't selected a server yet

#### Changed

* You can now visually see which of your servers have premium and beta applied without having to click on them individually
* Also, all new translation work has been pushed live

## 6/14/2021 - Accessibility Improvements & Bug Fixes

#### Fixed

* Fixed an issue where `!play` would throw an "unknown" error in addition to the original error message if Cakey Bot was unable to join the voice channel
* Fixed translations that would break after the first move in TTT \(This should also fix translation issues with other button/interaction related components\)
* Fixed a bug where image manipulation commands would sometimes silently fail if they failed to download an image to modify
* Fixed `!suggestion` embed error colors not being red
* Fixed an issue where you couldn't use numbered choose/choice placeholder lists if you didn't include the default unnumbered list

#### Changed

* Improved accessibility with toggling modules on the web dashboard and viewing their current status/state
  * Greatly increased the border width so the color is easier to identify
  * Changed button text "Click to Toggle" to "Click to Enable/Disable"

#### Added

* Added padding below toggle module panels so they don't clip behind the footer

## 6/12/2021 - New Placeholder

#### Fixed

* Fixed an issue where you couldn't edit or clone custom commands/auto responders that contained backticks on the web dashboard

#### Added

* Added a new placeholder `{messagelink}` which displays a Discord link/url to the original command/message that triggered the response

## 6/11/2021 - QOL Changes

#### Changed

* Updated Cakey Bot's invite to no longer request administrator while inviting
  * [https://discord.com/oauth2/authorize?client\_id=288163958022471680&permissions=2654334038&redirect\_uri=https%3A%2F%2Fdocs.cakeybot.app%2F&response\_type=code&scope=bot+applications.commands+identify+guilds](https://discord.com/oauth2/authorize?client_id=288163958022471680&permissions=2654334038&redirect_uri=https%3A%2F%2Fdocs.cakeybot.app%2F&response_type=code&scope=bot+applications.commands+identify+guilds)
* Updated website navbar buttons to be consistent across all pages \(Previously colors were inverted on some pages\)
* Pushed Korean and Swedish translations live

## 6/7/2021 - Temporary Actions

#### Fixed

* Reminders & temporary moderation actions are now working again

#### Changed

* Re-added "remindme" as a slash command

#### Added

* Added `!animequote` command
* Added `!petpet <opt:user>` command
* Added `!lolice <opt:user>` command
* Added `/afk` and `/unafk` slash commands
* Added two new placeholders!
  * You can now use the `{chance:X}` placeholder to randomly send a response \(or not :P\)
    * You can check out more details on our documentation here: [https://docs.cakeybot.app/setup/placeholders-variables\#response-chance](https://docs.cakeybot.app/setup/placeholders-variables#response-chance)
  * You can now use the `{react:X}` placeholder to add basic reactions to your responses! `[Premium Only]`
    * You can check out more details on our documentation here: [https://docs.cakeybot.app/setup/placeholders-variables\#reactions](https://docs.cakeybot.app/setup/placeholders-variables#reactions)

## 6/6/2021 - TTT Fixes

#### Fixed

* Fixed `!ttt` colors
* Fixed an issue where `!ttt` games could throw an incorrect "expired" error message when there's tons of games going on

#### Changed

* `!ttt` now keeps the game board displayed after it has finished
* Slightly improved AI to target winning tiles \(Still need to add the AI actively blocking player wins, but slightly better than pure randomization\)

#### Added

* Added new image manipulation command `!pride <opt:user>`, it will apply a rainbow overlay over your profile picture or the provided user's profile picture.

## 6/5/2021 - Bug Fixes

#### Fixed

* Fixed emoji count for `!serverinfo` command

#### Changed

* Updated custom command / auto responder rate limit to just drop/ignore spam instead of delaying/queueing it
* Limited `!calculator` output to 2k characters

## 6/3/2021 - Feature Requests

#### Changed

* Added usage info for `!quote` command when incorrect parameters are provided
* Updated `!warnings` to accept user id OR user object. \(This allows you to view warnings of users who are no longer in the server\)

## 6/2/2021 - Calculator

#### Added

* Added new `!calculator` command, should be fairly straightforward

## 5/31/2021 - Stage Channels!

#### Added

* Discord recently added stage channels that splits speakers and audience into two groups. All you have to do is make Cakey Bot a stage moderator and it will play your favorite music in stage channels too! Note: For the moment, sometimes you also have to right-click Cakey Bot and click "Invite to Speak"
  * How to add stage moderators: [https://support.discord.com/hc/article\_attachments/1500007375362/modifying\_stage\_moderators\_flow\_gif.gif](https://support.discord.com/hc/article_attachments/1500007375362/modifying_stage_moderators_flow_gif.gif) 
  * Stage channels FAQ: [https://support.discord.com/hc/en-us/articles/1500005513722](https://support.discord.com/hc/en-us/articles/1500005513722)

## 5/30/2021 - Slash Commands V2

#### Fixed

* Fixed some broken stuff with existing slash commands

#### Changed

* Updated some slash commands to be ephemeral \(This means they'll show the results only to you, so you can use them without spamming chat!\)

#### Added

* Added tons of new slash commands

## 5/29/2021 - Buttons!!

#### Added

* Added "Open Link" button to `!avatar`
* Added "Flip Again" button to `!coinflip`

## 5/28/2021 - Equalizer Presets

#### Added

* Added new command! `!eqpreset <preset>` This will allow you to automatically apply a preset equalizer to the song your listening to. 
  * Current presets are: `lowpass, highpass, flat, extrabass, extratreble, bassandtreble` \(Thanks @Captain Ibblesworth \)

## 5/6/2021 - Stickers!

#### Fixed

* Fix tons of misc. bugs, errors, and fatal crashes in Cakey Bot.

#### Added

* Added Stickers check to auto mod
* Add error message when `!video` returns no results

## 5/1/2021 - Music Fixes

#### Fixed

* Pushed a potential fix for music

#### Added

* You can now toggle 'persistent mutes' on the web dashboard. This will automatically reapply mute roles to users if they try to leave/join to bypass mutes

## 4/28/2021 - Among Us Fix

#### Fixed

* Fixed `!amongus` sending as a static image instead of an animated gif

## 4/3/2021 - Delete Placeholder Upgrade

#### Changed

* Updated `{confirmdelete}` placeholder cooldown \(30s=&gt;60s\)

## 3/25/2021 - Audit Log Fixes

#### Fixed

* Fixed "Message Deleted" audit log event not correctly preserving deleted images.

## 3/21/2021 - Custom Command Args/$N

#### Added

* Custom Command Arguments/$N variables are now released. You can read up on them here: [https://docs.cakeybot.app/setup/placeholders-variables\#arguments-usdn-variable-custom-commands-only](https://docs.cakeybot.app/setup/placeholders-variables#arguments-usdn-variable-custom-commands-only)
  * This placeholder is very new and could be buggy, please report any problems!

## 3/20/2021 - Choose & Choice Placeholders

#### Changed

* Updated advanced placeholders to be case-insensitive \(Originally only basic placeholders were case-insensitive\)

#### Added

* Implemented Choice and Choose advanced placeholders! You can read up on how to use these here: [https://docs.cakeybot.app/setup/placeholders-variables\#choose-and-choice](https://docs.cakeybot.app/setup/placeholders-variables#choose-and-choice)

## 3/14/2021 - Music Updates

#### Fixed

* Fixed default volume not being set when adding playlists

#### Changed

* Updated new dashboard audit log to be localized \(multi-language\)

#### Added

* Added max song length to dashboard
* Added word blacklist to dashboard for music titles \(To auto-blacklist ear rape or similar\)

#### Removed

* Removed the `!playskip` command.
* Removed useless code from `!search` \(Checking for playlist loading, will now display no results error\)

## 3/11/2021 - Dashboard Logging!

#### Added

* Added dashboard audit log! You can now keep an eye on what settings your server admins have been changing recently.
* Added support for `spotify:track:<trackid>` formats in music queueing.

## 3/9/2021 - Auto Mod Updates!

#### Added

* You can now add/remove custom blacklisted words!
  * Website blacklist/whitelist will be added soon as well.

## 3/4/2021 - Soundbites!

#### Added

* Added new `!soundbites <name>` command!
  * Current sound bites: `among-us, bruh, deja-vu, discord-call, discord-join, discord-notify, error, fail, got-you, haha, hello-there, here-comes-the-money, law-and-order, ok, oof, run, sad-violin, sexy-sax, stonks, taco-bell, trollolo, what-are-you-doing-in-my-swamp, windows-xp, wow, you-what`

## 3/1/2021 - Persistent Roles QOL Changes

#### Changed

* Disabled automatic persistent mutes on `!mute`
  * `!unmute` will continue to remove persistent roles to undo any current ones

#### Added

* Add dropdown to delete persistent & temporary roles \(add clear all button too\)

## 2/26/2021 - Bug Fixes + Premium Banners

#### Fixed

* Fixed `!image` command \(+related slash command\)
* Fixed profile images not working when user doesn't have one \(Affects multiple commands\)
* Fixed incorrect text on `!help` commands
* Multiple bug fixes

#### Changed

* Deprecated the `!settings` command. All configurations must be done via the Web Dashboard now.
  * `!setting prefix <new prefix>` will continue to work.

#### Added

* Added custom join/leave banner background images for premium users

## 2/14/2021 - AFK Updates

#### Added

* Added the ability to clone Custom Commands and Auto Responders
* Added the ability to view a list of AFK users in the web dashboard
  * Includes a button to delete/remove selected AFK messages on users

## 2/13/2021 - General Enhancements

#### Fixed

* Fixed `{dm}` placeholder being able to be used by non-premium users
* Fixed an issue where Cakey Bot would incorrectly mention multiple users/channels/roles in custom commands

#### Changed

* Improve strictness when censoring certain text in non-NSFW channels.
* Updated links in bot \(Donate =&gt; premium\)
* Added up-sale info on certain commands for Premium
* Updated premium info on docs/faq
* Updated web dashboard URLs in Cakey Bot
* Implemented roles on not/require placeholders

## 2/7/2021 - Better Auto Mod

#### Fixed

* Fixed incorrect error message when Cakey Bot fails to load a music track
* Improved error handling in auto mod

## 2/5/2021 - Premium Enhancements

#### Changed

* Redesigned Premium website page
  * Updated layout to be more responsive
  * Added BTC and ETH as payment options
  * Added FAQ questions/info
  * Added pricing
  * Updated style of premium perks to stand out more/easier to read

## 2/3/2021 - QOL Fixes

#### Fixed

* Fixed an issue where Cakey Bot would add duplicate entries to web dashboard music queue when skipping to next song
* Fixed an issue where "Temporary Actions" would show every server's actions on the web dashboard

#### Changed

* Cakey Bot will now send a persistent message when it has disconnected from a voice channel due to no users
* Added up to 2 retry attempts for all Cakey Bot temporary actions \(tempmute/tempban\) & reminders.

#### Added

* Added double quotation marks to the `!dehoist` command
* Added dedicated page to customize music on web dashboard

## 1/31/2021 - Music bug fixes

#### Fixed

* Fixed an issue where clearing the queue via Music Embed/Song Request would not skip the current song playing
* Fixed an issue where loop would fail without an error message if there was an invalid track state
* Fixed an issue where typing an incorrect channels/roles in `!settings` would cause the command to fail silently

## 1/29/2021 - Music seek improvements

#### Fixed

* Improved formatting for `!ff`, `!rewind` & `!seek` commands to better represent how far the song has adjusted.
* Added usage info when giving incorrect time values on `!seek`.
* Updated how Cakey Bot joins a channel. Should fix the issue where Cakey Refuses to join.

## 1/24/2021 - UX Improvements & Bug Fixes

#### Fixed

* Fixed typo and added missing commands on the commands list page
* Fixed Auto Message page not loading correctly
* Fixed tons of various music bugs including playback issues, typos, and incorrect/missing error messages.
* Fixed vote skips not showing the correct number of remaining votes required.

#### Changed

* Premium-Only features are now shown to everyone but are disabled for non-premium
* Placeholder and Documentation buttons now open in new tabs
* Updated Auto Mod to use a separate channel for logging instead of using Audit Log channel
* Censored text in `!lyrics`

#### Added

* Added option to select Auto Mod log channel
* Added buttons to Announcements to automatically set messages to banners or clear the message

## 1/17/2021 - Advanced Purging

#### Fixed

* Fixed an issue where Cakey Bot would delete a different amount than expected/specified

#### Changed

* Updated required user permissions for `!purge` \(Administrator =&gt; ManageMessages\)

#### Added

* Re-enabled advanced purge filters
  * Also added documentation for this [here](../tools-and-utilities/moderation.md#advanced-purge-filters).
  * Added pastebin message logs for advanced purges
  * Added aliases for common typos on types
  * Audit log for delete now displays the original specified amount to help remove confusion

## 1/15/2021 - Generic Bug Fixes

#### Fixed

* Fixed emoji command not displaying info/results
* Fixed commands that would not display due to excessively long text
* Fixed `!video` command and video slash command

## 1/14/2021 - Song Request Bug Fixes

#### Fixed

* Fixed \#songrequest controls not properly clearing the song queue
* Fixed formatting for queue items in \#songrequest channels
* Made even more fixes to music playing states, connections and disconnects

#### Added

* Add new `!report <user> <reason>` command \(setup via web dashboard\)

## 1/12/2021 - Addition Dashboard Info

#### Added

* Added a web dashboard page to view all active persistent roles
* Added a web dashboard page to view all current temporary bans & temporary mutes

## 1/11/2021 - Music Improvements

#### Fixed

* Fixed massive bug where music would stop moving on to next song when a song ended

#### Added

* Added `.M4A` file support to music

## 1/10/2021 - Even More Bug Fixes

#### Fixed

* Fixed an incorrect error message when trying to "resume" a non-paused song
* Fixed an issue where base64 en/decode slash commands wouldn't send the reply
* Fixed an issue where R-Rated gifs would cause the `!gif` command to fail
* Fixed music incorrectly matching on invalid Spotify URLs
* Fixed numerous issues with music player states
* Fixed `!fact` command
* Made auto responder and custom commands case-insensitive
* Removed `!discrim` command

## 1/4/2021 - Tons 'O Bug Fixes

#### Fixed

* Fixed numerous issues with Cakey's \#song\_request channel
* Fixed issues relating to `!loop` and `!skip`
* Updated old website URLs to reflect the new ones
* Updated `!announce` command to require "ManageMessages" instead of "ManageServer"
* Fixed an issue where `!qoute` would fail to quote large messages
* Fixed an issue where `!quote` would fail if you tried to quote a file/image
* Updated music queue in \#song\_request to automatically revert to default if the player state is invalid 
* Updated `/remindme` to check for null users when Discord sends incomplete data

## 1/1/2021 - Premium Subscriptions

#### Added

* Premium subscription options, with perks:
  * Higher Music Queue Song limit \(50 =&gt; Unlimited\)
  * Load Larger Music Playlists \(50 =&gt; Unlimited\)
  * Access to `{dm}` placeholders in Custom commands/Auto Responder
  * Custom `!query` Background Banner Images
  * * More Coming Soon

.


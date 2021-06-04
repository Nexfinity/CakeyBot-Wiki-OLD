# Changelist - 2021

## 6/3/2021 - Feature Requests

#### Changed

* Added usage info for `!quote` command when incorrect parameters are provided
* Updated `!warnings` to accept user id OR user object. \(This allows you to view warnings of users who are no longer in the guild\)

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

## 2/7/2021

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
* Fixed an issue where "Temporary Actions" would show every guild's actions on the web dashboard

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
  * Also added documentation for this [here](tools-and-utilities/moderation.md#advanced-purge-filters).
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

*  Add new `!report <user> <reason>` command \(setup via web dashboard\)

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
  * + More Coming Soon


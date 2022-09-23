# Auto Responder

## Overview

This feature allows you to set up custom trigegrs that Cakey Bot can automatically respond to. For example, you can make Cakey Bot respond to messages such as `wot` with a link to a funny gif. You can also set some flags to determine what types of messages Cakey Bot will respond to.

## Setup

{% hint style="warning" %}
You will need **`Manage Server`** or **`Administrator`** permission to manage servers and custom commands.
{% endhint %}

1. Login to the web dashboard on the [main website here](https://cakeybot.app/dashboard/public).
2. Click on the server you want to edit custom commands on.
3. Go to the "Auto Responder" page.
4. You can then create, delete, and edit any responses on this page. You can get an overview of any flags that are available below.&#x20;

## Flags

* Exact Match
  * Default behavior, looks for exact match strings
* Contains
  * Will search the entire message to see if it contains this string/trigger
* Starts With
  * Will check to see if the message begins with this string/trigger
* Ends With
  * Will check to see if the message ends with this string/trigger
* Contains Files
  * Will check to see if the message contains any files/attachments. (i.e. documents, images, videos)
* From Webhook
  * Will check to see if the message was sent by a webhook
* Contains user mention
  * Will check to see if the message contains a user mention
* Contains channel mention
  * Will check to see if the message contains a channel mention
* Contains role mention
  * Will check to see if the message contains a role mention
* Wildcard Contains
  * Will search the entire message to see if it contains this string/trigger while allowing you to match with wildcards:
    * **`*`** - Matches any number of characters
    * **`?`** - Matches a single character
      * If you need to have a literal question mark in the trigger, you can escape it using a backslash: `\?`

{% hint style="warning" %}
**Note:** When using the "Contains Files", "From Webhook", and "Contains X mention", the "Command" field is still required. However, it is not used to actually trigger the auto response. It's purely a cosmetic property.&#x20;
{% endhint %}

## Limitations/Restrictions

* You can't have duplicate tags with the same name
* Auto Responders are also limited to Discord's message character limit
* Messages sent by bots or webhooks will be ignored

## Placeholders/Variables

Auto Responder will work with BOTH **Basic Placeholders** & **Advanced Placeholders**. Placeholders can be included in the response section and can modify the behavior/output of the response. You can find the list of supported placeholders [here](../other-misc/placeholders-variables.md).

## Using Emoji/Emotes in Responses

Emoji/Emotes CAN be used in Custom Commands. However, it requires slightly more work due to how discord parses emotes. Normally in Discord, you could just type `:lel:` or `:smile:` to get an emote, however in Cakey Bot, neither of these will work. In order to get valid emojis you have to send the emojis in discord but place a backward slash in front of it to get the emote's full ID. Like so: `\:lel:` or `\:smile:` which will produce these results: `<:lel:408424717217693717>` or for Unicode emoji: `😄` . Once you have the full emoji id or the raw Unicode output, you can paste these into Cakey Bot's web dashboard and they should work as long as Cakey Bot is in a server that has that custom emote in it.

{% hint style="info" %}
It is worth noting that Cakey Bot can use emojis in between servers (similar to nitro users). So if you have an emoji in Server #1, you can use that emoji in a response for Server #2 if Cakey bot is in both of those servers.
{% endhint %}

## Using Images in Responses

To use images in responses, you can simply just type the image URL/link like you would in a normal message. If you have the file on your local machine/PC but no URL/link, you can upload it to an image hosting website (such as [Imgur](https://imgur.com/upload)) and paste the URL they provide into the response. Cakey Bot should automatically embed the image in Discord's client if it's a valid URL/image.

## Custom Embeds

{% hint style="warning" %}
Using custom embeds on responses is a [**Premium Only**](https://cakeybot.app/premium.php) feature.
{% endhint %}

You can include an optional embed on responses by following the steps below:

1. Follow the instructions at the top of this page to sign in to the dashboard.
2. Use our [custom embed editor](https://cakeybot.app/dashboard/public/embed-editor) to design your embed.
3. Copy your browser URL or click the "**Get Data Link**" button in the dropdown menu and copy the URL from there.
4. Create an auto responder like you normally would and paste the URL you copied in the last step into the **Embed URL** text field.

## Bulk Import/Export

### Limitations/Guidelines

* File **MUST** be in CSV format.
* File **MUST** be formatted with all of the required columns.
* Additional/extra columns will be ignored.
* `Command` & `Response` fields **MUST** be [Base64 encoded](https://www.base64encode.org/).
* Any fields that have too many characters will be trimmed. Column limits:
  * **Command:** 200 characters (before base64 encoding)
  * **Response:** 2,000 characters (before base64 encoding)
* Any fields that are not [Base64 encoded](https://www.base64encode.org/) or exceed the character will NOT work after importing.
* Bulk importing can **NOT** be canceled or reversed once started.
* Any broken commands will have to be individually deleted or fixed _after_ the import is finished.
* There is a limit of **500 commands** per bulk import.

### What is Base64 encoding?

Base64 is a group of binary-to-text encoding schemes that represent binary data in sequences of 24 bits that can be represented by four 6-bit Base64 digits. This sounds complicated, however, it's EXTREMELY easy to convert text to and from Base64 encoding. There are tons of online tools just like [this one](https://www.base64encode.org/) that automates the entire process just by you pasting your text in it.

### How can I Base64 encode a string?

If you using the tool linked above, all you have to do is paste your text in the top text input and it'll convert it into Base64 encoding and display it in the second text box. You can also convert Base64 back into text by using [this tool](https://www.base64decode.org/) OR by selecting "Decoding" at the top of the page and using the same process.

{% hint style="info" %}
Note: The convert file process on this page converts the ENTIRE raw file itself and not just the contents of the file. This means you can NOT use the convert file process when converting for Cakey Bot.
{% endhint %}

### How can I convert a ton of lines/rows of data?

This is easy as well! Using the same Base64 encoding tool linked above you can simply paste all of your data (each row on a new line) and simply check the `"Encode each line separately (useful for when you have multiple entries)."` option. This will then convert each line individually rather than treating every single line as a single blob of text.

{% hint style="warning" %}
Note: If you are doing this for a ton of data, you can only process/paste one column of data at a time. If you try to copy multiple columns in the spreadsheet and paste all of them at once it'll merge the rows together as a single string.
{% endhint %}

### What do the columns/fields and their values mean?

The template CSV file and bulk exported CSVs will have a few different columns with various restrictions. These are explained below:

* Status
  * This determines whether or not the command/response is "enabled" or "disabled"
  * Acceptable values:
    * 0 - Disabled
    * 1 - Enabled
* Command
  * This is the command/trigger phrase for a response.
  * It must be Base64 encoded and be less than 200 characters before Base64 encoding.
* Triggers
  * This is an internal value that determines whether or not a command is an Auto Responder or a Custom Command. The import script will ignore any value you put here and force set it internally.
  * Acceptable values:
    * 1 - Custom Commands
    * 2 - Auto Responders
* Flags
  * These are only used for Auto Responders, they map directly to the Auto Responder flags.
  * Acceptable values:
    * 1 - Exact Match
    * 2 - Contains
    * 3 - Starts With
    * 4 - Ends With
    * 5 - Contains Files
    * 6 - From Webhook
    * 7 - Contains user mention
    * 8 - Contains channel mention
    * 9 - Contains role mention
    * 10 - Wildcard Contains
* Response
  * This is the response phrase for a trigger/command.
  * It must be Base64 encoded and be less than 2,000 characters before Base64 encoding.
* Embed
  * This is an optional field for responses that use a Cakey Bot custom embed. Embeds can only be used by Premium Servers regardless if a value is set here or not.
  * The URL must start with [https://cakeybot.app/dashboard/public/embed-editor?data=](https://cakeybot.app/dashboard/public/embed-editor)

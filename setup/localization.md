# Localization

## Localization \(Multi-Language\)

{% hint style="info" %}
This is a new feature and new translations are constantly being added to the bot. This means some strings/phrases may not be translated yet especially for features that have been added recently.
{% endhint %}

Cakey Bot supports 10 different languages. Language can be changed per-guild and will apply for every user in that guild. You can change the guild's language from our web dashboard. Currently supported languages are listed below:

* English
* Dutch
* German
* Korean
* Greek
* Swedish
* Turkish
* Italian
* Arabic
* Romanian

We are adding more languages and you can contribute via our crowdin project located [here](https://crowdin.com/project/cakey-bot). Once a language is "completed" on crowdin it will be added as a supported language.

{% hint style="warning" %}
If you plan to add to our crowdin, please keep these guidelines below in mind.
{% endhint %}

1. Please do not insert unnecessary punctuation into strings, unless it is required for that language
2. Any string that contains \` symbols, please leave them in the same position and don't remove them. Nor change them to other symbols like ' or ", these are used to highlight certain text or to prevent "@everyone" pings from being used/abused
3. If you encounter any placeholders like {0}, {1}, etc, keep them in the string. These are automatically replaced in the bot with text so `Requested by {0}#{1}` when used in the bot will be replaced with like `Requested by MrCake#1337`
4. If you need more context/info about how/where a string is used to provide an accurate translation, just leave a comment on the string and a reviewer will provide further info/screenshots


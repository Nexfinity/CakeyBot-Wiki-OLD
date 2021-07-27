# Support Ticket System

{% hint style="warning" %}
Make sure that Cakey Bot has the **`Manage Channels`** permission and that the Cakey Bot's role is _above_ the support staff role.
{% endhint %}

## Overview

Cakey Bot's support ticket system allows your users to make tickets and get 1 on 1 support from your support team. You can easily manage tickets via Discord's button system and even save transcripts of the ticket history.

## Setup

1. Login to our [web dashboard](https://cakeybot.app/dashboard/).
2. Go to "Support Tickets" [here](https://cakeybot.app/dashboard/public/tickets).
3. Configure your desired settings

**Support Staff Role:** Selecting a support staff role will automatically allow users with the selected role to view/access all support tickets. If you do not select a support staff role only Administrators will have access to tickets.

**Transcript Channel:** Selecting a transcript channel will unlock the ability to save ticket history to the selected channel. Which will allow staff to review old closed/deleted tickets.

## Usage

Once you have enabled and configured support tickets via the web dashboard your users can start making tickets using the `!new <description>` command. 

{% hint style="info" %}
Note: The issue description is optional and a default reason will be filled in if a user does not provide one.
{% endhint %}

You do _not_ need to make/set up a support category, Cakey Bot will automatically generate the correct channels and permissions if Cakey Bot has access to do so.

Once a user has closed a ticket, Cakey Bot will send an embed with three different options:

* **Transcript:** Selecting this will save the contents of the ticket to a text file and uplaods it to your transcript channel.
  * If this option is disabled, you will need to configure your transcript channel on the web dashboard.
* **Re-Open:** This option will re-open the ticket to allow the user to provide more information or to ask more questions.
* **Delete:** This option will delete the ticket and clears the channel history.
  * This option does NOT automatically save a transcript.


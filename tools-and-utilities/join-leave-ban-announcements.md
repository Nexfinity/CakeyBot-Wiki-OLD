# Join/Leave/Ban Announcements

## Overview

Cakey Bot can automatically post custom messages when users join/leave or are banned. You can have Cakey Bot announce for one or all of these events and set different messages (or image banners) for each event.

## Setting A Message

You can set/modify messages and the announcement channel via our [web dashboard](https://cakeybot.app/dashboard/public/). Just log in, select a server, and head on over to the "Announcements" page. Once here you can select a channel as well as setting the message content. You can set a message for any one of these events, some of them or all of them.

{% hint style="info" %}
In order to have Cakey Bot send the messages, you will have to set a channel for Cakey Bot to post to. You can find more information about this below.
{% endhint %}

## Enable/Disable Announcements

In order to start posting announcements, you will need to designate a text channel as the announcement channel. You can do this by setting it in the [web dashboard](https://cakeybot.app/dashboard/public/). In order to disable announcements, simply select "none" instead of a channel name in the dropdown.

{% hint style="warning" %}
Cakey Bot will need access to Send/Read messages in the channel you designate for announcements. Cakey Bot may also require **`Use External Emoji`** permission if you include external emojis in the announcement messages.
{% endhint %}

## Image/Banner Announcements

You can also use a fancy banner picture for your join/leave messages too! In order to set an image banner as your join/leave message just type "banner" instead of a message. You can also choose a custom banner image to use if you have a premium subscription.

{% hint style="danger" %}
Currently, you can not set a banner for ban messages.
{% endhint %}

![](<../.gitbook/assets/SS5 (4).JPG>)

{% hint style="warning" %}
Note: If you choose to use a banner image, you will not be able to use/apply custom text or placeholders alongside it.
{% endhint %}

## Variables

Announcements will work with all **Basic Placeholders**. You can find the list of supported placeholders [here](../setup/placeholders-variables.md).

{% hint style="warning" %}
Announcements will **NOT** work with the **Advanced Placeholders**.
{% endhint %}

# Filters, Equalizer & Presets

## Equalizer (+ EQ Presets)

You can set custom equalizer bands using the `/equalizer <band> <value>` command. There are 15 bands (**0-14**) that can be changed. gain is the multiplier for the given band. The default value is **0**. Valid values range from **-0.25** to **1.0**, where **-0.25** means the given band is completely muted, and **0.25** means it is doubled.

You can also use our presets for those of you who just want a quick and easy solution by typing `/eqpreset <preset>`. Our presets include:

* Lowpass
* Highpass
* Bandpass
* Flat
* Extrabass
* Extratreble
* Bassandtreble

## Customizable Music Filters

{% hint style="warning" %}
Filters require a premium subscription to use due to increased CPU usage requirements.
{% endhint %}

You can also set custom filters on your music using the `/filter <name> <options>` command. If you'd like to revert these changes you can also type `/filter <name> reset`. If you run the `/nowplaying` command, it will show all of your currently applied filters as well. Our possible filters include:

* Distortion
  * Sin Offset - Default: 1
  * Sin Scale - Default: 1
  * Cos Offset - Default: 1
  * Cos Scale - Default: 1
  * Tan Offset - Default: 1
  * Tan Scale - Default: 1
  * Offset - Default: 1
  * Scale - Default: 1
* Karaoke
  * Level - Default: 1
  * Mono Level - Default: 1
  * Filter Band - Default: 200
  * Filter Width - Default: 100
* Lowpass
  * Smoothing - Default: 20
* Rotation
  * Frequency - Default: 1
* Timescale
  * Speed - Default: 1
  * Pitch - Default: 1
  * Rate - Default: 1
* Tremolo
  * Frequency - Default: 2
  * Depth - Default: 0.5
* Vibrato
  * Frequency - Default: 2
  * Depth - Default: 0.5

{% hint style="info" %}
All filters have a minimum value of **0.01** and a maximum value of **5.**
{% endhint %}

## Music Filters

{% hint style="warning" %}
All preset music filters require a [premium subscription](https://cakeybot.app/premium.php) to use due to increased CPU usage requirements.
{% endhint %}

* **Nightcore** is a special effect that speeds up the music while applying a slightly higher pitch to it. You can toggle this preset with the `/filterpreset nightcore` command.
* **Vaporwave** is a special effect that slows down the music while applying a slightly lower pitch to it. You can toggle this preset with the `/filterpreset vaporwave` command.
* **8D Audio** is a special effect that 'rotates' the music to provide a more interesting listening experience. You can toggle this preset with the `/filterpreset 8d` command.
* **Reverb** is a special effect that makes use of echo to create a more dynamic sound space for a song. You can toggle this preset with the `/filterpreset reverb` command.
* **Bass Boost** is a special effect that boosts the overall bass for the song. You can toggle this preset with the `/filterpreset bassboost` command.

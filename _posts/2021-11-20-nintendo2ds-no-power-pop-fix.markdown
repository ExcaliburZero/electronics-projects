---
layout: post
title: Fixing Nintendo 2DS that wouldn't power on
name: nintendo-2ds-no-power-pop-fix
image: /assets/2021/11/20/after.jpg
description: I fixed a Nintendo 2DS that would not power on.
date: 2021-11-20
tags: [Nintendo 2DS, Repair, Screen Replacement]
---

{% assign assets_dir = "/assets/2021/11/20" %}

Recently I've been learning more about how to mod and repair Nintendo handhelds, however I've mostly been working with older hendhelds like the GameBoy Advance and GameBoy Color. So to try something a bit different and possibly more challenging I decided to try repairing a more recent handheld from the DS / 3DS line.

While looking around on Ebay I found a listing for a broken Nintendo 2DS that looked like it might be an interesting candidate:

>  Nintendo 2DS Handheld Console Black & Red NO Power For Parts Or Repair - Condition is For Parts or Not Working - Shipped with USPS 
>
> ** SOLD AS IS - The Console will NOT power on and I do not know why so I am selling this AS IS for a low price. The photos show the item you will receive -  NO RETURNS **

A powering-on issue sounded like an interesting challenge, so I decided to give it a try.

The handheld was in fairly decent condition. The plastic shell had some scratches, and there was one notable scratch on the touch screen. It also had a large sticker on the back, which I had to remove using isopropyl alcohol before I could do any troubleshooting that required opening the device.

## Troubleshooting

First I tried charging the Nintendo 2DS in case there was a battery-related issue. The orange charging light came on as expected. I then tried turning the device on and the blue power led turned on, but after a few seconds the speakers made a "pop" sound and the power led turned off.

I also took out the battery and tested it with the "voltage" setting of my multimeter, and it gave a reading of `4.06 V`. So the battery seemed not to be dead or low.

After doing some searching online I found some YouTube videos that mentioned that the 2DS turning off after a few seconds with a "pop" sound could be due to a loose screen backlight ribbon cable.

I opened up the 2DS to give this fix a try. Upon opening it I found that the ribbon cable for home button was disconnected, so I reseated it and tried powering the 2DS back on, but the issue still persisted.

I then tried reseating the ribbon cables for the screens and turning the device on (as the videos I found recommended), but the issue still persisted.

I also asked on "The Retro Future" Discord channel's "#repair-help" channel to see if anyone there had some recommendations for how to troubleshoot the issue.

italianretroguy recommended that I try checking the wifi module, so I tried reseating it, but the issue unfortunately still persisted.

I ended up trying a few iterations of unseating some of the screen ribbon cables, and eventually I tried it with the 2 LCD ribbon cables unseated, but the backlight and touchscreen cables still seated and when I powered the device on the screen lit up but was very cracked. (But no longer "popped" and turned off)

Progress!

![Photograph of the front of the red and black Nintendo 2DS. The screen is backlit, but mostly black with some bright white cracks spreading out forn the top of the top screen going all the way to the bottom of the bottom screen.]({{ "/broken_screen.jpg" | prepend: assets_dir | absolute_url }})

With this evidence I was pretty sure that the screen was broken and needed to be replaced.

Besides the screen, the device was working well. I could hear sound from the speakers, and using the d-pad, buttons, and joystick all seemed to yield the correct audio cues.

## Screen replacement

I bought a replacement screen for the 2DS off of Amazon. It arrived in good condition.

![Photograph of the Nintendo 2DS replacement screen with the protective film still covering the screen.]({{ "/replacement_screen.jpg" | prepend: assets_dir | absolute_url }})

At first I tried removing the 2DS's motherboard and placing it on the back of the replacement screen to check if the replacement screen worked before installing it into the shell. However, I couldn't get the ribbon cables to line up right without the shell keeping everythng in place, so I decided to just install the screen and hope it works.

I carefully removed the broken screen from the front shell by gently bending the shell back and forth until the grip of the screen gasket was weak enough to remove the screen.

I removed the screen gasket from the broken screen and applied it to the replacement screen. This was definitely the most annoying step in the replacement process, since it took me quite a few tried to get the gasket to line up properly.

After applying the gasket, I installed the replacement screen back into the shell, put the mortherboard back in, and plugged in all the ribbon cables.

I then powered on the 2DS and the replacement screen worked! Yay!

![Photograph of the front of the, now working, red and black Nintendo 2DS. The screen is lit up and showing the main menu with the game Bravely Second loaded.]({{ "/after.jpg" | prepend: assets_dir | absolute_url }})

## Misc

After confirming that the screen worked I took out the buttons, membranes, etc. to clean them. I wasn't able to get the sides of the buttons as clean as I wanted them, but they were good enough. I also cleaned the contacts on the motherboard for the buttons and d-pad using IPA and a Q-tip.

I did some checks to confirm that the different parts of the device were really working.

* Buttons
* D-pad
* Joystick
* Volume slider
* Headphone jack
* Microphone
* Sleep switch
* Touch screen
* Cartridge reader
* SD card reader
* Wifi module

There were a few things I didn't check, because I wasn't sure offhand how to quickly test them (local wireless and IR transmitter/reciever). But all the things I did test seemed to be working fine.

## Conclusion

Overall the repair was interesting. There was some information online to help get me on track as to what the issue could be, but the issue wasn't that easily fixable problem that had the same symptoms. I ended up having to do some troubleshooting to discover what the actual issue was, but I was able to successfully troubleshoot the issue.

The screen replacement wasn't too difficult, with the exception of applying the gasket to the replacement screen.

I'm glad that I did the repair, since I ended up learning a lot more about the 2DS and I now feel more confident in doing handheld repairs.

*[IPA]: Isopropyl alcohol
*[IR]: Infrared
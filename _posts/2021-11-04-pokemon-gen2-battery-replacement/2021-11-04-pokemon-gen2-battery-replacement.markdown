---
layout: post
title: Pokemon Gen 2 Battery Replacement
name: pokemon-gen2-battery-replacement
image: 2021/11/04/cartridge_front.png
description: I replaced the save data battery in a Pokemon Silver cartridge as a soldering practice project.
date: 2021-11-04
tags: [GameBoy Color, Pokemon, Soldering, Battery, Cartridge]
---

{% assign post_url_parts = page.url | split: "/" %}
{% assign num_parts_to_grab = post_url_parts.size | minus: 1 %}
{% assign post_dir = post_url_parts | slice: 0, num_parts_to_grab | join: "/" %}

![Photograph of the front of a cartridge of the Japanese version of Pokemon Silver]({{ post_dir | append: "/cartridge_front.png" | absolute_url }})

For one of my first practical soldering project I decided to try replacing the save data battery in a generation 2 Pokemon game, since it would be a simple project to start with and I remember those games fondly from my childhood.

I picked up a Japanese copy of Pokemon Silver from Ebay, which had a dead save battery that prevented it from keeping its save data when turned off. I confirmed using a GameBoy Advance that the cartridge would play the game, but after saving, turning the handheld off for a few seconds, and turning it back on, the save data would no longer be there.

In order to replace the battery I needed to get a replacement battery and a screwdriver that would be able to remove the screw on the back of the cartridge that holds it together. I was able to find a [kit on Amazon](https://www.amazon.com/Triwing-Screwdriver-Batteries-Bundled-Security/dp/B07BKQJSDQ) for ~$14 USD that included a few replacement batteries and a screwdriver with 2 bits, one of which that supported the GBC cartridge screws.

I looked up some YouTube videos to see what the process is for replacing the battery and it is fairly simple: ([video](https://www.youtube.com/watch?v=NyEXRXeuA5w))

- Use a screwdriver to remove the screw on the back of the cartridge
- Open up the cartridge and remove the PCB inside
- De-solder and remove the old save battery
- Solder on the new save battery
- Put the PCB back into the cartridge
- Put cartridge back together and screw it closed

The only issue I ran into during the process is that the particular replacement batteries that I got had both tabs pointing directly outwards, as opposed to the existing battery had the tab on the top of the battery go down along the side of the battery and then point outwards. So I had to use a pair of pliers to bend the upper tab of the replacement battery down so that it touched the contact pad on the PCB.

During the process I also used some isopropyl alcohol to clean the PCB, especially the contact pads that are used to transfer data to the GameBoy, since I've heard those can wear over time.

**Before:**

![Photograph of the Pokemon Silver PCB with old battery]({{ post_dir | append: "/before.png" | absolute_url }})

**After:**

![Photograph of the Pokemon Silver PCB with the replacement battery installed]({{ post_dir | append: "/after.png" | absolute_url }})

After replacing the battery, I tried the cartridge out in my GameBoy Advance, and the save data was now preserved after turning it off and back on (after a few seconds).

![Photograph of a blue GameBoy Advance playing the fixed Pokemon Silver cartridge, with the screen showing that there is save data on the cartridge]({{ post_dir | append: "/save_data_working.png" | absolute_url }})
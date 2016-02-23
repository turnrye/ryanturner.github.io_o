---
layout: post
title: "Making a P25 Allstar node with a Motorola Astro Spectra"
description: ""
category: amateur-radio
tags: []
---
{% include JB/setup %}
The DB25 on a motorola astro spectra has most of what you need for interfacing it with a repeater controller except for the COR (carrier sense) line. In our use, since we may want to actually do P25 (letting the radio handle the modulation), we really want the COR to trigger when the speaker gets activated. Luckily there’s an easily accessible pin for that, U450 PIN 10. It puts out about 12V in my experience when the speaker is on and about 0.4V when the speaker is off. See the picture below for where you can access this. Nice and easy! All of the other needed pins are exposed on the accessory connector on the back of the radio (where you normally attach the control head).
[![Inside of Motorola Astro Spectra “drawer”]({{ site.url }}/assets/uploads/astro_inside_small.jpg)]({{ site.url }}/assets/uploads/astro_inside.jpg)
![Diagram showing connecting an Astro Spectra to a URIx]({{ site.url }}/assets/uploads/urix_astro_pinout.svg)

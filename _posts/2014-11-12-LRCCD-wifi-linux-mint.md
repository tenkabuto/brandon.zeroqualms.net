---
published: false
layout: post
title: Connecting to the LRCCD Wifi Network with Linux Mint
---

Sometime around the beginning of 2014, my college district upgraded/changed their Wi-Fi infrastructure, and seemingly no one but myself was affected by this change. Whereas other students' laptops would automatically and successfully connect to the network, my laptop (running Linux Mint 16) wouldn't. Trying the guides my college provided and contacting both the district's technical support and a professor that teaches Linux Networking, didn't help, but I finally figured it out[^1].

It turns out that the district's Wi-Fi network uses PEAP authentication for connecting to the network, and my laptop was not detecting and configuring itself so I could easily login. Once I knew the network used PEAP authentication, I just needed to poke around in Networking Settings a while to figure out how to get it to work. And finally, it now connects to the network!

Below are some basic instructions for how to connect your Linux Mint 17 laptop (this method may be compatible with previous versions, or other Linux distros, but LM17's what I'm using and have screenshots of) to the Los Rios Community College District's Wi-Fi network (SSID: "LRCCD").

If you need any further clarification (or want to say thanks), please send me a message through one of the social sites I'm linking to at the bottom of the page.

---

Open the Networking window (pictured below), click on the arrow to the right of the LRCCD network, click on the now-displayed "Settings..." button, and a window should have popped up

![Linux Mint 17's Networking Settings]({{ site.baseurl }}/images/Linux%20Mint%20-%20Networking%20Window.png)

In the window, find and click on the Wi-Fi Security tab, then proceed to change the Security and Authentication settings to what is pictured below

![Editing Network's Wi-Fi Security]({{ site.baseurl }}/images/Linux%20Mint%20-%20Editing%20LRCCD%20Wi-Fi%20Security.png)

Enter your student ID in the field next to Username, and enter your student password in the field below that

Finally, click the "Save..." button and try connecting or reconnecting to the network.

[^1]: I figured it out by looking at the LRCCD network's settings on my Android phone that was able to connect to the network without an issue.

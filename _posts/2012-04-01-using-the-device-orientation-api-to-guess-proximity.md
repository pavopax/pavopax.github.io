---
layout: post
title: Using the Device Orientation API to Guess Proximity
---
<p class="intro">The <a href="http://dev.w3.org/geo/api/spec-source-orientation.html">Device Orientation <abbr title="Application Programming Interface">API</abbr></a> of <abbr title="Hypertext Markup Language">HTML</abbr>5 tells us the orientation of the user’s device at any given moment. However, in some controlled environments it can also be used to guess a device’s position in the room.</p>

[Upperdog](http://upperdog.se/) was recently tasked with designing and developing an (iPad) web app for one of the big healthcare companies. It would be used as a sales tool at conventions and exhibitions and when not in the hand of a sales representative it would be mounted on the walls of the exhibition booth.

The idea was to turn the app’s own “screensaver” on as soon as the iPad was mounted on the wall, but since the iPad doesn’t have a RFID or NFC chip, how can we tell when it’s mounted on the wall? We used HTML5′s Device Orientation API.

<figure>
    <video width="640" height="360" controls="">
        <source src="{{ site.uploadsurl }}2014/device-orientation-assumptions.mp4" type="video/mp4">
        <source src="{{ site.uploadsurl }}2014/device-orientation-assumptions.ogg" type="video/ogg">
        <source src="{{ site.uploadsurl }}2014/device-orientation-assumptions.webm" type="video/webm">
    </video>
    <figcaption>
        <p>The angle of the books differ slightly. Using the Device Orientation API we can tell which book the iPhone is lying on. The colors are pre-defined.</p>
    </figcaption>
</figure>

The solution is not perfect and it’s just qualified guessing, but it works remarkably well. By adding a slight delay to the screensaver we can make sure that it’s not turned on as part of a larger hand motion.

This is in no way a replacement to proper near field communication, but in our controlled environment — the exhibition booth — it was all we needed to tell if the iPad was mounted on the wall or not.

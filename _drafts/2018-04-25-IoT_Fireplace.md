---
layout: post
title: IoT Fireplace
comments: true
---

<h2>IoT Fireplace</h2>

I've been asked to share how my IoT fireplace was setup so I decided to turn that knowledge into a blog post. <br><br>

<h4>Summary of why I created this</h4>
I've come to love my gas fireplace.  I don't have a need for heating the whole house as we spend a lot of our time in the living room.  One issue I was having was the need for getting the living room heated before I come home as I don't want to heat up rooms I wouldn't be using.  I decided to take matters into my own hands to make my fireplace connected to the cloud.  It uses a Particle Photon, Relay board, Alexa, and IFTTT.

<h4>Required Hardware</h4>
<a href="https://store.particle.io/collections/photon">Particle Photon</a> (make sure to get the one with headers)
<br>
<a href="https://www.amazon.com/JBtek-Channel-Module-Arduino-Raspberry/dp/B00KTEN3TM/ref=sr_1_3?keywords=single+relay+arduino&qid=1552393042&s=gateway&sr=8-3&tag=duc0c-20">Relay Module</a>
<br>
<a href="https://www.amazon.com/Multicolored-Breadboard-Dupont-Jumper-Wires/dp/B073X7P6N2/ref=sr_1_1_sspa?crid=3HHNG5TDQCIR9&keywords=jumper+wire+arduino&qid=1552393086&s=gateway&sprefix=jumper+wire+ard%2Caps%2C184&sr=8-1-spons&psc=1">Jumper wire</a>

<h4>Sofware</h4>
<a href="http://build.particle.io/build">Particle Build</a> (for developing the software)
<a href="https://ifttt.com">IFTTT</a> (to hook up to Alexa)
<a href="https://github.com/Connor-Knabe/fireplace-iot-particle/blob/master/fireplace.ino">The Code</a>

<h4>Demo</h4>
<div class = "flex-video">
    <iframe width="100%" height="100%" src="https://www.youtube.com/embed/TwfoPlLxzqA" frameborder="0" allowfullscreen></iframe>
</div>

<h2>Setup</h2>
1. Create an IFTTT account if you don't already have one.

2. Setup your Particle photon using the Particle app (iOS/Android stores). You'll need to connect to the devices WiFi and enter your WiFi password to get it setup.

3. Once it's connected with your account you'll need to flash the <a href="https://github.com/Connor-Knabe/fireplace-iot-particle/blob/master/fireplace.ino">code</a> to this device using Particle's <a href="https://build.particle.io/build">Web IDE</a>.

<h3>Triggering fireplace on from IFTTT app button</h3>

1. Setup a new <a href="https://ifttt.com/my_applets">Applet </a>

2. Choose button widget (button press)

3. Select Particle > call a function

4. Select rlySwitchOn "fireplace"

5. Do the same for fireplace off. You can optionally set it to turn

6. Set name to Fireplace on for a set amount of time use the function (rlySwitch15, rlySwitch60, etc) for 15, 60, or 120 mins. It will turn off after this set time.

<h3>Triggering fireplace from Alexa</h3>

1. Setup a new <a href="https://ifttt.com/my_applets">Applet </a>

2. Choose Alexa widget (say a specific phrase)

3. Set the phrase something like turn fireplace on

4. Select Particle > call a function

5. Select rlySwitchOn "fireplace"

<h3>Setting up the hardware</h3>

<h3>Setting up alert when Fireplace turns on (optional)</h3>

1. Go to the <a href="https://ifttt.com/maker_webhooks">webhooks</a> page and click on documentation to get the proper link to use for these triggers. You'll want to replace the event with fireplace-on or fireplace-off. Your link should look something like https://maker.ifttt.com/trigger/fireplace-on/with/key/las1kjsdfja0sdfja0sdff20aaf.

2. Go back to the Particle <a href="https://console.particle.io/integrations">integration</a> page and select new integration put in the URL from above. Type should be POST, format will be Web Form, Device Any and event name fireplace-on or fireplace-off.

3. Now head back to IFTTT and create a new Applet IF Webhook with event name of fireplace-on then THAT notification (note you will need the IFTTT app on your phone for this to be effective). Send notification from IFTTT app. Then hit create action. It will alert you anytime the fireplace has turned on. Do the same for fireplace-off.

<br><br>

If you want to talk or ask about what I've been working on drop me a line here: <a href="mailto:&#102;&#108;&#111;&#97;&#116;&#103;&#101;&#101;&#107;&#51;&#51;&#43;&#98;&#108;&#111;&#103;&#64;&#103;&#109;&#97;&#105;&#108;&#46;&#99;&#111;&#109;">floatgeek33+ifg@gmail.com</a>

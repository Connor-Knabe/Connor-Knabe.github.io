---
layout: post
title: What I've been up to lately
comments: true
---

It's been quite some time since I've last posted. I've been spending most of my free time working on side projects and the float business. I don't plan to start posting regularly again but I would like to share some of the projects I've been working on over the last few years.<br><br>

<h2>Holka-Garage (<a href="https://github.com/Connor-Knabe/holka-garage">Code on GitHub</a>)</h2>
This one was a lot of fun to implement!  It all started with a couple of problems that I was having. One problem that my wife and I both shared was a concern that we left the garage open while at work or over night.  Another was that my garage door opener signal was very weak and I would have to be in my driveway to even open the garage.  You might be thinking well why not just get a longer antenna but that'd only solve one probelm and wouldn't be nearly as enjoyable,  the same goes for buying a smart garage door opener.  This annoyance led me to creating software/hardware that would allow me to open my garage from any distance from my home.

<h4>Open via GPS</h4>
<div class = "flex-video">
    <iframe width="100%" height="100%" src="https://www.youtube.com/embed/w_uE6Tte2oI" frameborder="0" allowfullscreen></iframe>
</div>

<h4>Open via button</h4>
<div class = "flex-video">
    <iframe width="100%" height="100%" src="https://www.youtube.com/embed/bP_ioBE5NLI" frameborder="0" allowfullscreen></iframe>
</div>

<h2>Alexa/IFTTT Controlled Fireplace</h2>
Fireplace that turns on/off using a Particle Photon, Relay board, Alexa, and IFTTT.

<div class = "flex-video">
    <iframe width="100%" height="100%" src="https://www.youtube.com/embed/TwfoPlLxzqA" frameborder="0" allowfullscreen></iframe>
</div>

<h2>Clarity No Show Alert</h2>
Application written in Node.js using Nightmare.js that will alert if there are float appointments booked but no one is clocked in.  This is written on top of the FloatHelm booking/scheduling software we use.

<img class="img75" src="{{ site.baseurl }}/images/posts/what_ive_been_up_to_lately/noShowSystem.png" />

<h2>Helm member automation</h2>
At Clarity Float Spa we like to reward our members who have a stron float practice by allowing them to bring a friend every 10 floats they do.  In the past this was a manual process that our manager would have to do.  It was taking up time each week that could be spent on more creative efforts.  So I created a Nightmare.js automation script that would login to the FloatHelm (booking software we use) check to see if a member has reached 10 floats and then adds a task for the manager to send a gift card to that member. Eventually this will automatically generate the gift card and email it off to that member however we like having this be a more personal process at this time by directly emailing them.

<h2>Hue energy usage (<a href="https://github.com/Connor-Knabe/hue-energy-usage">Code on GitHub</a>)</h2>
I really appreciate limiting my electrical usage around my home.  Not only does it add up on our monthly utility bills but there is an environmental cost too.  I decided that tracking as many appliances and switching for energy efficient ones (if the numbers make sense) would be worth my time.  One thing that was extremely difficult to track was what sort of electrical footprint my light bulbs were having.  I have many Philips Hue LED light bulbs already so I wanted to know if I had incandescent bulbs which consume close to 6 times more electricity how much am I saving.  This program the tracks energy usage for these bulbs around our house.  It then reports the total costs and yearly and monthly costs.

<img class="img75" src="{{ site.baseurl }}/images/posts/what_ive_been_up_to_lately/heu.png" />

<h2>Nest energy usage</h2> 
Monitors energy usage and gives me an estimate on how much money will be spent on heating/cooling month to month.

<img class="img75" src="{{ site.baseurl }}/images/posts/what_ive_been_up_to_lately/nestEnergyUsage1.png" />
<img class="img75" src="{{ site.baseurl }}/images/posts/what_ive_been_up_to_lately/nestEnergyUsage2.png" />

<h2>Holka-Proxy</h2>
A reverse proxy server that handles incoming external requests and routes them securely over SSL to services running on a Ubuntu server.

<h2>Clarity-Waiver</h2>
A service that hooks into SmartWaiver's API that syncs data to MailChimp and Google Sheets when a waiver is filled out. Written in Node.js

<h2>Coach.me Automation</h2>
Auto completes habits that are routine using Nightmare.js

<h2>Simple-bank-helper (<a href="https://github.com/Connor-Knabe/simple-bank-helper">Code on GitHub</a>)</h2>
Little Node.js program that helps me determine where my money has been spent month to month based on goals that I have setup with Simple Bank.  Simple does this but I custom made this script to give me more accurate numbers.

<img class="img50" src="{{ site.baseurl }}/images/posts/what_ive_been_up_to_lately/simpleBankHelper.png" />

<br><br>

Want to talk about what I've been working on drop me a line here: <a href="mailto:&#102;&#108;&#111;&#97;&#116;&#103;&#101;&#101;&#107;&#51;&#51;&#43;&#98;&#108;&#111;&#103;&#64;&#103;&#109;&#97;&#105;&#108;&#46;&#99;&#111;&#109;">floatgeek33+wibutl@gmail.com</a>

---
layout: post
title: Auto Zen Float Tent
comments: true
---

I've had this idea of an automated float center for some time now.  If you'd like to know more about this see my articles titled <a href="{{ site.baseurl }}/2015/02/automated-float-tank-center" target="blank">Automated Float Tank Center</a> and <a href="{{ site.baseurl }}/2015/03/how-to-design-an-automated-float-tank-center" target="blank">How to Design An Automated Float Tank Center</a>.  Since I've started working on building a float center of my own called <a href="http://clarityfloats.com/" target="blank">Clarity Float Spa</a> my mindset on a fully automated float center has started to shift.  I've come to realize that having a human element seems to be crucial to a successful float center.  The post float discussion is extremely important, especially for those floatees who just had a profound life changing experience in the tank.  So instead of going for a fully automated center I've started creating hardware and software to make running a float center easier. That being said I still think there is a place for a fully automated float tank center but it is not something I am pursuing at this time.
<br><br>
The software and hardware I'm creating is designed to make the process of running a float center much smoother.  Instead of spending time worrying about the tanks you can focus on your customers and that personal interaction.  These systems should be able to monitor the water quality including: ph, hydrogen peroxide, specific gravity, alkalinity, water level, and more. All of this data should be accessible from the internet and can be recorded automatically or manually from a smart phone or computer.  There should be systems in place to also handle the lighting of the room, the float tank speakers (if applicable), and the pumps for filtering the water.  Another system that would be useful could monitor if anything goes wrong: pump failure, water leakage, heater failure, etc.  Keep in mind I do not have all of these systems developed yet but it is a work in progress.  I have a <a href="http://www.zenfloatco.com/?tap_a=5195-1d77bb&tap_s=10751-455ee4&tm_banner=sidebar" target="blank">Zen Float Tent</a> and have created some software and harware around it to test out the automated float tank concept.  If you'd like more info on the Zen Float Tent I have a post about it titled <a href="{{ site.baseurl }}/2015/09/thoughts-about-the-zen-float-tent" target="blank">Thoughts About the Zen Float Tent</a>.









<br><br>
<h2>Demos of the software</h2>

<div class = "flex-video">
    <iframe width="100%" height="100%" src="https://www.youtube.com/embed/0fiaWlnwovE" frameborder="0" allowfullscreen></iframe>
</div>
<h3>Automated Float Demo</h3>
A full demo of the automated software.  Shows you how to setup the float by choosing: how long your float is, what color before/after, and which music to bring you out of the float.  You may notice lights flashing near the middle (this typically is a warning to wrap up the shower before the float).
<br><br>

<div class = "flex-video">
    <iframe width="100%" height="100%" src="https://www.youtube.com/embed/bIeb9WJel68" frameborder="0" allowfullscreen></iframe>
</div>
<h3>Appointment Reminders - Confirm</h3>
This is a program I wrote that uses Twilio and Google Calendar API to send appointment reminders for people who are coming to float. The system is setup by adding a user to Google Calendar and entering their cell phone number under notes (only their for first appointment).  The software will know if it is their first time or not based on the number code in the title (00 or 01) and will only include tips for their first float.  This shows the confirmation message.
<br><br>

<div class = "flex-video">
    <iframe width="100%" height="100%" src="https://www.youtube.com/embed/Vfg2ShZ6_J8" frameborder="0" allowfullscreen></iframe>
</div>
<h3>Appointment Reminders - Cancel</h3>
This shows the cancelation message for the appointment reminder program.
<br><br>


<div class = "flex-video">
    <iframe width="100%" height="100%" src="https://www.youtube.com/embed/YzxXtxAGVcM" frameborder="0" allowfullscreen></iframe>
</div>
<h3>IoT Intex Pump on/off</h3>
This is the custom Intex pump setup for the Zen Float Tent.  It can be controlled via the website to turn it on and off.  After each float the pump kicks on for 30-45 minutes.  
<br><br>

<div class = "flex-video">
    <iframe width="100%" height="100%" src="https://www.youtube.com/embed/hImYL1xOaCI" frameborder="0" allowfullscreen></iframe>
</div>
<h3>IoT Intex Pump Timed</h3>
Demo of how to set a timer for how long the Intex pump should run.  This can be run at anytime not just after a float.
<br><br>

<div class = "flex-video">
    <iframe width="100%" height="100%" src="https://www.youtube.com/embed/HBL7oUec-AI" frameborder="0" allowfullscreen></iframe>
</div>
<h3>Hydrogen Peroxide Doser</h3>
Note this is a prototype/proof of concept.  It simply doses hydrogen peroxide throughout the day or from the website. You can also enter a custom amount in milliliters to dose manually.
<br><br>

<div class = "flex-video">
    <iframe width="100%" height="100%" src="https://www.youtube.com/embed/8XXIlJKzYy0" frameborder="0" allowfullscreen></iframe>
</div>
<h3>Hydrogen Peroxide Container</h3>
This is the container that holds the hydrogen peroxide.
<br><br>

<div class = "flex-video">
    <iframe width="100%" height="100%" src="https://www.youtube.com/embed/lleIsPFuNII" frameborder="0" allowfullscreen></iframe>
</div>
<h3>Water Sensor</h3>
This is a water sensor that will send a text message and turn off pumps if water is detected.
<br><br>



<h2>Summary</h2>
I see a bright future for the internet of things in the float community.  I think it will allow more quality customer interaction and less things to have to maintain manually.  At the end of the day it is the customers who really matter and taking some of the work away from the tanks and dedicating that time to more positive customer interactions seems to make sense.  I think software like this will make float centers even more of an enjoyable place to work and be.  

Want to talk about this further drop me a line here: <a href="mailto:&#102;&#108;&#111;&#97;&#116;&#103;&#101;&#101;&#107;&#51;&#51;&#43;&#98;&#108;&#111;&#103;&#64;&#103;&#109;&#97;&#105;&#108;&#46;&#99;&#111;&#109;">floatgeek33@gmail.com</a>

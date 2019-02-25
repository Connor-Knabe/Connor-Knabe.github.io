---
layout: post
title: What I've been up to lately
comments: true
---

It's been quite some time since I've last posted. I've been spending most of my free time working on side projects and the float business. I don't plan to start posting regularly again but I would like to share some of the projects I've been working on over the last few years.<br><br>

<h2>Holka-Garage (<a href="https://github.com/Connor-Knabe/holka-garage">Code on GitHub</a>)</h2>
This one was a lot of fun to implement!  It all started with a couple of problems that I was having. One problem that my wife and I both shared was a concern that we left the garage open while at work or overnight.  Another was that my garage door opener signal was very weak and I would have to be in my driveway to even open the garage.  You might be thinking well why not just get a longer antenna but that'd only solve one problem and wouldn't be nearly as enjoyable,  the same goes for buying a smart garage door opener.  This annoyance led me to creating software/hardware that would allow me to open my garage from any distance from my home.

<h4>Open via GPS</h4>
<div class = "flex-video">
    <iframe width="100%" height="100%" src="https://www.youtube.com/embed/w_uE6Tte2oI" frameborder="0" allowfullscreen></iframe>
</div>

<h4>Open via button</h4>
<div class = "flex-video">
    <iframe width="100%" height="100%" src="https://www.youtube.com/embed/bP_ioBE5NLI" frameborder="0" allowfullscreen></iframe>
</div>

<h2>Alexa/IFTTT Controlled Fireplace</h2>
I've come to love my gas fireplace.  I don't have a need for heating the whole house as we spend a lot of our time in the living room.  One issue I was having was the need for getting the living room heated before I come home as I don't want to heat up rooms I wouldn't be using.  I decided to take matters into my own hands to make my fireplace connected to the cloud.  It uses a Particle Photon, Relay board, Alexa, and IFTTT.

<div class = "flex-video">
    <iframe width="100%" height="100%" src="https://www.youtube.com/embed/TwfoPlLxzqA" frameborder="0" allowfullscreen></iframe>
</div>

<h2>Clarity No Show Alert</h2>
One concern I've had when owning a business that is run by a team of people is what happens if someone forgets their shift and has to open in the morning.  To help ease my concern I decided to write a program that would verify a teammate is clocked in so long as there is someone booked for an appointment that morning.  It is written in Node.js using Nightmare.js written on top of our booking software (FloatHelm) it sends text alerts to the managers and teammate who is supposed to be clocked in.  If they still don't clock in after 10 minutes it will call all of us.  Below are photos of the system working and another one when I was working on the code outside in the warm summer weather.

<img class="img75" src="{{ site.baseurl }}/images/posts/what_ive_been_up_to_lately/noShowAlert.png" />
<img class="img75" src="{{ site.baseurl }}/images/posts/what_ive_been_up_to_lately/noShowAlertOutside.jpg" />

<h2>Helm member automation</h2>
At Clarity Float Spa we like to reward our members who have a strong float practice by allowing them to bring a friend every 10 floats they do.  In the past this was a manual process that our manager would have to do.  It was taking up time each week that could be spent on more creative efforts.  So I created a Nightmare.js automation script that would login to the FloatHelm (booking software we use) check to see if a member has reached 10 floats and then adds a task for the manager to send a gift card to that member. Eventually this will automatically generate the gift card and email it off to that member however we like having this be a more personal process at this time by directly emailing them.

<h2>Hue energy usage (<a href="https://github.com/Connor-Knabe/hue-energy-usage">Code on GitHub</a>)</h2>
I like to focus some energy on limiting my electrical usage around my home.  Not only does it add up on our monthly utility bills but there is an environmental cost too.  I decided that tracking as many appliances and switching for energy efficient ones (if the numbers make sense) would be worth my time.  One thing that was extremely difficult to track was what sort of electrical footprint my light bulbs were having.  I have many Philips Hue LED light bulbs already so I wanted to know if I had incandescent bulbs which consume close to 6 times more electricity how much am I saving.  This program the tracks energy usage for these bulbs around our house.  It then reports the total costs and yearly and monthly costs.

<img class="img75" src="{{ site.baseurl }}/images/posts/what_ive_been_up_to_lately/heu.png" />

<h2>Nest energy usage</h2> 
Air conditioners are one of the most energy hungry appliances in a home or an apartment.  Along the same lines as why I track my light bulb energy usage I wanted to do the same for my AC and Furnace.  I previously had a Honeywell Smart thermostat which was great however it did not have a good API that I could use to pull data from it.  This is what prompted me to purchase a Nest Gen 3 thermostat was because the API and documentation were excellent and would allow me to gather the data I needed to solve this problem.  The program I wrote monitors energy usage and gives me an estimate on how much money will be spent on heating/cooling month to month.

<img class="img75" src="{{ site.baseurl }}/images/posts/what_ive_been_up_to_lately/nestEnergyUsage1.png" />
<img class="img75" src="{{ site.baseurl }}/images/posts/what_ive_been_up_to_lately/nestEnergyUsage2.png" />

<h2>Holka-Proxy</h2>
I have many different programs and services hosted on my <a href="https://m.do.co/c/cf0b0981d05d">DigitalOcean</a> box.  In order to help keep all of the programs secure using SSL I created a reverse proxy. This program handles incoming external requests and routes them securely over SSL to services running on my Ubuntu server.

<h2>Clarity-Waiver</h2>
At Clarity Float Spa in the past we would send out hand written letters to customers after their first float.  This process was difficult to track what letters were written and by whom.  To make this easier I hooked into our waiver's API (SmartWaiver) using Node.js that then would sync data over to a Google Sheet in order for us to keep track of which letters were written. This allowed us to make the process much easier and required much less manual work to accomplish.

<h2>Coach.me Automation</h2>
I'm a huge fan of the website <a href="https://Coach.me">https://Coach.me</a> it has helped me accomplish many self improvement goals that I set for myself and ultimately I believe has made myself a better person.  There are many habits that I do daily (like meditation) that I would manually have to click every morning.  I do like to keep track of this in the event I do fall out of a meditation habit.  So instead of removing this habit from the app I wrote a little script using Nightmare.js that logs in every morning and checks off my daily habits automatically.

<h2>Simple-bank-helper (<a href="https://github.com/Connor-Knabe/simple-bank-helper">Code on GitHub</a>)</h2>
I was wondering how much money I was spending month to month based on my current budget that was set up with my bank <a href="https://www.simple.com/">https://simple.com/</a>.  The way I had my budget setup make it difficult to calculate these numbers unless you went back manually and looked to see month to month what the expenses were in each of the <a href="https://www.simple.com/features/goals">goals</a> I had created for that month's budget.  One thing you might be wondering is why not use <a href="https://www.simple.com/features/expenses">expenses</a>?  At the time expenses had not come out yet (they came out a few months after I wrote this program actually). The program was written in Node.js and would help me determine where my money has been spent month to month.  
<img class="img50" src="{{ site.baseurl }}/images/posts/what_ive_been_up_to_lately/simpleBankHelper.png" />

<br><br>

If you want to talk or ask about what I've been working on drop me a line here: <a href="mailto:&#102;&#108;&#111;&#97;&#116;&#103;&#101;&#101;&#107;&#51;&#51;&#43;&#98;&#108;&#111;&#103;&#64;&#103;&#109;&#97;&#105;&#108;&#46;&#99;&#111;&#109;">floatgeek33+wibutl@gmail.com</a>

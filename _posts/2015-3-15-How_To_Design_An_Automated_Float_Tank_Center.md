---
layout: post
title: 3 Parts of An Automated Float Tank Center
comments: true
---
<b> Last edited: 3/15/15 </b>

<h3>Various components to the system</h3>
This post may get a bit technical so if some of this information seems to be a bit dry to you feel free to skip around.  
The reason for this post is to speak in more detail about what will be required to create a fully automated float center. Some of the components that will need to be implemented will include Arduinos(microcontrollers), access cards(to get into building), a database(storing user info), Stripe/Paypal(credit card processor), and networking to tie the whole system into the internet.  

We will break down the whole system into 3 different systems. These systems are:
<ol>
    <li>Scheduling/Billing System</li>
    <li>Building security</li>
    <li>Filtration/clean up</li>
</ol>


<h3>Scheduling/Billing System</h3>
This is the system that will be designed around a website that will allow floaters to sign up on the website and schedule floats.  
There are already many versions of this type of software developed however one needs to be custom designed to fit in with the automated float center. Some examples include:
<ol>
    <li><a href="https://floathelm.com/" target="blank">FloatHelm</a></li>
    <li><a href="http://www.frontdeskhq.com/" target="blank">FrontDesk</a></li>
    <li><a href="http://zenplanner.com/" target="blank">ZenPlanner</a></li>
    <li><a href="https://www.mindbodyonline.com/" target="blank">MindBodyOnline</a></li>
</ol>
Scheduling all starts with the customer wanting to book at float online.  He will go to the website and there will be a button that will pull up the scheduling application.  From there they can pick the time they want to float and then pay using a credit card.  This system will need to be tied into the building security system which will permit the user to gain access using their access card or PIN number when they show up to float.

This process might look like this:  
<ol>
    <li>User books/pays for float online</li>
    <li>Access card is activated for the time they have scheduled</li>
    <li>They show up and their access card allows them to enter their specified float room</li>
</ol>


<h3>Building security</h3>
In order to maintain security for the building and the customers who use this facility there must be strict access into the building only permitted if that user has scheduled a float.
The reason for strict access is that we only want floaters who are permitted into the facility at their designated float time,  if this is not the case then people may be tempted to steal floats or to disrupt the peaceful waiting room which could become overcrowded.  The access control software would be able to keep track of how long users stay at the float tank center including time during, before, and after their float.  These metrics would be a lot easier to obtain if the only permitted people into the building have been authorized to float.  These metrics could be used to help cut back on unnecessary time spent between float sessions and to help provide an overall better experience for the floater.

This aspect of the float center would operate similar to a 24/7 tanning salon except that users only have a certain time window in which they can gain access to the facility.  This system would need an access card reader or PIN pad on the front door and on each of the float tank room doors.  When the user arrives they will already know which room they are floating in via text message or email, so they can go into the facility and head to the room they have booked for floating.  Once the user enters their room they will take a shower and then enter the tank.  A sensor will be placed on the door of the room which will detect when it was opened and will know to start a timer which will play music in the tank when the float time is up.  

Certain problems can appear at this stage of the process:
<ol>
    <li>What if the floater arrives late for their float?</li>
    <li>How do you prevent a floater from staying longer in the tank?</li>
    <li>What if the floater has health complications in the tank?</li>
</ol>

To combat some of these problems there will need to be fail-safes in place.  Let's take the example of the floater arriving late for their appointment.  If the floater arrives more than 15 minutes late the front door would not allow them to enter.  This would keep the process moving smoothly because if a floater arrives late it could push back the floats for other people.  

In the event that a floater stays in the tank longer than scheduled, there will be various ways to "encourage" them to get out of the tank. When the time is up there first might be some music that begins to play in their float tank.  Then if they still have not gotten out (motion sensor to detect this) a light could come on and then start flashing if they continue to stay in the tank.  

The third problem is a bit tricky because without someone being on site it might be hard to know if someone is having problems in the tank.  This issue could be compared to a swimming pool that has no lifeguard on duty where there would be a disclaimer that in the event something bad happens there may be no one to help you.  Besides this disclaimer another useful option would be to place an "emergency" button inside the tank so if the floater is having issues they can hit the button and it will dial 911 and they could talk to them via a speaker in the tank.  


<h3>Filtration/clean up</h3>
In between float sessions it is necessary to run the tank's filtration system in order to clean all of the water of bad bacteria and pathogens that may have accumulated after a person's float.  This system will be implemented by using a motion detector to sense when a person has gotten out of the tank and has started their post float shower.  Something to keep in mind the system would have to verify that that floater's time has been used up in the event that they were planning on going back to continue floating.  

<h3>Summary</h3>
To sum things up there is a lot of technical aspects that go into creating an automated float tank center.  Clearly this system needs to be well thought out ahead of time and designed carefully with fail-safes in place to help deal with any problems that might occur.

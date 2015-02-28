---
layout: post
title: How To Design An Automated Float Tank Center
comments: true
---
<b> Last edited: 2/26/15 </b>

<h3>Various components to the system</h3>
This post may get a bit technical so if some of this information seems to be a bit boring to you feel free to skip over the technical parts.  
The reason for this post is to lay out what will be required to create a fully automated float center and which parts would consume the most amount of time to develop.  Some of the components that will need to be implemented will include Arduinos(microcontrollers), access cards(to get into building), a database(storing user info), Stripe, Paypal(credit card processor), and networking to tie the whole system into the internet.  

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
For scheduling it all starts with the customer wanting to book at float.  He will go to the website and there will be a button that will pull up the scheduling software.  From there they can pick the time they want to float and then pay using a credit card.  This system will need to be tied into the building security system which will permit the user to gain access using their card when they show up to float.  
<ol>
    <li>User books/pays for float online</li>
    <li>Access card is activated for the time they have scheduled</li>
    <li>They show up and their access card allows them to enter their specified float room</li>
</ol>


<h3>Building security</h3>
In order to maintain security for the building and the customers who use this facility there must be strict access into the building only permitted if that user has scheduled a float.
The reason for strict access is that we only want floaters who are permitted into the facility at their designated float time,  if this is not the case then people may be tempted to steal floats or to disrupt the peaceful waiting room which could become overcrowded.  Another reason for this is it would be useful to keep track of how long users stay at the float tank center including time before and after their float.  These metrics would be a lot easier to obtain if the only permitted people into the building have been authorized to float.

This aspect of the float center would operate similar to a 24/7 tanning salon except that users only have a certain time window in which they can gain access to the facility.  This system would need an access card reader on the front door and on each of the float tank room doors.  When the user arrives they will already know which room they are floating in via text message or email so they can go into the facility and head to the room they have booked for floating.  Once the user enters their room they will take a shower and then enter the tank.  A sensor will be placed on the door of the room which will detect when it was opened and will know to start a timer which will play music in the tank when the float time is up.  

Certain problems can appear at this stage of the process:
<ol>
    <li>What if the floater arrives late for their float?</li>
    <li>How do you prevent a floater from staying longer in the tank?</li>
    <li>What if the floater has health complications in the tank?</li>
</ol>

To combat some of these problems.........

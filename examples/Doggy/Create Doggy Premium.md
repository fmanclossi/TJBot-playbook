# Mount Doggy Premium - a TJBot companion with superdog vision, a cute tail and two powerful legs!

Doggy is the perfect companion for your TJBot. DOGGY Premium hosts an HC-SR04 sensor that provides a superdog vision, a servo motor to animate the cutest tail in the world and two motorized legs.

# HAVE FUN and REPORT ISSUES!!! PHOTOS, VIDEOS, FEEDBACKS are WELCOME!

## Level: some task could be tricky but could be performed under adult’s guidance

## Requirements

## Get and Print/Copy DOGGY Premium design file

## Mount your Doggy Premium

* Print/reproduce all the design sheets

![Premium design sheets](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/DoggyReduced/01.Doggy%20printed%20sheets.jpg)
 
* Follow instructions for Doggy Basic (2-6) and step 2 for Doggy Standard.

* Cut and Fold advanced Belly component

![Premium cut and folded](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/DoggyReduced/13.Doggy%20Advanced%20cutted%20and%20folded.jpg)
 
* Clip hind legs

![hind legs #1](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/DoggyReduced/14.Doggy%20-%20stappling%20hind%20legs%20-%20detail.jpg)

![hind legs #2](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/DoggyReduced/15.Doggy%20-%20Stappling%20hind%20legs.jpg)

![hind legs #3](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/DoggyReduced/16.Doggy%20-%20stapple%20hind%20legs.jpg)
   
* Mount servo motors for front legs and clip to fix them

![servo #1](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/DoggyReduced/17.Doggy%20-%20mount%20servo%20motors.jpg)

![servo #2](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/DoggyReduced/18.Doggy%20-%20servo%20position1.jpg)
 
* (optional and in beta version) If you want to tighten up belly component (e.g. if you print it on 200gr/m² A4 paper), print, cut, fold and clip the beam component

![stronger belly #1](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/DoggyReduced/19.Doggy%20-%20Beta%20-%20component%20for%20stronger%20belly.jpg)

![stronger belly #2](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/DoggyReduced/20.Doggy%20-%20beta%20-%20make%20a%20stronger%20belly.jpg)
  
* Cut and Roll up front legs on shortest side

![create leg](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/DoggyReduced/21.Doggy%20roll%20up%20legs.jpg)
 
TIP: Fix leg to servo arm as shown in picture, leaving space to attach it to servo and fixing leg to the external part.

![fix leg #1](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/DoggyReduced/22.Doggy%20how%20to%20create%20leg.jpg)

![fix leg #2](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/DoggyReduced/23.Doggy%20how%20to%20fix%20leg.jpg)
  

As tail, legs are personality traits. Use your imagination and try different legs. In the following photo, I wrapped leg starting from servo arm to leg’s end.

![tail #2](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/DoggyReduced/25.Doggy%20tail%20version2.jpg)

* wire HC-SR04 sensor and SG-90 servo motor (tail, right leg/arm, left leg/arm) to TJBot. A breadboard is recommended. Fix breadboard to Doggy’s belly.

**Breadboard wiring for Advanced cases**

Description | From TJBot | From Doggy’s eyes | From Doggy’s tail | From Doggy’s left arm | From Doggy’s Right arm
----------- | -------- | ----------------- | ----------------- | --------------------- | ----------------------
Type of connectors | Female to Male | Male to Female | Male to Male | Male to Male | Male to Male
Pin 38 - GPIO 20 - Data servo motor (right Doggy’s arm) | Green |  |  |  | Violet to Orange (data servo motor)
Pin 40 - GPIO 21 - Data servo motor (left Doggy’s arm) | Yellow |  |  | Violet to Orange (data servo motor)	 | 
Pin 25 - Ground | Blue | Blue to Ground | Brown to Brown (Ground) | Brown to Brown (Ground) | Brown to Brown (Ground)
Pin 23 - GPIO 11 - Echo | Violet | Green to Echo |  |  | 
Pin 21 - GPIO 09 - Trigger | Gray | Yellow to Trigger |  | 	 | 
Pin 4 - 5V | White | Orange to VCC | Red to Red (5V) | Red to Red (5V) | Red to Red (5V)
Pin 24 - GPIO 08 - Data servo motor (tail) | Black |  | Orange to Orange (Data servo motor) |  | 

**WARNING: pay attention to connect the right PINs to avoid damages to components.**

* Build tail (version #1). Get Servo arm and tape tail to it.

![tail #1](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/DoggyReduced/24.Doggy%20Tail%20version%201.jpg)

* Build tail (version #2). Tail is a personality trait. Use your imagination and try different tails. In the following photo, I wrapped tail starting from servo arm to tail’s end creating a rotation effect that I like.

![tail #2](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/DoggyReduced/25.Doggy%20tail%20version2.jpg)

* enjoy your Doggy Premium

![Doggy Premium](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/DoggyReduced/26.Doggy_standing%20up.jpg)


....

[Back to main Doggy's page](https://github.com/fmanclossi/TJBot-playbook/tree/master/examples/Doggy)


# License  
This project uses the [Apache License Version 2.0](../../LICENSE) software license.  

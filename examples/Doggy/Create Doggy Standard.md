# Mount Doggy Standard - a TJBot companion with superdog vision and a cute tail!

Doggy is the perfect companion for your TJBot. DOGGY Standard hosts an HC-SR04 sensor that provides a superdog vision and a servo motor to animate the cutest tail in the world.

# HAVE FUN and REPORT ISSUES!!! PHOTOS, VIDEOS, FEEDBACKS are WELCOME!

## Level: some task could be tricky but could be performed under adult’s guidance

## Requirements

## Get and Print/Copy DOGGY Standard design file

## Mount your Doggy Standard


* Print/reproduce only the Tail and advanced Sheet

![design file to print](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/DoggyReduced/01.Doggy%20printed%20sheets%20-%20first.jpg)

* Follow instructions for Doggy Basic, just cut tail parts.

[link to Doggy Basic](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Create%20Doggy%20Basic.md)

* Mount servo motor for tail (do not mount tail now, the right position will to be identified during software setup)

[Basic with servo mounted - and eyes not cut](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/DoggyReduced/08.Doggy%20-%20basic%20with%20tail%20servo%20mounted.jpg)

(notice that I forgot to cut eyes)

* wire HC-SR04 sensor and SG-90 servo motor to TJBot (look at the picture to insert servo with the right orientation). A breadboard could make this task easier, but it’s not strictly required.: fix breadboard to Doggy’s back (upside down).
Breadboard wiring for Standard case

Description | From TJBot | From Doggy’s eyes | From Doggy’s tail
----------- | ---------- | ----------------- | -----------------
Type of connectors | Female to Male | Male to Female | Male to Male
Pin 25 - Ground | Blue | Blue to Ground | Brown to Brown (Ground)
Pin 23 - GPIO 11 - Echo | Violet | Green to Echo	
Pin 21 - GPIO 09 - Trigger | Gray | Yellow to Trigger	
Pin 4 - 5V	White | Orange to VCC | Red to Red (5V)
Pin 24 - GPIO 08 Data servo motor (tail) | Black | Orange to Orange (Data servo motor)

**WARNING: pay attention to connect the right PINs to avoid damages to components.**

8a-Build tail (version #1). Get Servo arm and tape tail to it.

![tail #1](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/DoggyReduced/24.Doggy%20Tail%20version%201.jpg)

8b-Build tail (version #1). Tail is a personality trait. Use your imagination and try different tails. In the following photo, I wrapped tail starting from servo arm to tail’s end creating a rotation effect that I like.

![tail #2](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/DoggyReduced/25.Doggy%20tail%20version2.jpg)

9 (optional) - print and cut standard belly component from Optional/Advanced Parts design sheet

![standard belly](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/DoggyReduced/10.Doggy%20-%20tailed%20version%20with%20basic%20belly.jpg)
 

* enjoy your Doggy Standard

....

[Back to main Doggy's page](https://github.com/fmanclossi/TJBot-playbook/tree/master/examples/Doggy)


# License  
This project uses the [Apache License Version 2.0](../../LICENSE) software license.  

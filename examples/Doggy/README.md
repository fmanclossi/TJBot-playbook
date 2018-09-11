# TJBot and her/his dog

Doggy is the perfect companion for your TJBot. It's available in four format, expanding TJBot features and enabling funny scenarios.

![TJDog and his-her dog](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/TJBot%20and%20Doggy%20-%20advanced%20version.gif)

It works with TJBot already configured as described in [setup pages](https://github.com/fmanclossi/TJBot-playbook/tree/master/setup).

## Doggy's family

### DOGGY BASIC 

Doggy hosts an HC-SR04 sensor that provides a superdog vision.

### DOGGY STANDARD

In addition to BASIC format, Doggy  has also a very cute tail, powered by one SG-90 servo motor.

### DOGGY ADVANCED (PREMIUM)

Doggy increases its capability with two motorized front legs.

## MINIDOGGY

![MiniDoggy](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/MiniDoggy_with_tail_20180903b.jpg)

This little Doggy has just tail, powered by one SG-90 servo motor. No superdog vision!

It's very easy to build 'cause it provided with A4 format. Just print it on your printer and cut, fold, connect.

# HAVE FUN and REPORT ISSUES!!! PHOTOS, VIDEOS, FEEDBACKS are WELCOME!

### Level: some task could be tricky but could be performed under adult’s guidance

### Requirements:
Component |Doggy Basic | Doggy Standard | Doggy Advanced (Premium) | MiniDoggy
--------- | ---------- | -------------- | -------------- | ---------
TJBot setup with [JCBisson Node-Red nodes](https://github.com/fmanclossi/TJBot-playbook#jeancarl-node-red-examples) | Yes | Yes | Yes | Yes
1 x HC-SR04 ultrasonic sensor for TJDog supervision  | Yes | Yes | Yes | No
1 x SG90 servo motor for TJDog tail | No | Yes | Yes | Yes
2 x SG90 servo motor for TJDog front legs | No | No | Yes | No
1 x Breadboard | No | Optional | Yes | No
Cables, Cardboard, stapler, marking pens, scotch tape | Yes | Yes | Yes | Yes

## Build your preferred TJBot companion

### Get the last design file from [Doggy Github house](https://github.com/fmanclossi/TJBot-playbook/tree/master/examples/Doggy/Design_files)

* Doggy Basic - Superdog vision only

   * [Doggy DXF format](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Design_files/Doggy_with_tail_A4_20180908a.dxf)

   * [Doggy PDF format - basic parts](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Design_files/Doggy_with_tail_20180908a_basic_A4.pdf)

* Doggy Standard - Basic plus ultra-dynamic tail

   * [Doggy DXF format](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Design_files/Doggy_with_tail_A4_20180908a.dxf)

   * [Doggy PDF format - basic parts](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Design_files/Doggy_with_tail_20180908a_basic_A4.pdf)

* Doggy Premium - Standard plus powerful front legs

   * [Doggy DXF format](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Design_files/Doggy_with_tail_A4_20180908a.dxf)

   * [Doggy PDF format - basic parts](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Design_files/Doggy_with_tail_20180908a_basic_A4.pdf)

   * [Doggy PDF format - Optional and advanced parts](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Design_files/Doggy_with_tail_20180908a_advanced_A4.pdf)

* MiniDoggy - ultra-dinamic tail only

   * [MiniDoggy DXF format](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Design_files/MiniDoggy_with_tail_20180903b.dxf)

   * [MiniDoggy PDF format](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Design_files/MiniDoggy_with_tail_20180903b.pdf)

### Print or Copy the design file on selected support

Please, share your experience on [Doggy's House](https://github.com/fmanclossi/TJBot-playbook/tree/master/examples/Doggy)!!!
 
* Doggy Basic - Superdog vision only

Do not use common printer paper. 
Doggy Basic can be easily printed on 200gr/m² A4 paper (local print shop or standard printer) or cardboard.
200gr/m² A4 paper is enough strong to support sensor weight.
No need for "Belly" part (but if you like it, just fold and insert it).

* Doggy Standard - Basic plus ultra-dinamic tail

Do not use common printer paper. 
Doggy Standard can be easily printed on 200gr/m² A4 paper (local print shop or standard printer) or cardboard.
200gr/m² A4 paper is enough strong to support sensor weight.
"Belly" part is optional, depending upon wiring choices (but if you like it, just fold and insert it).

* Doggy Premium - Standard plus powerful front legs

Do not use common printer paper. 
Doggy Standard can be easily printed on 200gr/m² A4 paper (local print shop or standard printer) or cardboard.
200gr/m² A4 paper is enough strong to support sensor weight.
"Belly" part is mandatory. It could be printed on 200gr/m² A4 paper, but cardboard is the best choice.

* MiniDoggy - ultra-dynamic tail only

MiniDoggy can be easily printed on 200gr/m² A4 paper (local print shop or standard printer)
200gr/m² A4 paper is enough strong to support servo motor weight.
No need for "Belly" part (but if you like it, just fold it and insert mounting servo on it). Belly part is mandatory if you use standard printer paper.

 
### Mount your Doggy

#### Doggy Basic - Superdog vision only

* Print/reproduce only the Tail and advanced Sheet

* cut all the red lines using a cutter and a scissor (do not cut parts to host servo motor for tail). If you plan to use superdog vision, remind to cut eyes too.
 
(P.S: in the following pictures these lines are cut as used in Standard and Advanced version)

* fold up or down green and green lines

  (fold up)

(fold down)

(I’m folded up and down)

* stapple left and right ears
      
* stapple neck and back
 
* insert tongue and clip the tail

(notice neck and back staple)

* wire HC-SR04 sensor to TJBot (no need for breadboard)

Description	 | From TJBot to Doggy’s eyes
----------- | --------------------------
Type of connectors | Female to Female
Pin 25 - Ground | Blue to Ground
Pin 23 - GPIO 11 - Echo | Green to Echo
Pin 21 - GPIO 09 - Trigger | Yellow to Trigger
Pin 4 - 5V | Orange to VCC

**WARNING: pay attention to connect the right PINs to avoid damages to components.**

* enjoy your Doggy Basic


....

# License  
This project uses the [Apache License Version 2.0](../../LICENSE) software license.  

For many of the proposed LABs you can use a standard TJBot or a modified one. If a different configuration is required, it will be noted at the start of the exercise.
Many exercises are based upon Node-Red. It's easy, fast, good for every kind of students (from kids to grandmas)!

## Setup a standard TJBot
Bring TJBot to life following instructions available at https://github.com/ibmtjbot/tjbot
![Bring TJBot to life](https://github.com/ibmtjbot/tjbot/raw/master/images/tjbot.jpg)

### Some tips:

* Carefully verify LED PINs layout
* If you plan to use LED, disable internal audio and use a USB audio adapter or bluetooth
* Remind your Raspberry user and password :)
* Note your TJBot IP address (if it remains the same)
* Perform all the tests
  * Connect to Raspberry (using local keyboard/screen, VNC or SSH)
  * Install TJBot test prerequisite. The following command assumes you have cloned the tjbot git repository to your Desktop.

    `npm install ~/Desktop/tjbot/bootstrap/tests`

  * Go in bootstrap directory:

    `cd ~/Desktop/tjbot/bootstrap`

  * Run full comprehensive tests for TJBot:

    `./runTests.sh`

  * Or Run single test launching specific script:

    `cd ~/Desktop/tjbot/bootstrap/tests`
    
    `sudo node test.camera.js`
    
    `sudo node test.led.js`
    
    `sudo node test.servo.js`
    
    `sudo node test.speaker.js`

### Try some official recipes on your own *before* performing laboratories at school :)

Recipes are step-by-step instructions to bring your TJBot to life. They follow a typical structure:
![recipe structure](https://github.com/fmanclossi/TJBot-playbook/blob/master/setup/Images/TJBot%20Lab%20-%20Recipe%20structure.jpg)

**Official recipes:**
* [Use Your Voice to Control a Light with Watson!](http://www.instructables.com/id/Use-Your-Voice-to-Control-a-Light-With-Watson/)
* [Make Your Robot Respond to Emotions Using Watson!](http://www.instructables.com/id/Make-Your-Robot-Respond-to-Emotions-Using-Watson/)
* [Build a Talking Robot with Watson!](http://www.instructables.com/id/Make-Your-Robot-Respond-to-Emotions-Using-Watson/)

## Setup a "standard" TJBot Node-Red environment
*.... to be completed...*

## Setup a NOT standard TJBot
*.... to be completed...*
[TJbot with two arms and two LEDs... and more!](https://github.com/fmanclossi/tjbotTwoArmsTwoLEDs)

## Setup a "standard" TJBot Node-Red environment
*.... to be completed...*
[Node-Red nodes for TJbot with two arms and two LEDs... and more!](https://github.com/fmanclossi/node-red-contrib-tjbotTwoArmsTwoLeds)

## Working On... 
*Where I can buy more time?*

# License  
This project uses the [Apache License Version 2.0](https://github.com/fmanclossi/TJBot-playbook/blob/master/LICENSE) software license.  

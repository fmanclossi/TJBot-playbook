# TJBot-playbook
Collected information about IBM TJBot, my enahncements and most from all the fans around the world!

Contribution are welcome!

First of all, read https://github.com/ibmtjbot/tjbot
Many thanks to the entire TJBot team!!!

Second, free your creativity!

![ASLTJBot](/Images/ASLTJBot_2018_two_arms.gif)

![Faccina (little face)](/Images/Faccina.jpg)

I've collected a presentation about TJBot to support activities performed at I.I.S. Galileo Galilei di Crema (CR), a secondary state school with about 1,900 students aged 14-19 working in two fields of education: “Applied Sciences high school” and “Technological high school”.

[This is the last version](ASL%20-%20TJBot%20playground%20v0.5.20180618.pptx)

This is an *early* way to share it.

I'm starting collecting and sharing student's guide and proposed exercises. Feel free to collaborate.

# Setup

For many of the proposed LABs you can use a standard TJBot or a modified one. If a different configuration is required, it will be noted at the start of the exercise.
Many exercises are based upon Node-Red. It's easy, fast, good for every kind of students (from kids to grandmas)!

## Setup a standard TJBot
Bring TJBot to life following instructions available at https://github.com/ibmtjbot/tjbot
![Bring TJBot to life](https://github.com/ibmtjbot/tjbot/raw/master/images/tjbot.jpg)

## Some tips:

* Carefully verify LED PINs layout
* If you plan to use LED, disable internal audio and use a USB audio adapter or bluetooth
* Remind your Raspberry user and password :)
* Note your TJBot IP address (if it remains the same)
* Perform all the tests
  * Connect to Raspberry (using local keyboard/screen, VNC or SSH)
  * Install TJBot test prerequisite. The following command assumes you have cloned the tjbot git repository to your Desktop.

    npm install ~/Desktop/tjbot/bootstrap/tests

  * Go in bootstrap directory:

    cd ~/Desktop/tjbot/bootstrap

  * Run full comprehensive tests for TJBot:

    ./runTests.sh

  * Or Run single test launching specific script:

    cd ~/Desktop/tjbot/bootstrap/tests
    sudo node test.camera.js
    sudo node test.led.js
    sudo node test.servo.js
    sudo node test.speaker.js

* Try some official recipes on your own *before* performing laboratories at school :)

## Let's cooking
Recipes are step-by-step instructions to bring your TJBot to life. They follow a typical structure:
![recipe structure]()

### Official recipes:
* [Use Your Voice to Control a Light with Watson!](http://www.instructables.com/id/Use-Your-Voice-to-Control-a-Light-With-Watson/)
* [Make Your Robot Respond to Emotions Using Watson!](http://www.instructables.com/id/Make-Your-Robot-Respond-to-Emotions-Using-Watson/)
* [Build a Talking Robot with Watson!](http://www.instructables.com/id/Make-Your-Robot-Respond-to-Emotions-Using-Watson/)

# Working On... 
Where I can buy more time?


# License  
This project uses the [Apache License Version 2.0](LICENSE) software license.  

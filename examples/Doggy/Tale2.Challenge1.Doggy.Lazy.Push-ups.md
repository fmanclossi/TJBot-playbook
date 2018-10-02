# Tales of two doggies
# Tale 2- Doggy likes his treats. It needs to eat healthier and start doing exercises
Doggy is a sweet tooth. It loves treats, cakes and ice cream. Also likes hamburgers, chips, pizza and pasta!  It’s getting fat, so it needs to eat healthier and start doing exercises! But it doesn’t like gymnastic!!!

[Back to Tale of two doggies MAIN INDEX](Tales%20of%20two%20doggies.md)

## Tale2.Challenge1 – Doggy is lazy and wants to skip exercises

Doggy doesn't like to do exercises. When it start a serie, if nothing is near to it, it moves its tail instead of doing push-ups. Modify previous scene to introduce this behavior.

**Requirement:** TJBot, Doggy Premium – [already setup and tested](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Setup%20Doggy%20and%20Test%20features.md)

**Skill:** Node-Red (basic level)

**Age:** 10+

**Knowledge acquired:** Servo motor and Sonar sensor usage, test condition, set value to variable, Node-red subflow, Problem decomposition

**Preparation steps (usually performed by IBMers, Teachers…):**

* point your browser to Node-Red Dashboard - http://«TJBot_ip_address»:1880

* verify that TJBot is fully functional and node-red is working as expected (TJBot credentials, too).

* verify if LOOPTIMER is installed. If not, install node-red-contrib-looptimer via “Manage Palette”

* verify that Tale2.Scene2 is enabled and working on dedicated Flow

**Macro-Steps:**

* save distance value

![save distance](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t02C01.Save.Object.Distance.jpg)

* test if anything is near

![test distance](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t02C01.Test.If.Anything.Near.jpg)

* create a new SubflowFlow called "Doggy Move Tail Right to Left" with DELAY, two change nodes and copied "TJdog Tail Pin24" from Doggy setup. Right tail position is at "0". Left is on "100" value.

![tail subflow](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t02C01.Move.Tail.SubFlow.jpg)

* connect nodes as in following picture and deploy it.

![image](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t02C01.Doggy.lazy.Flow.jpg)

What happen when you move an object in front of Doggy?

![image](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t02c01.Doggy.Lazy.PushUps.Animated.gif)

[Move to Tale of two doggies MAIN INDEX](Tales%20of%20two%20doggies.md)

[Back to main Doggy's page](https://github.com/fmanclossi/TJBot-playbook/tree/master/examples/Doggy)

# HAVE FUN and REPORT ISSUES!!! PHOTOS, VIDEOS, FEEDBACKS are WELCOME!

# License  
This project uses the [Apache License Version 2.0](../../LICENSE) software license.  

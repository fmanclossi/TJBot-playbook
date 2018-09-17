# Tales of two doggies
# TALE 2 – Doggy is a greedy pet and needs to go on diet

Doggy is a cute pet... sweet tooth, too. Cake, ice creams but also hamburgers, chips, pizza and pasta! It needs to go on diet!

[Back to Tale of two doggies MAIN INDEX](Tales%20of%20two%20doggies.md)

## Tale2.Scene1 – Stand Up, Doggy!

**Requirement:** TJBot, Doggy Premium – [already setup and tested](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Setup%20Doggy%20and%20Test%20features.md)

**Skill:** Node-Red (basic level)

**Age:** 8+

**Knowledge acquired:** Servo motor and Sonar sensor usage, test condition, set value to variable

**Preparation steps (usually performed by IBMers, Teachers…):**

* point your browser to Node-Red Dashboard - http://«TJBot_ip_address»:1880

* verify that TJBot is fully functional and node-red is working as expected (TJBot credentials, too).

* (Doggy version only) verify that Tale1.Scene4 is enabled and working on dedicated Flow

**Steps:**

* point your browser to Node-Red Dashboard - http://«TJBot_ip_address»:1880

* create a new Flow

* double-click Flow label and rename it to “Tale2.Scene1”. Press “Done” to close.

* double-click “Tale1.Scene4” Flow label and set status to “Disabled”. Press “Done” to close.

* select “Doggy Eyes” and “Less than 30cm”nodes in “Tale1.Scene4” Flow. Press CTRL+C keys to copy them. Click on “Tale2.Scene1” Flow label. Press CTRL+V keys to paste them.

* drag twice PI-GPIOD node to working area (you'll get two nodes)

* double-click PI-GPIOD nodes and configure them as shown in following pictures.
   
![Configure LEFT ARM](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/9b-Setup%20front%20legs%20flow%20-%20configure%20left%20arm%20servo%20motor.jpg)
   
![Configure RIGHT ARM](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/9b-Setup%20front%20legs%20flow%20-%20configure%20right%20arm%20servo%20motor.jpg)
     
* drag four times CHANGE node to working area and configure them as shown in picture following the table provided

![Configure CHANGE LEFT ARM DOWN ](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t02s01.Doggy.Set.CHANGE.Node.LEFT.ARM.DOWN.jpg)
   
Node | Name | Value
---- | ---- | -----
Change #1 | Set DOGGY LEFT ARM to DOWN | 100
Change #2 | Set DOGGY LEFT ARM to UP | 0
Change #3 | Set DOGGY RIGHT ARM to DOWN | 0
Change #4 | Set DOGGY RIGHT ARM to UP | 100
           
* connect and rearrange, if needed, as show in the following picture

![image]( https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t02s01.Doggy.StandUP.Flow.jpg)

* press DEPLOY button

![image](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t02s01.StandUp.Doggy.animated.gif)

What happen when an obstacle reaches Doggy?

What happen if the object stays away from Doggy?

What happen if the object stays in front of Doggy’s eyes?

**Anyone scared by Doggy? Don't panic! It's a cute dog.**

[Move to Tale of two doggies MAIN INDEX](Tales%20of%20two%20doggies.md)

[Back to main Doggy's page](https://github.com/fmanclossi/TJBot-playbook/tree/master/examples/Doggy)

# HAVE FUN and REPORT ISSUES!!! PHOTOS, VIDEOS, FEEDBACKS are WELCOME!

# License  
This project uses the [Apache License Version 2.0](../../LICENSE) software license.  

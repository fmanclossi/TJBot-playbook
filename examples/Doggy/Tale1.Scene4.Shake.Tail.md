# Tales of two doggies
# TALE 1 – Doggy barks and shake its tail if an object is less than 30cm away
Doggy is a very careful watchdog. Nothing and no one can pass without getting a strong barking.

[Back to the first scene - Tale1.Scene1](Tale1.Scene1.Say.BARK.md) - Create a flow that makes Doggy say “BARK!” if an object is less than 30cm away

[Back to the second scene - Tale1.Scene2](Tale1.Scene2.BARKING.md) – Make Doggy barking (a real barking!) if an object is less than 30cm away

[Back to the previous scene - Tale1.Scene3](Tale1.Scene3.Smart.BARKING.md) – Smart barking, just one time, please!

## Tale1.Scene4 – Shake a tail! Shake it, shake it, shake it Doggy! 

**Requirement:** TJBot, MiniDoggy, Doggy (Standard or Premium) – [already setup and tested](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Setup%20Doggy%20and%20Test%20features.md)

**Skill:** Node-Red (basic level)

**Age:** 8+

**Knowledge acquired:** Servo motor and Sonar sensor usage, test condition, set value to variable, use random values, create loop

**Preparation steps (usually performed by IBMers, Teachers…):**

* point your browser to Node-Red Dashboard - http://«TJBot_ip_address»:1880

* verify that TJBot is fully functional and node-red is working as expected (TJBot credentials, too).

* verify if LOOPTIMER is installed. If not, install node-red-contrib-looptimer via “Manage Palette”

* (Doggy version only) verify that Tale1.Scene3 is enabled and working on dedicated Flow

**Steps:**

* point your browser to Node-Red Dashboard - http://«TJBot_ip_address»:1880

* create a new Flow

* double-click Flow label and rename it to “Tale1.Scene4”. Press “Done” to close.

* (Doggy version only) double-click “Tale1.Scene3” Flow label and set status to “Disabled”. Press “Done” to close.

* (Doggy version only) select “Doggy Eyes” and “Less than 30cm”nodes in “Tale1.Scene3” Flow. Press CTRL+C keys to copy them. Click on “Tale1.Scene4” Flow label. Press CTRL+V keys to paste them.

* (MiniDoggy only) drag INJECT node to Working area. Double-click it and configure as in following picture

![image]( https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/ t01s41.Configure.INJECT.Simulating.Eyes.Nodes.jpg)

* (MiniDoggy only) drag RANDOM node to Working area. Double-click it and configure as in following picture

![image]( https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/ t01s42.Configure.RANDOM.Distance.Measurement.Nodes.jpg)

* rearrange and connect nodes

![image]( https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/ t01s43.Arrange.Nodes.jpg)

* drag LOOPTIMER node to Working area. Configure it to fire 30 times, every 0.2 seconds.

![image]( https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/ t01s44.Configure.LOOPTIMER.Nodes.jpg>

* drag RANDOM node to Working area. Configure it to send an integer between 0 and 100.

![image]( https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/ t01s45.Configure.RANDOM.Tail.Position.Nodes.jpg)

* drag PI-GPIOD node to Working Area and configure it to PIN 24 (GPIO 8)

![image]( https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/ t01s46.Configure.PI-GPIOD.TAIL.PIN24.Nodes.jpg)

* connect and rearrange, if needed, as show in the following picture

![image]( https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/ t01s47.Tail.Animated.Flow.Completed.jpg)

* press DEPLOY button

**(MiniDoggy version only)**

What happens when you press “Simulated Doggy’s Eyes” INJECT node?

![image]( https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/ t01s48.MiniDoggy.Test.Tail.Animated.Flow.Completed.jpg)

Why the tail shakes only some time and not always?

HINT: add a debug node to show “Simulated Distance Measurement” output. Call it “Distance” and press DEPLOY. Press again “Simulated Doggy’s Eyes” INJECT node 

![image]( https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/ t01s49.MiniDoggy.Test.Random.Tail.Animated.Flow.Completed.jpg)

**(Doggy version only)**

What happen when an obstacle reaches Doggy?

What happen if the object stays near Doggy?

**Funny! I challenge you to add scene3 elements to make Doggy barking and shaking tail when an object is near than 30cm. Ready… Steady… GO!**

Fantastic! Doggy is growing up smarter, step by step!

[Move to Tale of two doggies MAIN INDEX](Tales%20of%20two%20doggies.md)

[Back to main Doggy's page](https://github.com/fmanclossi/TJBot-playbook/tree/master/examples/Doggy)

# HAVE FUN and REPORT ISSUES!!! PHOTOS, VIDEOS, FEEDBACKS are WELCOME!

# License  
This project uses the [Apache License Version 2.0](../../LICENSE) software license.  

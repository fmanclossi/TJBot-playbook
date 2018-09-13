# Tales of two doggies
# TALE 1 – Doggy barks and shake its tail if an object is less than 30cm away
Doggy is a very careful watchdog. Nothing and no one can pass without getting a strong barking.

[Back to the first Scene - Tale1.Scene1 - Create a flow that makes Doggy say “BARK!” if an object is less than 30cm away](Tale1.Scene1.Say.BARK.md)

[Back to the previous Scene - Tale1.Scene2 – Make Doggy barking (a real barking!) if an object is less than 30cm away](Tale1.Scene2.BARKING.md)

## Tale1.Scene3 – Smart barking, just one time, please!

**Requirement:** TJBot, Doggy (Basic, Standard or Premium) – [already setup and tested] (https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Setup%20Doggy%20and%20Test%20features.md)

**Skill:** Node-Red (basic level)

**Age:** 8+

**Knowledge acquired:** Sonar sensor usage, test condition, set value to variable, debugging, play audio, use global variables

**Preparation steps (usually performed by IBMers, Teachers…):**

* point your browser to Node-Red Dashboard - http://«TJBot_ip_address»:1880

* verify that TJBot is fully functional and node-red is working as expected (TJBot credentials, too). 

* verify that Tale1.Scene2 is enabled and working on dedicated Flow

**Steps:**

* point your browser to Node-Red Dashboard - http://«TJBot_ip_address»:1880

* create a new Flow

* double-click Flow label and rename it to “Tale1.Scene3”. Press “Done” to close.

* double-click “Tale1.Scene2” Flow label and set status to “Disabled”. Press “Done” to close.

* select all nodes in “Tale1.Scene2” Flow drawing an area over them

* press CTRL+C keys to copy.

* click on “Tale1.Scene3” Flow label

* press CTRL+V keys to paste nodes. When you find the best place to paste them, right click to save positions.

* delete connection between SWITCH and CHANGE nodes, and make space in the flow

![image]( https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t01s31.Rearrange.Flow.jpg)

* drag twice CHANGE node to Working area. Drag SWITCH node, too.

![image]( https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t01s32.Add.CHANGE.SWITCH.Nodes.Smarter.Barking.jpg)

* double-click upper new CHANGE node and configure it as follow. Press “Done” to close.

![image]( https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t01s33.Configure.global.DogIsBarking.TRUE.CHANGE.Node.jpg)

* double-click other new CHANGE node and configure it as follow. Press “Done” to close.

![image]( https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t01s34.Configure.global.DogIsBarking.FALSE.CHANGE.Node.jpg)

* double-click new SWITCH node and configure it as follow. Press “Done” to close.

![image]( https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t01s35.Configure.SWITCH.DogIsBarking.Node.jpg)

*(if needed, rearrange nodes to make space and) connect as show in picture

![image]( https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t01s36.Connect.DogIsBarking.Nodes.jpg)

* press DEPLOY button

What happen when an obstacle reaches Doggy? As previously, Doggy start barking.

What happen if the object stays near Doggy?

What needs to happen to let Doggy barking again? 

**Awesome! Doggy is growing up smarter, step by step! It’s time to shake tail!**

[Move to the next scene - Tale1.Scene4 – Shake a tail! Shake it, shake it, shake it Doggy!](Tale1.Scene4.Shake.Tail.md)

[Back to main Doggy's page](https://github.com/fmanclossi/TJBot-playbook/tree/master/examples/Doggy)

# HAVE FUN and REPORT ISSUES!!! PHOTOS, VIDEOS, FEEDBACKS are WELCOME!

# License  
This project uses the [Apache License Version 2.0](../../LICENSE) software license.  

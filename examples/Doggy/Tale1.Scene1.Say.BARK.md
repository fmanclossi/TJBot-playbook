# Tales of two doggies
# TALE 1 – Doggy barks and shake its tail if an object is less than 30cm away
Doggy is a very careful watchdog. Nothing and no one can pass without getting a strong barking.

## Tale1.Scene1 - Create a flow that makes Doggy say “BARK!” if an object is less than 30cm away 

**Requirement:** TJBot, Doggy (Basic, Standard or Premium) – [already setup and tested](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Setup%20Doggy%20and%20Test%20features.md)

**Skill:** Node-Red (basic level)

**Age:** 8+

**Knowledge acquired:** Sonar sensor usage, test condition, set value to variable, debugging

**Preparation steps (usually performed by IBMers, Teachers…):**

* point your browser to Node-Red Dashboard - http://«TJBot_ip_address»:1880

* verify that TJBot is fully functional and node-red is working as expected. 

* disable every existing Flow (double-click each label, set Status to “Disabled”, press “Done to close”)

**Steps:**

* point your browser to Node-Red Dashboard - http://«TJBot_ip_address»:1880

* create a new Flow

![image]( https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/ t01s01.Create.New.Flow.jpg)

* double-click Flow label and rename it to “Tale1.Scene1”. Press “Done” to close.

* drag PI-SRF node to the working area

![image]( https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t01s02.Add.PI-SRF.Node.jpg)

* double-click PI-SRF node and configure it as shown in the following picture

![image]( https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t01s03.Configure.PI-SRF.Node.jpg)

* drag a SWITCH node to the working area

![image]( https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t01s04.Add.SWITCH.Node.jpg)

* double-click SWITCH node and configure it as shown in the following picture

![image]( https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t01s05.Configure.SWITCH.Node.jpg)

* drag a line from the output of the first node to the input of the second one

![image]( https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t01s06.Connect.PI-SRF.to.SWITCH.Node.jpg)

* drag a CHANGE node to the working area

![image]( https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t01s07.Add.CHANGE.Node.jpg)

* configure CHANGE node setting the message to “BARK!”

![image]( https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t01s08.Configure.CHANGE.Node.to.BARK.jpg)

* connect the first output from SWITCH node to the input of CHANGE one

![image]( https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t01s09.Connect.SWITCH.to.CHANGE.Node.jpg)

* drag a DEBUG node to the working area

![image]( https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t01s10.Add.DEBUG.Node.jpg)

* connect its input to the output of CHANGE node

![image]( https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t01s11.Connect.CHANGE.to.DEBUG.Node.jpg)

* press DEPLOY button and switch to “debug” tab (if not already highlighted)

![image]( https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t01s12.Press.DEPLOY.switch.DEBUG.jpg)

**What happen when you put an object near to Doggy’s eyes?**

![image]( https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t01s13.Put.Object.Less30cm.jpg)

Excellent! But we want a strong bark not a text on dashboard.

[Move to the next scene](Tale1.Scene2.BARKING.md)

[Back to main Doggy's page](https://github.com/fmanclossi/TJBot-playbook/tree/master/examples/Doggy)

# HAVE FUN and REPORT ISSUES!!! PHOTOS, VIDEOS, FEEDBACKS are WELCOME!

# License  
This project uses the [Apache License Version 2.0](../../LICENSE) software license.  

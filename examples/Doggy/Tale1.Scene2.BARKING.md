# Tales of two doggies
# TALE 1 – Doggy barks and shake its tail if an object is less than 30cm away
Doggy is a very careful watchdog. Nothing and no one can pass without getting a strong barking.

[Back to the previous Scene - Tale1.Scene1 - Create a flow that makes Doggy say “BARK!” if an object is less than 30cm away](Tale1.Scene1.Say.BARK.md)

## Tale1.Scene2 – Make Doggy barking (a real barking!) if an object is less than 30cm away 

**Requirement:** TJBot, Doggy (Basic, Standard or Premium) – already setup and tested (https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Setup%20Doggy%20and%20Test%20features.md)

**Skill:** Node-Red (basic level)

**Age:** 8+

**Knowledge acquired:** Sonar sensor usage, test condition, set value to variable, debugging, play audio

**Preparation steps (usually performed by IBMers, Teachers…):**

* point your browser to Node-Red Dashboard - http://«TJBot_ip_address»:1880

* verify that TJBot is fully functional and node-red is working as expected (TJBot credentials, too). 

* verify that Tale1.Scene1 is enabled on dedicated Flow

* get a good sound file (WAV format) with a dog barking (e.g. dogbark2.wav from https://www.freesoundeffects.com/free-sounds/dogs-10026/)

* upload bark sound file to TJBot Desktop using VNC file transfer feature, an USB Key or whatever you like (e.g. /home/pi/Desktop/dogbark2.wav). P.S: You can download it directly using TJBot browser :D

* test TJBot speaker with bark audio file

**Steps:**

* point your browser to Node-Red Dashboard - http://«TJBot_ip_address»:1880

* create a new Flow

* double-click Flow label and rename it to “Tale1.Scene2”. Press “Done” to close.

* double-click “Tale1.Scene1” Flow label and set status to “Disabled”. Press “Done” to close.

![image]( https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t01s20.Disable.T1S1.Flow.jpg)

* select all nodes in “Tale1.Scene1” Flow drawing an area over them

![image]( https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t01s21.Select.All.Nodes.in.T1S1.Flow.jpg )

* press CTRL+C keys to copy.

* click on “Tale1.Scene2” Flow label

* press CTRL+V keys to paste nodes. When you find the best place to paste them, right click to save positions.

* delete DEBUG node (click on it and press DEL key)

![image]( https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t01s22.Delete.DEBUG.node.jpg)

* double-click SWITCH node and modify it as shown in the following picture

![image]( https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t01s22.Change.SWITCH.Setting.Audio.Path.jpg)

* drag SPEAK node (from TJBot palette) to the Working area

![image]( https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t01s23.Add.TJBOT.SPEAK.Node.jpg)

* double-click SPEAK node, select BOT according to your environment, set MODE to “Play” and set NAME to “Bark”

![image]( https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t01s24.Configure.TJBOT.SPEAK.Node.jpg)

* connect it to CHANGE node and press DEPLOY button

![image]( https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t01s25.Connect.CHANGE.to.SPEAK.Node.jpg)

Do you get a strong barking when you put an object near to Doggy’s eyes? If not, very prerequisites (e.g. audio power turned on 😊 )

What happen if the object stays near Doggy?

**Congratulation! You’re ready to move to the next level! Let’s make Doggy a little smarter!**

[Move to the next scene - Tale1.Scene3 – Smart barking, just one time, please!](Tale1.Scene3.Smart.BARKING.md)

[Back to main Doggy's page](https://github.com/fmanclossi/TJBot-playbook/tree/master/examples/Doggy)

# HAVE FUN and REPORT ISSUES!!! PHOTOS, VIDEOS, FEEDBACKS are WELCOME!

# License  
This project uses the [Apache License Version 2.0](../../LICENSE) software license.  

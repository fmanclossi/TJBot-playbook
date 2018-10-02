# Tales of two doggies
# TALE 1 – Doggy barks and wags its tail if an object is less than 30cm away
Doggy is a very careful watchdog. Nothing and no one can pass without getting a strong barking.

[Back to Tale of two doggies MAIN INDEX](Tales%20of%20two%20doggies.md)

## Tale1.Scene5 – TJBot wakes up when Doggy start barking and calms it down 

**Requirement:** TJBot, Doggy Premium – [already setup and tested](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Setup%20Doggy%20and%20Test%20features.md)

**Skill:** Node-Red (basic level)

**Age:** 10+

**Knowledge acquired:** Servo motor and Sonar sensor usage, test condition, set value to variable, TJBot capabilities (Text to Speech, Visual Recognition, Wave)

**Preparation steps (usually performed by IBMers, Teachers…):**

* point your browser to Node-Red Dashboard - http://«TJBot_ip_address»:1880

* verify that TJBot is fully functional and node-red is working as expected (TJBot credentials, too).

* (Doggy version only) verify that Tale1.Scene3 worked fine.

**There are several steps blocks in this scene according to Doggy version used**

**Steps (part 1):**

* point your browser to Node-Red Dashboard - http://«TJBot_ip_address»:1880

* create a new Flow

* double-click Flow label and rename it to “Tale1.Scene5”. Press “Done” to close.

* disable any other active flow.

* select all nodes in “Tale1.Scene3” Flow. Press CTRL+C keys to copy them. Click on “Tale1.Scene5” Flow label. Press CTRL+V keys to paste them.

**Steps (part 2 - opional - Doggy Premium only):**

* drag twice PI-GPIOD node to working area (you'll get two nodes)

* double-click PI-GPIOD nodes and configure them as shown in following pictures.
   
![Configure LEFT ARM](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/9b-Setup%20front%20legs%20flow%20-%20configure%20left%20arm%20servo%20motor.jpg)
   
![Configure RIGHT ARM](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/9b-Setup%20front%20legs%20flow%20-%20configure%20right%20arm%20servo%20motor.jpg)
     
* duplicate PI_GPIOD nodes
	 
* drag four times CHANGE node to working area and configure them as shown in picture following the table provided

![Configure CHANGE LEFT ARM DOWN ](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t02s01.Doggy.Set.CHANGE.Node.LEFT.ARM.DOWN.jpg)
   
Node | Name | Value
---- | ---- | -----
Change #1 | Set DOGGY LEFT ARM to DOWN | 100
Change #2 | Set DOGGY LEFT ARM to UP | 0
Change #3 | Set DOGGY RIGHT ARM to DOWN | 0
Change #4 | Set DOGGY RIGHT ARM to UP | 100
           
* connect and rearrange, if needed, as show in the following picture.

![image]( https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t01s05.Doggy.StandUP.Flow.jpg)

* press DEPLOY button. What happens moving object in front of Doggy?

![image]( https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t01s05.Doggy.StandUP.Animated.gif)

(**IBMers/Teachers TIP:** introduce comment nodes - Things can grow up very fast and one comment can save your life)

**Steps (part 3):** Let's TJBot take on the stage!

* drag once OUTPUT LINK node to working area beside SPEAK node

* drag one INPUT LINK node to working area below the flow. Double-click it and name it "Doggy is barking"

* double-click OUTPUT NODE and link it to "Doggy is barking" LINK
     
![Configure LINK](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t01s05.Link.Nodes.Barking.Waking.jpg)
   
* drag TJBot's SEE and SPEAk, Function (and DEBUG) nodes from Palette and connect them as in picture

![Configure TJBot identify and speak actions ](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t01s05.TJBot.SEE.and.SPEAK.jpg)
   
* configure SEE, SPEAK and FUNCTION nodes as following

![Configure SEE ](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t01s05.Configure.SEE.node.jpg)
   
![Configure SPEAK ](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t01s05.Configure.SPEAK.node.jpg)
   
![Configure FUNCTION ](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t01s05.Configure.FUNCTION.node.Visual.Recognition.jpg)
   
This is the code inserted in FUNCTION to copy and paste:

`Calm down, Doggy. That's only a {{payload.0.class}} !`
	 
* drag twice TJBot's SHINE node to Working area. Connect and configure them as shown in following picture.
	
![image]( https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t01s05.TJBot.SEE.and.SPEAK.and.SHINE.jpg)

* press DEPLOY button. What happens moving object in front of Doggy? What happens if an object goes away and then back while TJBot is talking?

Probably you (or your students) noticed that Doggy and TJBot try to identify multiple objects mixing barking and speaking. This is bad.

(**IBMers/Teachers hint: this is the same solution used in [Tale2.Scene2](Tale2.Scene2.Doggy.Push-ups.md) - look at it to get the details)

* change flow as in following picture and retry (changed nodes are highlighted). TJBot and Doggy are more realistic?

![image]( https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t01s05.Doggy.wakes.TJBot.Fixed.Flow.jpg)

**Steps (part 4):** Doggy is calmed and happy
When Doggy is calm, it wags its tail and go down on its belly.

* modify flow as shown in the following figure (hint: copy nodes from previous flow)

![image]( https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t01s05.Doggy.wakes.TJBot.Calm.Down.Flow.jpg)


What happen when an obstacle reaches Doggy?

What happen if the object stays away from Doggy?

What happen if the object stays in front of Doggy’s eyes?

![Calm down, Doggy](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t01s05.TJBot.waked.up.Calm.Down.Doggy_with_TEXT.gif)

[click to run video from YouTube](https://youtu.be/5DM6FVKDyXQ)

[Move to Tale of two doggies MAIN INDEX](Tales%20of%20two%20doggies.md)

[Back to main Doggy's page](https://github.com/fmanclossi/TJBot-playbook/tree/master/examples/Doggy)

# HAVE FUN and REPORT ISSUES!!! PHOTOS, VIDEOS, FEEDBACKS are WELCOME!

# License  
This project uses the [Apache License Version 2.0](../../LICENSE) software license.  

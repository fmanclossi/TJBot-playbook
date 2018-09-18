# Tales of two doggies
# TALE 2 – Doggy is a greedy pet and needs to go on diet

Doggy is a cute pet... sweet tooth, too. Cake, ice creams but also hamburgers, chips, pizza and pasta! It needs to go on diet!

[Back to Tale of two doggies MAIN INDEX](Tales%20of%20two%20doggies.md)

## Tale2.Scene2 – Doggy trying to do push-ups - Doggy does push-ups when anything is less that 30cm away

**Requirement:** TJBot, Doggy Premium – [already setup and tested](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Setup%20Doggy%20and%20Test%20features.md)

**Skill:** Node-Red (basic level)

**Age:** 10+

**Knowledge acquired:** Servo motor and Sonar sensor usage, test condition, set value to variable, Node-red subflow, Problem decomposition

**Preparation steps (usually performed by IBMers, Teachers…):**

* point your browser to Node-Red Dashboard - http://«TJBot_ip_address»:1880

* verify that TJBot is fully functional and node-red is working as expected (TJBot credentials, too).

* verify if LOOPTIMER is installed. If not, install node-red-contrib-looptimer via “Manage Palette”

* verify that Tale2.Scene1 is enabled and working on dedicated Flow

**Steps (part 1 - just one push-up!):**

* point your browser to Node-Red Dashboard - http://«TJBot_ip_address»:1880

* create a new Flow

* double-click Flow label and rename it to “Subflow working area”. Press “Done” to close.

* double-click “Tale2.Scene1” Flow label and set status to “Disabled”. Press “Done” to close.

* select all nodes in “Tale2.Scene1” Flow. Press CTRL+C keys to copy them. Click on “Subflow working area” Flow label. Press CTRL+V keys to paste them.

* select "Set Doggy LEFT ARM DOWN", "Set Doggy RIGHT ARM DOWN", "TJDog LEFT ARM Pin38" and "TJDog RIGHT ARM Pin40" nodes keeping CTRL pressed while clicking on them.

* Copy them on the same flow and select them

* Click on Node-Red Menu, click on SUBFLOWS, and select "Selection to SubFlow". Selection will be substituted by a new node, that appears even in palette area.

![Create subflow from selected nodes](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t02s02.Create.Subflow.From.Selected.Nodes.jpg)

![Created subflow - default](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t02s02.Created.Subflow.Default.Name.jpg)

* double-click on created subflow in the Palette area. It opens in Working area and could be edited. Click on value "1" in Inputs selector and connect new input node to CHANGE nodes

![Add input to Created subflow](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t02s02.Add.Input.to.SubFlow.jpg)

![Connect input to nodes](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t02s02.Connect.Input.to.Nodes.jpg)

* Click on "Edit Properties" and change name to "Doggy Stand-Up". Press "Done" to close and close subflow editor.

![Connect input to nodes](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t02s02.Change.SubFlow.Name.jpg)

![Connect input to nodes](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t02s02.Doggy.StandUP.Subflow.jpg)

* do the same again with "Set Doggy LEFT ARM UP", "Set Doggy RIGHT ARM UP", "TJDog LEFT ARM Pin38" and "TJDog RIGHT ARM Pin40", creating a new subflow called "Doggy Sit Down". In the same way, you can create basic Doggy actions (shake.tail, bark...).

![Connect input to nodes](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t02s02.Doggy.SitDOWN.Subflow.jpg)

* delete “Subflow working area” flow

* create a new Flow

* double-click Flow label and rename it to “Tale2.Scene2”. Press “Done” to close.

* double-click “Tale2.Scene1” Flow label.

* select “Doggy Eyes” and “Less than 30cm”nodes in “Tale2.Scene1” Flow. Press CTRL+C keys to copy them. Click on “Tale2.Scene2” Flow label. Press CTRL+V keys to paste them.

* now, start little, just one push-up! From palette, drag "Doggy Stand Up" and "Doggy Sit Down" subflows to Working area. Drag DELAY node, too. Double-click it and set a 1 second delay. Connect nodes as show in figure.

![image]( https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t02s02.Doggy.One.PushUP.Flow.jpg)

* press DEPLOY button

![image](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t02s01.StandUp.Doggy.animated.gif)

What happen when an obstacle reaches Doggy?

What happen if the object stays away from Doggy?

What happen if the object stays in front of Doggy’s eyes?

**Doggy has to do more exercise :)**

Now, we have to count push-ups and start a serie only if the previous one was terminated. We used flow variables to keep how many push-ups did Doggy.

**Steps (part 2 - 10 push-ups):**

* create a subflow called "Doggy Push-Up" using "Doggy Stand Up","Doggy Sit Down" and "delay 1s" nodes. Modify “Tale2.Scene2” flow using new created subflow.

![image](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t02s02.Doggy.PushUP.Subflow.jpg)

![image](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t02s02.Doggy.One.PushUP.Flow.With.Subflow.jpg)

* delete connection between SWITCH and "Doggy Push-Up"

* drag once CHANGE node from Palette to Working area. Modify it as shown in figure

![image](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t02s02.Reset.PushUps.Count.jpg)

* drag once SWITCH node from Palette to Working area. Modify it as shown in figure

![image](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t02s02.Check.New.Serie.jpg)

* drag another SWITCH node from Palette to Working area. Modify it as shown in figure

![image](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t02s02.Check.If.More.Pushups.jpg)

* drag once FUNCTION node from Palette to Working area. Modify it as shown in figure, inserting the following code that set/increase pushups count:

`var myCount = flow.get("pushups") || 0;

myCount += 1;

flow.set("pushups", myCount);

return msg;`

![image](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t02s02.Increase.Pushups.Count.jpg)

* drag once DELAY node from Palette to Working area. Set delay to 2 seconds.

* Connect nodes as show in figure. Pay attention to create the loop!

![image]( https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t02s02.Doggy.PushUP.Series.Flow.jpg)

* we need to instanciate count variable (**teacher/IBMers, evaluate how to introduce this concept to classroom**). Drag once INJECT node to Working area and copy "reset push-up count" node. Configure INJECT node as follow and connect nodes.

![image](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t02s02.Instanciate.PushUP.Series.INJECT.jpg)

![image](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t02s02.Instanciate.PushUP.Series.Flow.jpg)

* press DEPLOY button

![image](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t02s02.Doggy.PushUps.Animated.gif)

What happen when an obstacle reaches Doggy?


**Anyone scared by Doggy? Don't panic! It's a cute dog.**

[Move to Tale of two doggies MAIN INDEX](Tales%20of%20two%20doggies.md)

[Back to main Doggy's page](https://github.com/fmanclossi/TJBot-playbook/tree/master/examples/Doggy)

# HAVE FUN and REPORT ISSUES!!! PHOTOS, VIDEOS, FEEDBACKS are WELCOME!

# License  
This project uses the [Apache License Version 2.0](../../LICENSE) software license.  

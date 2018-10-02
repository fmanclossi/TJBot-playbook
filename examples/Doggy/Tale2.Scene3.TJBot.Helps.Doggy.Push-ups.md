# Tales of two doggies
# Tale 2- Doggy likes his treats. It needs to eat healthier and start doing exercises
Doggy is a sweet tooth. It loves treats, cakes and ice cream. Also likes hamburgers, chips, pizza and pasta!  It’s getting fat, so it needs to eat healthier and start doing exercises! But it doesn’t like gymnastic!!!

[Back to Tale of two doggies MAIN INDEX](Tales%20of%20two%20doggies.md)

## Tale2.Scene3 – When anything is less that 30cm away, TJBot start counting push-ups for Doggy

**Requirement:** TJBot, Doggy Premium – [already setup and tested](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Setup%20Doggy%20and%20Test%20features.md)

**Skill:** Node-Red (basic level)

**Age:** 10+

**Knowledge acquired:** Text to Speech, TJBot capabilities (wave, speak)

**Preparation steps (usually performed by IBMers, Teachers…):**

* point your browser to Node-Red Dashboard - http://«TJBot_ip_address»:1880

* verify that TJBot is fully functional and node-red is working as expected (TJBot credentials, too).

* verify that Tale2.Scene2 is enabled and working on dedicated Flow

**Steps (part 1 - TJBot speaks):**

* point your browser to Node-Red Dashboard - http://«TJBot_ip_address»:1880

* create a new Flow

* double-click Flow label and rename it to “Tale2.Scene3”. Press “Done” to close.

* double-click “Tale2.Scene2” Flow label and set status to “Disabled”. Press “Done” to close.

* select all nodes in “Tale2.Scene2” Flow. Press CTRL+C keys to copy them. Click on “Tale2.Scene3” Flow label. Press CTRL+V keys to paste them.

*  drag FUNCTION node to Working area and modify it to create a message that inclused the current number of push-ups performed by Doggy.

![image]( https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t02s03.Create.Text.With.pushup.count.jpg)

* drag TJBot's SPEAK node to Working area connecting it 

![image]( https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t02s03.Create.SPEAK.Node.jpg)

* configure TJBot's SPEAK node according with yout TJBot configuration (TTS credential, HW setup...) 

![image]( https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t02s03.Configure.SPEAK.Node.jpg)

* Rearrange nodes as in the following picture and press DEPLOY button. What happen when an obstacle reaches Doggy? Is TJBot in synch with Doggy execises? 

(**Note for Teacher/IBMers: this is a good chance to explain local vs central processing...**)

![image]( https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t02s03.TJBot.Helps.Doggy.jpg)

How can we get TJBot and Doggy more synched?

(**IBMers/Teachers: try to connect Doggy subflow to a different node**)

[click for one candidate solution]( https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t02s03.TJBot.Helps.Doggy.jpg)

Amazing!

[Move to Tale of two doggies MAIN INDEX](Tales%20of%20two%20doggies.md)

[Back to main Doggy's page](https://github.com/fmanclossi/TJBot-playbook/tree/master/examples/Doggy)

# HAVE FUN and REPORT ISSUES!!! PHOTOS, VIDEOS, FEEDBACKS are WELCOME!

# License  
This project uses the [Apache License Version 2.0](../../LICENSE) software license.  

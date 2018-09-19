# Tales of two doggies
# TALE 2 – Doggy is a greedy pet and needs to go on diet

Doggy is a cute pet... sweet tooth, too. Cake, ice creams but also hamburgers, chips, pizza and pasta! It needs to go on diet!

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

![image]( https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t02s03.Create.SPEAK.Node.jpg)

* press DEPLOY button. What happen when an obstacle reaches Doggy? Is TJBot in synch with Doggy execises? (**Note for Teacher/IBMers: this is a good chance to explain local vs central processing... **)

* Rearrange nodes as in the following picture. Are TJBot and Doggy more synched?

![image]( https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Tales/t02s03.TJBot.Helps.Doggy.jpg)

Amazing!

**Anyone scared by Doggy? Don't panic! It's a cute dog.**

[Move to Tale of two doggies MAIN INDEX](Tales%20of%20two%20doggies.md)

[Back to main Doggy's page](https://github.com/fmanclossi/TJBot-playbook/tree/master/examples/Doggy)

# HAVE FUN and REPORT ISSUES!!! PHOTOS, VIDEOS, FEEDBACKS are WELCOME!

# License  
This project uses the [Apache License Version 2.0](../../LICENSE) software license.  

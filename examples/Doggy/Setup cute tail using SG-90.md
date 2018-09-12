# How to Setup and Test Doggy tail (SG-90)

* Apply to: MiniDoggy, Doggy Standard, Doggy Premium

Doggy is a cute dog! It has tail that shakes to show its happyness. A little servo motor (SG-90) moves the tail.

![SG-90](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/5.SG-90.jpg)

Using SG-90 in Node-Red is very easy!

* follow wiring instructions for your Doggy version as provided in [Mount instructions](https://github.com/fmanclossi/TJBot-playbook/tree/master/examples/Doggy). **Note:** If you've changes PINs connections, change the following example according to your different layout.

* point your browser to Node-Red URL  - http://«TJBot_ip_address»:1880

* verify that TJBot is fully functional and node-red is working as expected.

* install node-red-node-pisrf node to manage HC-SR04 and superdog vision. 

   * open Node-Red Dashboard.
   
   * click on Menu

   * select MANAGE PALETTE
   
   ![Node-Red palette](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/1.Manage%20Node-Red%20Palette.png)

   * choose INSTALL tab
   
   * search package inserting "pigpiod" test in search field
   
   ![install pigpiod](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/6.install%20node-red%20gpiod.png)
   
   * push INSTALL button and wait successful installation.
   
   * press CLOSE to return to Node-Red dashboard.
   
* **take away Doggy's tail.** We have to set the right position to avoid damages to it.
   
* tune tail position creating the following flow using PI-GPIOD and INJECT nodes

   * drag three times INJECT node to working area (you'll get three nodes); drag PI-GPIOD node, too. Connect INJECT nodes to PI-GPIOD.
   
   ![Tail tune flow unset](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/6a-Setup%20tail%20flow%20-%20drag%20nodes.jpg)
        
   * double-click the first INJECT node and configure it as shown in picture. It change name to "Set TAIL to CENTER"

   ![Configure INJECT](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/6b-Setup%20tail%20flow%20-%20set%20tail%20to%20center.jpg)
   
   * as before, configure other INJECT nodes with 0 and 100 integer value. New names will be "Set TAIL to RIGHT" and "Set TAIL to LEFT".
        
   * double-click PI-GPIOD node and configure it as shown in picture.
   
   ![Configure RPI-GPIOD](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/7.configure%20node-red%20pi-gpiod%20node.png)
   
   * push DEPLOY button.
   
   ![Tail tune flow](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/8-Setup%20tail%20flow%20-%20put%20tail%20to%20center%20position.jpg)
   
* Push "Set TAIL to CENTER" inject node. Servo motor should reach middle position. Attach tail to Doggy in RAISED position.
 
* Push "Set TAIL to LEFT" inject node. Does tail move to Doggy's left side? If not, verify that servo is mounted as described in [provided instructions](https://github.com/fmanclossi/TJBot-playbook/tree/master/examples/Doggy#mount-your-doggy) according with your Doggy's version.
 
* Push "Set TAIL to RIGHT" inject node. Does tail move to Doggy's right side? If not, verify that servo is mounted as described in [provided instructions](https://github.com/fmanclossi/TJBot-playbook/tree/master/examples/Doggy#mount-your-doggy) according with your Doggy's version.

* That’s all! We’re ready to buid a story with Doggy's superdog eyes!

![Doggies with supereyes!](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Doggies%20with%20supereyes.jpg)


## Credits

...

# HAVE FUN and REPORT ISSUES!!! PHOTOS, VIDEOS, FEEDBACK are WELCOME!

# License  
This project uses the [Apache License Version 2.0](../../LICENSE) software license.  
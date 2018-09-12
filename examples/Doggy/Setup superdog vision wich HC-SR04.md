# How to Setup and Test Doggy superdog vision (HC-SR04)

* Apply to: Doggy Basic, Doggy Standard, Doggy Premium

Doggy is a superdog! It has a supervision powered by a very easy to use sensor named HC-SR04. This is a ultrasonic sonar. It emits a sound that travels through the air. If there is an object on its path, the sound will bounce back to the sensor that evaluate travel time to calculate how far is the object. HC-SR04 is able to detect object from 2cm to 400cm (1” to 13 feet).

![HC-SR04](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Ultrasonic-Sensor-HC-SR04.jpg)

Using HC-SR04 in Node-Red is very easy!

* follow wiring instructions for your Doggy version as provided in [Mount instructions](https://github.com/fmanclossi/TJBot-playbook/tree/master/examples/Doggy). **Note:** If you've changes PINs connections, change the following example according to your different layout.

* point your browser to Node-Red URL  - http://«TJBot_ip_address»:1880

* verify that TJBot is fully functional and node-red is working as expected.

* install node-red-node-pisrf node to manage HC-SR04 and superdog vision. 

   * open Node-Red Dashboard.
   
   * click on Menu

   * select MANAGE PALETTE
   
   ![Node-Red palette](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/1.Manage%20Node-Red%20Palette.png)

   * choose INSTALL tab
   
   * search package inserting "pisrf" test in search field
   
   ![install pisrf](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/2.install%20node-red%20pisrf.png)
   
   * push INSTALL button and wait successful installation.
   
   * press CLOSE to return to Node-Red dashboard.
   
* test superdog vision creating the following flow using RPI-SRF and DEBUG nodes

   * drag RPI-SRF node to working area; drag DEBUG node, too. Connect RPI-SRF to DEBUG.
   
   * double-click RPI-SRF node and configure as shown in picture.
   
   ![Configure RPI-SRF Node](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/3.configure%20rpi-srf%20node.png)
   
   * push DEPLOY button and verify that in the DEBUG area you'll get the distance (in centimeters) between Doggy's head and an obstacle.
   
   ![HC-R04 test flow](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/4.configure%20and%20test%20superdog%20vision.png)
 
* That’s all! We’re ready to buid a story with Doggy's superdog eyes!


## Credits

...

# HAVE FUN and REPORT ISSUES!!! PHOTOS, VIDEOS, FEEDBACK are WELCOME!

[Back to setup and test page](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Setup%20Doggy%20and%20Test%20features.md)

# License  
This project uses the [Apache License Version 2.0](../../LICENSE) software license.  

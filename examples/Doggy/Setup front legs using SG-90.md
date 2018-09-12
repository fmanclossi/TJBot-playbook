# How to Setup and Test Doggy front legs (2 x SG-90)

* Apply to: Doggy Premium

Doggy Premium is a strong dog! It can raise up on its front legs to intimidate unkown object and people. Two little servo motors (SG-90) powers front legs.

![SG-90](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/5.SG-90.jpg)

Using SG-90 in Node-Red is very easy!

* follow wiring instructions for Doggy Premium as provided in [Mount instructions](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Create%20Doggy%20Premium.md). **Note:** If you've changes PINs connections, change the following example according to your different layout.

* point your browser to Node-Red URL  - http://«TJBot_ip_address»:1880

* verify that TJBot is fully functional and node-red is working as expected.

* install node-red-node-pi-gpiod node to manage SG-90 servo motors. 

   * open Node-Red Dashboard.
   
   * click on Menu

   * select MANAGE PALETTE
   
   ![Node-Red palette](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/1.Manage%20Node-Red%20Palette.png)

   * choose INSTALL tab
   
   * search package inserting "pigpiod" test in search field
   
   ![install pigpiod](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/6.install%20node-red%20gpiod.png)
   
   * push INSTALL button and wait successful installation.
   
   * press CLOSE to return to Node-Red dashboard.
   
* **take away Doggy's legs.** We have to set the right position to avoid damages to them.

![Doggy without front legs](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Doggy%20Premium%20tune%20arms%20positions.jpg)
   
* tune legs position creating the following flow using PI-GPIOD and INJECT nodes

   * drag four times INJECT node to working area (you'll get four nodes); drag twice PI-GPIOD node, too (You'll get two nodes). Connect two INJECT nodes per PI-GPIOD.
   
   ![front legs tune flow unset](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/9a-Setup%20front%20legs%20flow%20%20not%20configured.jpg)
        
   * double-click the first INJECT node and configure it as shown in picture. It changes name to "Set DOGGY LEFT ARM to DOWN"

   ![Configure INJECT #1](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/9c-Setup%20front%20legs%20flow%20-%20set%20left%20arm%20to%20DOWN.jpg)
   
   * as before, configure other INJECT nodes according with the following table
   
   Node | Name | Value
   ---- | ---- | -----
   Inject #2 | Set DOGGY LEFT ARM to UP | 0
   Inject #3 | Set DOGGY RIGHT ARM to DOWN | 0
   Inject #4 | Set DOGGY RIGHT ARM to UP | 100
           
   * double-click PI-GPIOD nodes and configure them as shown in following pictures.
   
   ![Configure LEFT ARM](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/9b-Setup%20front%20legs%20flow%20-%20configure%20left%20arm%20servo%20motor.jpg)
   
   ![Configure RIGHT ARM](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/9b-Setup%20front%20legs%20flow%20-%20configure%20right%20arm%20servo%20motor.jpg)
   
   * push DEPLOY button.
   
   ![Front legs tune flow](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/9c-Setup%20front%20legs%20flow%20-%20finished%20-%20down.jpg)
   
* Push "Set DOGGY LEFT ARM to UP" and "Set DOGGY RIGHT ARM to UP" inject nodes. Attach front legs to let Doggy to its belly.

![UP Position](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Doggy%20Premium%20arms%20UP.jpg)
 
* Push "Set DOGGY LEFT ARM to DOWN" and "Set DOGGY RIGHT ARM to DOWN" inject nodes. Does DOGGY raised up? If not, verify that servos are mounted as described in [provided instructions](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Create%20Doggy%20Premium.md).

* That’s all! We’re ready to buid a story using Doggy's front legs!

![Doggy DOWN!](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Media/Doggy%20Premium%20arms%20DOWN.jpg)


## Credits

...

# HAVE FUN and REPORT ISSUES!!! PHOTOS, VIDEOS, FEEDBACK are WELCOME!

[Back to setup and test page](https://github.com/fmanclossi/TJBot-playbook/blob/master/examples/Doggy/Setup%20Doggy%20and%20Test%20features.md)

# License  
This project uses the [Apache License Version 2.0](../../LICENSE) software license.  

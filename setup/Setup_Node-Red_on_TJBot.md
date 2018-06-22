For many of the proposed LABs you can use a standard TJBot. You can program it with Node.js language. It's not complicated... but Node-Red is more friendly, easy to learn and play.

Node-RED is a flow-based development tool developed by Nick O’Leary and Dave Conway-Jones of IBM’s Emerging Technology Services group for wiring together hardware devices, APIs and online services as part of the Internet of Things. Node-RED provides a browser-based flow editor, which can be used to create JavaScript code.

# Prereq
Remind that you need to have an already setup TJBot. Jump here to setup a [standard TJBot](Setup_standard_TJBot.md).

# Credits
This is my humble summary of the excellent work by JeanCarl Bisson, an IBM Developer Advocate. ![JeanCarlBisson](https://cdn-images-1.medium.com/fit/c/60/60/1*tocg1dafjcMwYIKG8wnpww.jpeg).

You can reach him on [Github Repository](https://github.com/jeancarl/node-red-contrib-tjbot).

JeanCarl also created a wonderful [Medium series on Node-Red and TJBot](https://medium.com/@jeancarlbisson/how-to-train-your-tjbot-in-node-red-88bfb3bbe0ab) where he explains how to setup and use his Node-Red nodes with YouTube videos and ready-to-use code.

# Setup Node-Red on TJBot
* Upgrade Node-RED preinstalled with Raspbian Jessie using the command below.

`bash <(curl -sL https://raw.githubusercontent.com/node-red/raspbian-deb-package/master/resources/update-nodejs-and-nodered)`

* Setup Node-Red to run when the Pi boots up, run:

`sudo systemctl enable nodered.service`

`sudo node test.led.js`

* Then, install TJBot nodes from JeanCarl repository:

`cd .node-red`

`mkdir nodes`

`cd nodes`

`git clone https://github.com/jeancarl/node-red-contrib-tjbot`

`cd node-red-contrib-tjbot`

`npm install`

`sudo nano /lib/systemd/system/nodered.service # some TJBot actions has to run as root so change User from pi to root`

`sudo systemctl daemon-reload`

`node-red-start # check node-red environment. Settings file should be at /root/.node-red/settings.js `

`node-red-stop`

`mkdir /home/pi/Desktop/tjbot/Pictures # place to host static content from top level URL`

`sudo nano /root/.node-red/settings.js. `

* Modify /root/.node-red/settings.js to point to the original Node-RED directory uncommenting and setting userDir and nodesDir variables as 

`userDir: '/home/pi/.node-red/’,`

`nodesDir: '/home/pi/.node-red/nodes’,`

`httpStatic: ‘/home/pi/Desktop/tjbot/Pictures/’`

* Restart Node-Red environment

`node-red-start `

* Point your browser to Node-Red URL (http://«TJBot_ip_address»:1880 and verify that nodes for TJBot are available.

# License  
This project uses the [Apache License Version 2.0](https://github.com/fmanclossi/TJBot-playbook/blob/master/LICENSE) software license.  

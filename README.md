# Bean Demo Flows
Flows used to take data from a PunchThrough Bean push it to the cloud.  Uses Node-RED, AT&amp;T Flow Designer, and AT&amp;T M2X.

In a nutshell
-----------------
The bean_edge flow runs in Node-RED at the edge, directly communicating with the Bean and sending its data up to the cloud flow.  Then, the bean_cloud_flow handles that data, saving it to M2X.  It can easily be changed to send to almost any other data storage service.

Prerequisites
-------------
1. To use these flows you will need a Punch Through Bean sensor tag.  https://punchthrough.com/bean
2. You will need a edge Node-RED flow on your computer or laptop.  See the other part of this project.
3. You will need a free AT&T Developer Account.  http://developer.att.com/

Additional information
----------------------
To use these flows you will need to create a device in M2X and configure the M2X node in this flow with the appropriate API key.  Put the device ID from M2X in the edge flow in Node-RED.  In M2X you'll also need to create 3 streams for numeric data: Temperature, X-Axis, and Y-Axis.

The bean_edge flow runs in Node-RED on your computer and connects to the Bean directly over Bluetooth.  If you change the name of your Bean you will need to configure the nodes to connect to it.

Both flows are imported using the top-right menu in their respective UIs.

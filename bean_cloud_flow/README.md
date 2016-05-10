Bean Demo - Cloud Flow
====================

In a nutshell
-----------------
This AT&T Flow Designer flow provides the connectivity from the edge flow for the Bean up through storing data in M2X.

Prerequisites
-------------
1. To use this flow you will need a Punch Through Bean sensor tag.  https://punchthrough.com/bean
2. You will need a edge Node-RED flow on your computer or laptop.  See the other part of this project.
3. You will need a free AT&T Developer Account.  http://developer.att.com/

Flow description
-----------------
This flow takes in input from a MQTT channel - one for temperature data and one for accelerometer data.  It formats the payloads for M2X and then sends both sets of data to a single device in M2X.

Additional information
----------------------
To use this flow you will need to create a device in M2X and configure the M2X node in this flow with the appropriate API key.  Put the device ID from M2X in the edge flow in Node-RED.  In M2X you'll also need to create 3 streams for numeric data: Temperature, X-Axis, and Y-Axis.





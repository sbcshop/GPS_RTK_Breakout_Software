# GPS RTK Breakout

The SB-Components GPS RTK Breakout is the next iteration of u-blox's GPS offerings! This version takes advantage of dead reckoning for navigation. The u-Blox ZED-F9R is a powerful GPS-RTK (Real Time Kinematic) unit that uses a fusion of IMU, wheel ticks, a vehicle dynamics model, correction data, and GNSS measurements to provide a highly accurate and continuous position for navigation under challenging conditions. We will quickly get you set up using the Qwiic ecosystem through Arduino and Python so that you can start reading the output!

## What is Dead Reckoning?

Dead Reckoning is the process of determining the current position by combining previously determined positional data with speed and heading. This process can also be applied to determine future positions as well! The ZED-F9R uses Dead Reckoning which calculates speed and heading (amongst many other points of data) through the use of an ***internal inertial measurement unit (IMU)***. The addition of a wheel tick, RTCM-formatted corrections, and ***IMU allows the ZED-F9R to produce high precision*** and more accurate readings in between GNSS data refreshes!
In addition, the module can also give accurate and useful GNSS data in areas where satellite connections are difficult to maintain: areas like the dense urban environments of major cities, long tunnels, parking garages, and any large UFOs that may descend from the sky, etc.

## Hardware Overview

Specifications Image(.jpg)


## Battery
Just like the breakout board, the small metal disk just to the right of the ZED-F9R module is a small lithium battery. This battery does not provide power to the IC as the 3.3V system does, but to relevant systems inside the IC that allow for a quick reconnection to satellites. The time to first fix will be about ~26 seconds, but after it has a lock, that battery will allow for a two-second time to first fix. This is known as a hot start and lasts for four hours after the board is powered down. The battery provides over a year's worth of power to the backup system and charges slowly when the board is powered. To charge it to full, leave your module plugged in for 48 hours.


## LED’s
Just like the breakout board, there are four LEDs on the bottom left of the board. Starting from the left:
PWR: The power LED labeled as PWR will illuminate when 3.3V is activated.
PPS: The pulse per second LED labeled as PPS will illuminate each second once a position lock has been achieved. This generates a pulse that is synchronized with a GPS or UTC time grid. By default, you'll see one pulse a second.
RTK: The RTK LED will be illuminated constantly upon power-up. Once RTCM data has been successfully received it will begin to blink. This is a good way to see if the ZED-F9R is getting RTCM from various sources. Once an RTK fix is obtained, the LED will turn off.
GEO: The GEO LED can be configured to turn on/off for geofencing applications.




## USB
To connect the ZED-F9R to u-center software, you can attach a USB Type-C cable to the connector. Keep in mind that the power pin is not connected to the USB-C connector. You will need to draw power from the qwiic connector or the Pi's 2x20 header pins.




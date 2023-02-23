# GPS RTK Breakout 

In less than 30 seconds, GPS RTK Breakout enables you to determine your position, direction, and travel route to any destination on Earth. So, the better the precision, the more! We had to include it on this board since GPS Real Time Kinematics (RTK) has perfected fine-tuning its GPS modules' accuracy to only millimetres!

The GPS-RTK HAT from SB Components enhanced high-precision GPS. The ZED-F9P module from u-Blox, which offers 10mm of 3-dimensional accuracy, is the newest one that it has. The X, Y, and Z coordinates that may be generated using these boards are roughly the width of your fingernail. That is what you just read. High precision GPS requires both a stream of correction data from an RTCM source and a powerful antenna.

<img src = "https://github.com/sbcshop/GPS_RTK_Breakout_Software/blob/main/Images/img.png"/>

## Hardware Overview

Specifications Image(.jpg)


## Battery
Just like the breakout board, the small metal disk just to the right of the ZED-F9R module is a small lithium battery. This battery does not provide power to the IC as the 3.3V system does, but to relevant systems inside the IC that allow for a quick reconnection to satellites. The time to first fix will be about ~26 seconds, but after it has a lock, that battery will allow for a two-second time to first fix. This is known as a hot start and lasts for four hours after the board is powered down. The battery provides over a year's worth of power to the backup system and charges slowly when the board is powered. To charge it to full, leave your module plugged in for 48 hours.


## LED’s
Just like the breakout board, there are four LEDs on the bottom left of the board. Starting from the left:

* ***PWR:*** The power LED labeled as PWR will illuminate when 3.3V is activated.
* ***PPS:*** The pulse per second LED labeled as PPS will illuminate each second once a position lock has been achieved. This generates a pulse that is synchronized with a GPS or UTC time grid. By default, you'll see one pulse a second.

* ***RTK:*** The RTK LED will be illuminated constantly upon power-up. Once RTCM data has been successfully received it will begin to blink. This is a good way to see if the ZED-F9R is getting RTCM from various sources. Once an RTK fix is obtained, the LED will turn off.

* ***GF:*** The GEO LED can be configured to turn on/off for geofencing applications.

## USB
To connect the ZED-F9R to u-center software, you can attach a USB Type-C cable to the connector.


## Steps to Setup With Raspberry pi 

**Step.1 -** To start working with our GPS RTK Breakout with Rasberry pi/Rock pi, you to setup your pi board to boot by uploading lates OS of it.

**Step.2 -** After that, attach the GPS RTK Breakout on your Pi board and power it by providing suitable power supply. 

**Step.3 -** Once your Pi is booted, open command line and type the below command to clone this repository:
```
git clone https://github.com/sbcshop/GPS_RTK_Breakout_Software.git
```

**Step.4 -** After downloading this repository in your Pi board, you can run any of examples provided in this repository. Make sure before running any example code, move it out of ***Examples folder*** and then open it to run.


## Using GPS RTK HAT Via USB:
<img src = "https://github.com/sbcshop/GPS_RTK_Breakout_Software/blob/main/Images/img1.png"/>
 
For using this Breakout with USB cable you have to install the USB driver and a Software Application of ublox(U Center). For this you can visit the links below,

[**Download USB Driver**](https://deviceinbox.com/drivers/1870-u-blox-gnss-standard-usb-driver.html)

[**Download Software Application**](https://www.u-blox.com/en/product/u-center) and we have also provided it in this repository. After making these setup follow the steps below:

#### To learn how to use U Center application, click here.
[u-center User guide ](https://github.com/sbcshop/GPS_RTK_HAT_Hardware/blob/main/u-center_Userguide.pdf)

**Step.1 -** After intalling the above mentioned software, plugin your GPS RTK HAT to your system via USB Type-C cable and check for the available COM port. As shon in below image

<img src ="https://github.com/sbcshop/GPS_RTK_HAT_Software/blob/main/images/Scr2.png" />
<img src ="https://github.com/sbcshop/GPS_RTK_HAT_Software/blob/main/images/Scr1.png" />

**Step.2 -** Ublox begins to receive data from numerous satellites from different country as soon as you connect to the correct port, as seen in the figure below.
<img src ="https://github.com/sbcshop/GPS_RTK_HAT_Software/blob/main/images/img.JPG" />
<img src ="https://github.com/sbcshop/GPS_RTK_HAT_Software/blob/main/images/img3.JPG" />

## Documentation

* [GPS RTK Breakout Hardware]()
* [Getting Started with Raspberry Pi](https://www.raspberrypi.com/documentation/computers/getting-started.html)
* [Raspberry Pi Pico Official website](https://www.raspberrypi.com/documentation/microcontrollers/)
* [Raspberry Pi Datasheet](https://www.raspberrypi.com/documentation/computers/compute-module.html)
* [Hardware Design](https://www.raspberrypi.com/documentation/computers/compute-module.html)
* [Raspberry Pi](https://www.raspberrypi.com/documentation/microcontrollers/raspberry-pi-pico.html)


## Related Products

* [GPS HAT](https://shop.sb-components.co.uk/products/gps-hat-for-raspberry-pi?_pos=1&_sid=c0a565487&_ss=r)

 ![GPS HAT](https://cdn.shopify.com/s/files/1/1217/2104/products/GPSHATforRaspberryPi_4.png?v=1648553361&width=400)
 
 * [GPS RTK HAT]()

 ![GPS RTK HAT]()
 
 

## Product License

This is ***open source*** product. Kindly check LICENSE.md file for more information.

Please contact support@sb-components.co.uk for technical support.
<p align="center">
  <img width="360" height="100" src="https://cdn.shopify.com/s/files/1/1217/2104/files/Logo_sb_component_3.png?v=1666086771&width=350">
</p>

Aethera
=======

Aethera is a framework for creating DIY environmental sensor networks for awareness and art. 

##Hardware Overview
The sensor is created with Seeeduino Cloud and several sensors.

- Seeeduino Cloud

		Seeeduino Cloud is a microcontroller board based on Dragino WiFi IoT module HE and
		ATmega32u4. HE is a high performance, low cost 150M, 2.4G WiFi module which means
		“core” in Chinese and with an Open Source OpenWrt system inside. Seeeduino Cloud is 
		also an Arduino compatible board, 100% compatible to grove, shield and IDEs(>=1.5.3).
		Except for the normal interface of Arduino, Seeeduino Cloud has built-in Ethernet
		and WiFi support, a USB-A port which makes it very suitable for those prototype
		design that need network connection and mass storage. It is also a good idea to
		make Seeeduino Cloud to be an IoT gateway. 	
- Grove - Air Quality Sensor
- Grove - Dust Sensor
- Grove - Sound Sensor
- Grove - UV Sensor
- Grove - Digital Light Sensor
- Grove - Temperature and Humidity Sensor Pro




##Deployment

###1. Software

####1.1. Arduino Side

Step 1: Download the project: https://github.com/KillingJacky/Aethera/archive/master.zip and then unzip it.

Step 2: Copy Aetheraduino/libraries/* to your Adrduino IDE's library directory.

Step 3: Open Aetheraduino/AetheraSerial/AetheraSerial.ino with Arduino IDE.

Step 4: Connect your Seeeduino Cloud board to PC with the micro usb cable.

Step 5: Select board type "Arduino Leonardo" and the right tty/COM port in Arduino IDE.

Step 6: Upload the sketch.

####1.2. OpenWrt Side

Step 1: Same as Arduino Side's step 1.

Step 2: Config the Seeeduino Cloud to connect to your home's WiFi AP, refer to [this wiki](http://www.seeedstudio.com/wiki/Seeeduino_Cloud#Configure_Network).

Step 3: Config xively channels:

	3.1 ssh to seeeduino cloud: ssh root@seeed.local, password is [seeeduino]
	3.2 # cd /tmp
	3.3 # wget --no-check-certificate https://github.com/KillingJacky/Aethera/raw/master/AetheraCloud/iot
	3.4 # wget --no-check-certificate https://github.com/KillingJacky/Aethera/raw/master/AetheraCloud/uart_passthrough.lua
	3.5 # cp iot /etc/config/iot
	3.6 # cp uart_passthrough.lua /usr/lib/lua/dragino/uart_passthrough.lua
	
	


###2. Assembly

TODO


![image](https://raw.githubusercontent.com/KillingJacky/Aethera/master/images/assembly1.png)

![image](https://raw.githubusercontent.com/KillingJacky/Aethera/master/images/assembly2.png)

![image](https://raw.githubusercontent.com/KillingJacky/Aethera/master/images/assembly3.png)

![image](https://raw.githubusercontent.com/KillingJacky/Aethera/master/images/deployment_at_office.png)


###3. Result
Sensor reading at https://xively.com/feeds/224139911

![image](https://raw.githubusercontent.com/KillingJacky/Aethera/master/images/sensor_readings.png)


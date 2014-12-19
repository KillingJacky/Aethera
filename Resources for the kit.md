# Hardware Introduction and Resources

## Seeeduino Cloud 

![image](http://www.seeedstudio.com/depot/bmz_cache/2/249e68159b1ce7c0dc5e0c0dd3e93121.image.530x397.jpg =400x)

[Seeeduino Cloud](http://www.seeedstudio.com/depot/Seeduino-Cloud-Arduino-Yun-compatible-openWRT-controller-p-2123.html) is a microcontroller board based on Dragino WiFi IoT module HE and ATmega32u4. HE is a high performance, low cost 150M, 2.4G WiFi module which means “core” in Chinese and with an Open Source OpenWrt system inside. Seeeduino Cloud is also an Arduino compatible board, 100% compatible to grove, shield and IDEs(>=1.5.3). Except for the normal interface of Arduino, Seeeduino Cloud has built-in Ethernet and WiFi support, a USB-A port which makes it very suitable for those prototype design that need network connection and mass storage. It is also a good idea to make Seeeduino Cloud to be an IoT gateway. 

[HE module](http://www.dragino.com/products/linux-module/item/87-he.html):

![image](http://www.dragino.com/media/k2/galleries/87/HE_10.png =250x)

###Features of Seeeduino Cloud:

*   Compatible with Arduino Yun
*   Based on Dragino WiFi IoT module HE
*   Open Source OpenWrt system inside
*   Support 2.4Ghz WiFi, 802.11 b/g/n
*   Support Ethernet
*   Support USB 2.0
*   Size:  75.10mm x 53.39mm x 11.50mm / 2.95" x 2.10 x 0.45"
*   Working temperature:  -20~60°C
*   Surface colors:  Red

###Features of HE module:
* CPU: ATHEROS AR9331 chipset, which integrates MIPS 24Kc processor, CPU 400MHz, Switch (MAC,PHY) and integrates with MAC, RF, PA and LNA for WiFi. 
* RAM : 64MB;
* Flash : 16MB
* Interfaces: 2 x RJ45, 1 x USB Host, 1 x UART, 14 multiplex GPIOs
* OS: Open Source OpenWrt 
* Power: 3.3v power input
* WiFi: Support 150M 2.4Ghz WiFi, 802.11 b/g/n
* Frequency range: 2.4~2.4835GHz
* Modulation: BPSK, QPSK, CCK and OFDM (BPSK/QPSK/16-QAM/ 64-QAM)
* Sensitivity @PER : 135M : -65dBm@10%PER; 65M : -65dBm@10%PER; 54M : -68dBm@10%PER; 11M : -84dBm@8% PER; 6M : -88dBm@10% PER; 1M : -90dBm@8% PER
* Typical Distance: Indoor: 60m (max); Outdoor 150m (max) (with 2 dBi antenna) 
* RF Power: 11n: 13dBm; 11g: 13-15dBm, 11b: 16-18dBm,
* Connector: I-PEX connector. Provide Optional ANT pin out for SMT


###Resources:
* Wiki: http://www.seeedstudio.com/wiki/Seeeduino_Cloud
* Schematic: http://www.seeedstudio.com/wiki/File:Seeeduino_Cloud_PDF.pdf
* Latest Firmware: http://www.seeedstudio.com/wiki/File:Seeed-build--v1.3.4--20140815-1100.zip
* Link of the "HE" Core module: http://www.dragino.com/products/linux-module/item/87-he.html

	Note: You can also refer to the documentations of Arduino Yun as they're commonly forked from the Linino branch of OpenWrt OS.

* Datasheet for HE: http://www.dragino.com/downloads/index.php?dir=datasheet/&file=HE%20WiFi%20IoT%20Module%20datasheet.pdf
* Link of Arduino Yun: http://arduino.cc/en/Main/ArduinoBoardYun?from=Main.ArduinoYUN

###Tips:
* How to reset Arduino side (32U4) without resetting the whole board?

		Press the button with overlay "RESET" aside.
		
* How to reset the MIPS side?

		Press the button with overlay "ORST" aside.
		
* How to restore the WiFi setting to factory default? 
		
		Press the button with overlay "START" over 5 seconds (less than 30 seconds) and then release.
		
* How can I make the seeeduino cloud connect to another WiFi router?
		
		You need to press the "START" button over 5 seconds to clear the previous WiFi 
		settings, then power cycle the Seeeduino Cloud. Use your laptop to search the WiFi
		 SSID named "Seeeduino-Cloud-xxxx", then join that SSID. Open the web browser, goto
		 "192.168.240.1", then you will see the Seeeduino Cloud WEB GUI web page. Default
		 password is "seeeduino".


##Base Shield V2

![image](http://www.seeedstudio.com/depot/bmz_cache/b/b8312e50059ec7b2f092ac35939228d3.image.530x397.jpg =400x)

As an expansion board, [Base Shield v2](http://www.seeedstudio.com/depot/Base-Shield-V2-p-1378.html) has many Grove connectors, making it convenient for you to use Grove products together. And It is compatible with a series of Arduino products.

Power Compatible: Every Grove connector has four wires, one of which is Vcc. However, not every micro-controller main board needs a supply voltage of 5V, some need 3.3V. That's why we add a power switch to Base Shield v2. In this way, you can adjust the voltage of Vcc via this switch, making sure the voltage of Vcc is the same as supply power of the main board.


###Resources:
* Wiki page: http://www.seeedstudio.com/wiki/Base_shield_v2
* Schematic: http://www.seeedstudio.com/wiki/File:Base_Shield_v2.zip

##Grove - Dust Sensor

![image](http://www.seeedstudio.com/depot/bmz_cache/1/1976cb8eaa49ee0fa94d5642953c4c91.image.530x397.jpg =400x)

[Dust Sensor](http://www.seeedstudio.com/depot/Grove-Dust-Sensor-p-1050.html) is to create Digital (Lo Pulse) output to Particulate Matters (PM). Lo Pulse Occupancy time (LPO time) is in proportion to PM concentration. The output is for PM whose size is around 1 micro meter or larger. We can use the sensor to detect the dust in clean room. 

###Features:
* Grove compatible interface(extra wire with connecter) 
* Supply voltage range: 5V 
* Minimum detect particle: 1um 
* PWM output 
* Dimensions: 59(W)x45(H)x22(D) [mm]

###Resources:
* Wiki page: http://www.seeedstudio.com/wiki/Grove_-_Dust_sensor
* Datasheet: http://www.seeedstudio.com/wiki/images/4/4c/Grove_-_Dust_sensor.pdf
* Example 1: https://github.com/Seeed-Studio/TravellingMine
* Example 2: https://github.com/Seeed-Studio/Air_Quality_Test_Box
* Example 3: https://github.com/Seeed-Studio/Grove_Dust_Sensor


##Grove - UV Sensor

![image](http://www.seeedstudio.com/depot/bmz_cache/a/aec20fab6989d66cbbd915df21a74c23.image.530x397.jpg =200x)

The [Grove – UV Sensor](http://www.seeedstudio.com/depot/Grove-UV-Sensor-p-1540.html) is used for detecting the intensity of incident ultraviolet(UV) radiation. This form of electromagnetic radiation has shorter wavelengths than visible radiation. It is based on the sensor GUVA-S12D.It has a wide spectral range of 200nm-400nm. The module will output electrical signal which is varied with the change of the UV intensity. UV sensors are used for determining exposure to ultraviolet radiation in laboratory or environmental settings.
 
###Features:
* High stability
* Good Sensitivity
* Low power consumption
* Schottky type photodiode sensor
* Wide response range
* Grove Interface

###Resources:
* Wiki page: http://www.seeedstudio.com/wiki/Grove_-_UV_Sensor
* Datasheet: http://www.seeedstudio.com/wiki/File:GUVA-S12SD.pdf
* Schematic: http://www.seeedstudio.com/wiki/File:Grove_-_UV_Sensor_v1.0_Schematic.pdf
* Eagle File: http://www.seeedstudio.com/wiki/File:Grove_-_UV_Sensor_Eagle_File.zip

##Grove - Air quality sensor

![image](http://www.seeedstudio.com/depot/bmz_cache/0/080f9fde69ce40f9014165343ca3e52a.image.530x397.jpg =200x)

###Resources:
* Wiki page: http://www.seeedstudio.com/wiki/Grove_-_Air_Quality_Sensor
* Sensor Datasheet: http://www.seeedstudio.com/wiki/File:TP-401A_Indoor_Air_quality_gas_sensor.pdf
* Schematic: http://www.seeedstudio.com/wiki/File:Air_quality_sensor_schematic.pdf
* Example 1: https://github.com/Seeed-Studio/TravellingMine
* Example 2: https://github.com/Seeed-Studio/Grove_Air_quality_Sensor
* Example 3: https://github.com/Seeed-Studio/Air_Quality_Test_Box

##Grove - Sound Sensor

![image](http://www.seeedstudio.com/depot/bmz_cache/5/55dd867cf1dab660307a36cfed9ec839.image.530x397.jpg =200x)

The [Sound sensor](http://www.seeedstudio.com/depot/Grove-Sound-Sensor-p-752.html) module is a simple microphone. Based on the power amplifier LM386 and the electret microphone, it can be used to detect the sound strength of the environment. The value of output can be adjusted by the potentiometer.

###Features:
* Grove compatible interface
* Wide supply voltage range: 4V-12V
* Low quiescent current drain: 4mA
* 2.0cm x 2.0cm twig module
* Minimum external parts
* Gain adjustable

###Resources:
* Wiki: http://www.seeedstudio.com/wiki/index.php?title=Twig_-_Sound_Sensor
* Schematic: http://www.seeedstudio.com/wiki/images/e/e6/Grove_-_Sound_Sensor_v1.pdf
* Eagle file: http://www.seeedstudio.com/wiki/File:Grove_-_Sound_Sensor_v1.3_eagle.zip%E2%80%8E
* Datasheet: http://garden.seeedstudio.com/images/a/ae/LM386.pdf

##Grove - Digital Light Sensor

![image](http://www.seeedstudio.com/depot/bmz_cache/7/7dea62fdd646e6ce323bc4dea6bd54b8.image.530x397.jpg =200x)

[This module](http://www.seeedstudio.com/depot/Grove-Digital-Light-Sensor-p-1281.html) is based on the I2C light-to-digital converter TSL2561 to transform light intensity to a digital signal. Different from traditional analog light sensor, as Grove - Light Sensor, this digital module features a selectable light spectrum range due to its dual light sensitive diodes: infrared and full spectrum. 
 
You can switch between three detection modes to take your readings. They are infrared mode, full spectrum and human visible mode. When running under the human visible mode, this sensor will give you readings just close to your eye feelings.
 
###Features:
* Selectable detection modes
* high resolution 16-Bit digital output at 400 kHz I2C Fast-Mode
* Wide dynamic range: 0.1 - 40,000 LUX
* Wide operating temperature range: -40°C to 85°C
* Programmable interrupt function with User-Defined Upper and lower threshold settings

###Resources:
* Wiki page: http://www.seeedstudio.com/wiki/Grove_-_Digital_Light_Sensor
* Library: https://github.com/Seeed-Studio/Grove_Digital_Light_Sensor
* Schematic pdf: http://www.seeedstudio.com/wiki/File:Digital_light_sensor.pdf
* Eagle file: http://www.seeedstudio.com/wiki/File:Digital_light_sensor_eagle_file.zip
* TSL2561 datasheet: http://www.seeedstudio.com/wiki/File:TSL2561T.pdf

##Grove - Temperature & Humidity Sensor Pro

![image](http://www.seeedstudio.com/depot/bmz_cache/7/70777aac5fb1498dcb66c94e0a9ea950.image.530x397.jpg =200x)

This product is a high accuracy temperature and humidity sensor used in home conditions. It consists of a capacitive sensor element used for measuring relative humidity and a negative temperature coefficient (NTC) thermistor used for measuring temperature. Every sensor was calibrated in an accurate humidity room. Small dimension, ultra low power consumption, more than 20m's signal transmission distance make it a good selection for various application environment. Different from Twig - Temp&Humi Sensor v0.9b, the accuracy of this module can gets up to 0.3 degree in temperature and 2% in relative humidity.

###Resources:
* Wiki: http://www.seeedstudio.com/wiki/Grove_-_Temperature_and_Humidity_Sensor_Pro
* Library: https://github.com/Seeed-Studio/Grove_Temper_Humidity_TH02
* Eagle file: http://www.seeedstudio.com/wiki/File:Temp_Humi_Pro_eagle_files.zip
* Datasheet for TH02: http://www.hoperf.cn/upload/sensor/TH02_V1.1.pdf


The end
















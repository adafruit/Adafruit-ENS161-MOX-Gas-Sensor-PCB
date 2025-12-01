## Adafruit ENS161 MOX Gas Sensor - STEMMA QT / Qwiic PCB

<a href="http://www.adafruit.com/products/6431"><img src="assets/6431.jpg?raw=true" width="500px"><br/>
Click here to purchase one from the Adafruit shop</a>

PCB files for the Adafruit ENS161 MOX Gas Sensor - STEMMA QT / Qwiic. 

Format is EagleCAD schematic and board layout
* https://www.adafruit.com/product/6431

### Description

*sniff* *sniff* ... do you smell that? No need to stick your nose into a carton of milk anymore, you can build a digital nose with the ENS161 Gas Sensor, a fully integrated MOX gas sensor. This is a very fine air quality sensor from the sensor experts at [ScioSense](https://www.sciosense.com/products/environmental-sensors/digital-multi-gas-sensor/), with I2C interfacing so you don't have to manage the heater and analog reading of a MOX sensor. It combines multiple metal-oxide sensing and heating elements on one chip to provide more detailed air quality signals.

The ENS161 is an update to the popular ENS160 (the replacement for the [popular, but now-discontinued CCS811.](https://www.sciosense.com/products/environmental-sensors/ccs811/))  The ENS161 has the same four-part gas sensor and I2C/SPI interface but with improved built-in eCO2 and TVOC algorithms plus a new Air Quality Index (AQI) output.

The ENS161 has a 'standard' hot-plate MOX sensor divided into 4 sections, as well as a small microcontroller that controls power to the plate, reads the analog voltage, and provides an I2C interface to read from. [ScioSense provides an Arduino library with examples of reading the four raw resistance values and also the TVOC and eCO2](https://github.com/sciosense/ens16x-arduino), and [a Python/CircuitPython library](https://github.com/adafruit/Adafruit_CircuitPython_ENS160) that can be used with Linux computers like the Raspberry Pi or our CircuitPython boards.

<b>Please note, this sensor, like all VOC/gas sensors, has variability, and to get precise measurements you will want to calibrate it against known sources!</b> That said, for general environmental sensors, it will give you a good idea of trends and comparison.

Another nice element of this sensor is [the ability to set temperature and humidity compensation for better accuracy](https://github.com/sciosense/ens16x-arduino/tree/main/examples/02_Temperature_and_RH_compensation). An external humidity sensor is required and then the RH% is written over I2C to the sensor, so it can better calibrate the MOX sensor reading and reduce humidity/temperature-based variations.

Nice sensor right? So we made it easy for you to get right into your next project. The surface-mount sensor is soldered onto a custom-made PCB in the [STEMMA QT form factor](https://www.adafruit.com/?q=stemma%20qt%20sensor), making them easy to interface with. The [STEMMA QT connectors](https://learn.adafruit.com/introducing-adafruit-stemma-qt/what-is-stemma-qt) on either side are compatible with the [SparkFun Qwiic](https://www.sparkfun.com/qwiic) I2C connectors. This allows you to make solderless connections between your development board and the ENS161 or to chain it with a wide range of other sensors and accessories using a [compatible cable](https://www.adafruit.com/?q=stemma%20qt%20cable). [QT Cable is not included, but we have a variety in the shop](https://www.adafruit.com/?q=stemma+qt+cable&sort=BestMatch).

We’ve of course broken out all the pins to standard headers and added a 3.3V voltage regulator and level shifting to allow you to use it with either 3.3V or 5V systems, such as the Arduino Uno, or Feather M4.

### License

Adafruit invests time and resources providing this open source design, please support Adafruit and open-source hardware by purchasing products from [Adafruit](https://www.adafruit.com)!

Designed by Limor Fried/Ladyada for Adafruit Industries.

Creative Commons Attribution/Share-Alike, all text above must be included in any redistribution. 
See license.txt for additional details.

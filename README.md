# MLX90316-Test
## Bare bones code for testing the MLX90316 angle sensor
This will be a replacement for a broken precision potentiometer in my MetOne Instruments anemometer-windvane.

I got the idea to use this sensor from: https://www.instructables.com/id/Accurate-Wireless-Weather-Vane/

The code was originally from: <http://interface.khm.de/index.php/lab/interfaces-advanced/rotary-positionsensor-mlx90316/> 

But the above link is FUBAR; it's only here to give credit to the author(s).  And I made a couple 
changes: 
- Changed use of the UNIX "cron-like" Metro library and instead to use Chrono.
- Added error messages if signal too weak, too strong.
- and prints "angle = "

## Original from the khm.de website (when the link worked):

MLX90316 Rotary Position Sensor<br>
KHM 2010 /  Martin Nawrath<br>
Kunsthochschule fuer Medien Koeln<br>
Academy of Media Arts Cologne<br>

The MLX90316BDG is a rotary position sensor which measures the direction of a 
magnetic field with an SPI interface. It is a substitution for potentiometers or 
shaft encoders. The resolution is about 1/10 of a degree with an update rate 
of 2 mS. A diametrically opposed magnet placed on a shaft or a joint where the sensor is placed 
next to it is the typical configuration. To obtain the best accuracy the 
rotation axis of the magnet should be placed over the center of the chip. 
The MLX90316 library helps to read the chip data.

## Metro Library
The below is from the author of Metro, which is a "cron-like" library for theArduino/ESP8266: 

https://github.com/thomasfredericks/Metro-Arduino-Wiring

Metro works well, but this is the new version : https://github.com/SofaPirate/Chrono

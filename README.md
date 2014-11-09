Adafruit NeoPixel library with RFduino Support
=========================

## Notes about RFduino

This is Adafruit's NeoPixel library with modifications for [RFduino](http://rfduino.com) made by Thomas Olson. See [the RFduino forum post](http://forum.rfduino.com/index.php?topic=30.msg1495#msg1495) for more details.

This code is based off an older version of the NeoPixel library https://github.com/adafruit/Adafruit_NeoPixel/commit/510e4558937b6f1ec4e5f3e4d8070361c7bf8657

This code works with Arduino IDE 1.5.6-r2 and RFduino 2.1 or earlier. The forum post said it is broken with 1.5.7.

Download Arduino IDE 1.5.6-r2 beta from http://arduino.cc/en/Main/OldSoftwareReleases

Install RFduino extensions

    $ cd "/Applications/Arduino 1.5.6 r2.app/Contents/Resources/Java/hardware/arduino"
    $ git clone https://github.com/RFduino/RFduino
    $ cd RFduino
    $ git checkout v2.1

Install NeoPixel Library

    $ cd ~/Documents/Arduino/libraries
    $ git clone https://github.com/don/Adafruit_NeoPixel Adafruit_NeoPixel_tolsonMod

Notes: 
    You'll need the "tolson" branch of https://github.com/don/Adafruit_NeoPixel. You should get this branch by default.
    You'll need to delete or move Adafruit's version of Adafruit_NeoPixel from your library directory.

I get an error when uploading but the sketch still works.

	Couldn't determine program size: java.io.IOException: Cannot run program "/Applications/Arduino 1.5.6 r2.app/Contents/Resources/Java/hardware/arduino/RFduino/size": error=2, No such file or directory0

## Original README

Arduino library for controlling single-wire-based LED pixels and strip such as the [Adafruit 60 LED/meter Digital LED strip][strip], the [Adafruit FLORA RGB Smart Pixel][flora], the [Adafruit Breadboard-friendly RGB Smart Pixel][pixel], the [Adafruit NeoPixel Stick][stick], and the [Adafruit NeoPixel Shield][shield].

After downloading, rename folder to 'Adafruit_NeoPixel' and install in Arduino Libraries folder. Restart Arduino IDE, then open File->Sketchbook->Library->Adafruit_NeoPixel->strandtest sketch.

[flora]:  http://adafruit.com/products/1060
[strip]:  http://adafruit.com/products/1138
[pixel]:  http://adafruit.com/products/1312
[stick]:  http://adafruit.com/products/1426
[shield]: http://adafruit.com/products/1430

# LED7Segment/DirectDrive

Drives a 7-segment display, performing a countdown from 9 to 0.

## Notes

The 7-segment display unit I have is stamped "SMA42056". It appears to be fairly common, however I've yet to find a datasheet for it.
From inspection hwoever, it's clearly a common cathode unit, and similar to the
the [SC56-11](./assets/SC56-11_datasheet.pdf?raw=true)

There are two common cathode pins, but since these are internally connected there is no need to connect both to ground.
Lighting a segment simply means providing a driving voltage to the corresponding anode pin.

This circuit puts the resistors in series of the anode pins. This ensures a consistent brightness no matter how many segments are on. Note that it is possible to put the current-limiting resistor on the common cathode;
this is a bit of an approximation and will lead to varying LED brightness but may be "good enough" depending on your application.

for a simple test.

### Construction

![The Breadboard](./assets/DirectDrive_bb.jpg?raw=true)

![The Schematic](./assets/DirectDrive_schematic.jpg?raw=true)

![The Build](./assets/DirectDrive_build.jpg?raw=true)

## Credits and references
* [SC56-11 Datasheet](./assets/SC56-11_datasheet.pdf?raw=true)
* [Arduino and 7 Segment LED](http://www.hacktronics.com/Tutorials/arduino-and-7-segment-led.html) - original idea and source code
* [Drive a 7-Segment LED with an Arduino](http://makezine.com/projects/drive-a-7-segment-led-with-an-arduino/)
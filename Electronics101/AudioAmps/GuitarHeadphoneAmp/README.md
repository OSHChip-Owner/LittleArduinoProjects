# GuitarHeadphoneAmp

An LM386 fixed-gain guitar headphone amp.

## Notes

Yet another LM386-based audio amplifier, this time adapted as a guitar headphone amp.

The main differences in this case:
* gain is limited to 50x with pin 1 tied to 8 through R3 + C3.
* R1 at input is appropriate match for guitar input impedence

How it performs:
* the input volume control works fine, although it is pretty redundant as it is doing the same job as a guitar's onboard volume control
* the lack of independent gain control is a bit limiting. i.e. the choice is quiet and clean, or load and overdriven.
* on a bradboard, there's a bit of interference and noise in the mix. That would probably clean up quite a bit in a PCB build.

## Construction

![Breadboard](./assets/GuitarHeadphoneAmp_bb.jpg?raw=true)

![The Schematic](./assets/GuitarHeadphoneAmp_schematic.jpg?raw=true)

![The Build](./assets/GuitarHeadphoneAmp_build.jpg?raw=true)

## Credits and References
* Based on "Project 07 - Guitar Headphone Amplifier" from [Beginning Analog Electronics through Projects](http://www.amazon.com/gp/product/0750672838/ref=as_li_tl?ie=UTF8&camp=1789&creative=390957&creativeASIN=0750672838&linkCode=as2&tag=itsaprli-20&linkId=QUZ3GKIDBEXGNSG7)
* [my LittleGem/A386 build](../LittleGem)
* [Smokey Amps](http://www.smokeyamps.com/) - official site
* [Smokey Amp Analysis](http://www.electrosmash.com/smokey-amp-analysis) - excellent circuit analysis of the original Smokey amp.
* [Observations on the Smokey circuit by Dave Stork](http://www.blueguitar.org/new/schem/_ss/smokey.txt)
* [LM386 datasheet](http://www.futurlec.com/Linear/LM386N-3.shtml)


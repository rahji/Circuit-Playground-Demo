# Circuit Playground Express Mega Demo for PlatformIO

This is a version of the Adafruit Circuit Playground [Mega Demo](https://github.com/adafruit/Adafruit_CircuitPlayground/tree/master/examples/mega_demo) that works with the Circuit Playground *Express* and PlatformIO (instead of the Arduino software). 

## Play Instructions (adapted from the comments in main.cpp)

This is a showcase of interesting demos for the Circuit Playground Express. 

* The **slide switch** essentially turns the demo on (left) and off (right)
* Press the **left button** to cycle through each demo
* Press the **right button** to cycle through each mode within a demo

The demos and their modes are:

1. NeoPixel color rainbow (changing the mode changes the animation speed)
2. Volume level meter (changing the mode cycles through levels of sensitivity)
3. Capacitive touch (pressing the mode button turns on sound)
4. Accelerometer tilt demo (changing the mode cycles through the different axes - X/Y/Z)
5. Temperature & light sensor demo. Left/blue half is the temperature. Right/red half is the light sensor. (changing the mode cycles through levels of sensitivity)

## Changes from the Original

* Added some forward declarations for functions
* Changed main.io to main.cpp (but left the other .ino files alone, since it would be a lot more work to convert those to .cpp files and I'm really just trying to get this to *build* in PlatformIO)
* Skipped moving over some of the unnecessary dot files that were in the repo
* The all-important platform.ini is in place, with the required dependencies (Circuit Playground, SleepyDog, and ZeroDMA for the CPX)

## Why?

This is for a quick demo in the first week of my physical computing course in the Department of Art at Florida State University. We're using vscode and PlatformIO instead of the Arduino software.

We are not using the Circuit Playground Express this semester, but I have a bunch of CPX boards hanging around and this will allow them to see the process of building and uploading files to a microcontroller, and dazzle students with the possibilities of using sensors and light/sound while we wait for our microcontroller kits to arrive in week 2.

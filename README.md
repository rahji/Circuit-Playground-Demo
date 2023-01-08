# Circuit Playground Express Mega Demo for PlatformIO

This is a version of the Adafruit Circuit Playground [Mega Demo](https://github.com/adafruit/Adafruit_CircuitPlayground/tree/master/examples/mega_demo) that works with the Circuit Playground *Express* and PlatformIO (instead of the Arduino software). The changes were:

* Added some forward declarations for functions
* Changed main.io to main.cpp (but left the other .ino files alone, since it would be a lot more work to convert those to .cpp files and I'm really just trying to get this to *build* in PlatformIO)
* Skipped moving over some of the unnecessary dot files that were in the repo
* The all-important platform.ini is in place, with the required dependencies (Circuit Playground, SleepyDog, and ZeroDMA for the CPX)

This is for a quick demo in the first week of my physical computing course in the Department of Art at Florida State University. We are actually using a different MCU, but I have a bunch of CPX boards hanging around and this will allow them to see the process of building and uploading files to a microcontroller, and dazzle students with the possibilities of using sensors and light/sound.

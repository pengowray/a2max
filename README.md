# a2max
Integer Basic boot loader with maximum compatibility for the Apple II series and emulators

To use:
 - Make a copy of example/morse321.dsk and rename it
 - Replace the contents of the file named APPLESOFT with an Integer BASIC program of your choice (e.g. using CiderPress)

Result:
 - Your "APPLESOFT" program will run on boot on the original Apple II
 - On other machines in the series, integer basic will load onto the language card first, and then "APPLESOFT" will run

To do:
 - Use LOADER.OBJ0 program to fast-load INTBASIC if possible
 - Use relocatable Integer Basic if language card not available
 - Work out what it's actually doing rn I'm not really sure I'm new to this but it works
 - Investigate: Possibly don't need bootloader at all if using something other than DOS3.3 idk.
 - Check it works on real hardware
 - Find a compatible catalog menu program for multi-headed applications

Original motivation:
 - To make single-program disks playable on the internet archive, where emulator support for the original Apple II is flaky.
 - I couldn't work out a simpler way
 - Based on code from: https://archive.org/details/D10S2_DECODAGE_MORSE_RTTY

Further reading
 - [Versions of DOS 3.3](https://github.com/cmosher01/Apple-II-Source/blob/master/README-notes) ([archive](https://web.archive.org/web/20220507220847/https://github.com/cmosher01/Apple-II-Source/blob/master/README-notes))
 - [How to make a maximally compatible Integer BASIC (Apple II) game disk for the Internet Archive?](https://retrocomputing.stackexchange.com/questions/24455/how-to-make-a-maximally-compatible-integer-basic-apple-ii-game-disk-for-the-in)

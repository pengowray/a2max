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
 - Fallback to regular INTBASIC loader (if that's possible/needed)
 - Use relocatable Integer Basic if language card not available
 - Work out what I'm actually doing rn I'm not really sure I'm new to this but it works
 - Investigate: Possibly don't need bootloader at all if using something other than DOS3.3 idk.
 - Check it works on real hardware
 - Find an original Apple II compatible [catalog menu program](https://retrocomputing.stackexchange.com/questions/14206/where-did-the-levi-file-selector-runner-for-the-apple-ii-dos-3-3-come-from/14228#14228) with a very simple UI (just select program to run; no extraneous copy/delete/etc)

Original motivation:
 - To make single-program disks playable on the internet archive, where emulator support for the original Apple II is flaky.
 - I couldn't work out a simpler way
 - Based on code from: https://archive.org/details/D10S2_DECODAGE_MORSE_RTTY

Further reading
 - [Versions of DOS 3.3](https://github.com/cmosher01/Apple-II-Source/blob/master/README-notes) ([archive](https://web.archive.org/web/20220507220847/https://github.com/cmosher01/Apple-II-Source/blob/master/README-notes))
 - [Integer Basic brief history](https://retrocomputing.stackexchange.com/questions/13137/using-integer-basic-on-apple-ii-plus-without-a-language-card/13139#13139)
 - [How to make a maximally compatible Integer BASIC (Apple II) game disk for the Internet Archive?](https://retrocomputing.stackexchange.com/questions/24455/how-to-make-a-maximally-compatible-integer-basic-apple-ii-game-disk-for-the-in)

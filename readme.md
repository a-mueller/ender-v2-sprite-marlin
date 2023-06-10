# Ender v2 firmware for Sprite Extruder
This is mainly for myself to make it possible to rebuild this. This worked for me by connecting the short cable to the extruder for the CR Touch evnethough a lot of people in the internet seem to have problems with that. It will not unlock the higher temperatures though.

What you should have:
- 4.2.2 Board
- Ender v2
- Sprite extruder
- CR touch probe

## Just need the firmware
Depending on your mainbord processor download the RC or the RE version of the .bin file. (it says on the chip on the 4.2.2 board)
Flash it by copying to the SD card and restarting your printer
Flash the display by copying the `DWIN_SET` folder to an SD card and insert it into the slot of the display (NOT THE PRINTER, I always forget that)
Make sure you do the z-probe wizard thing as the default will be too high.


## Compile yourself
Clone the 2.1.2.1 source repo from Marlin, and follow one of the tutorials how to compile in vscode. (Don't forget to install that plugin)
Use the config files from this repo instead of the one from the `/examples` folder in the tutorial.
The .ini file just specifies the rc processor as default (which I have)
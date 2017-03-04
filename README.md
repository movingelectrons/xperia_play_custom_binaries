# xperia_play_custom_binaries
Binary files for flashing to Sony Ericson Xperia Play (these are the binaries that I personally use)

DISCLAIMER: I TAKE ABSOLUTLY NO CREDIT FOR THE CREATION OF THESE FILES, I AM MEERLY MAKING THEM EASY TO FIND, AS I SPEND COUNTLESS HOURS FIGURING OUT WHAT WORKED FINALLY ON MY PHONE.

## How to (flash the kernal then install the rom, google apps, and the wifi fix
### preresiquites
must install android development kit, and the google usb driver (there are tons of easy guides to follow already)
then replace the driver with this one (go into device manager and manually select this file for the phone (after you plug the phone in and put it into fastboot mode.  Hold down the search button (bottom right button on front of phone) while the phone is off and plug the USB cable into your PC to enter fastboot mode.
put the rom, gapps, and the wififix in the root of your sdcard and put the sdcard in the phone

### flash the kernel
put the phone into fastboot mode
go into ~/AppData/Local/Android/sdk/platform-tools (AppData is a hidden folder in the root of your home directory (IE /c/Users/whateveryourusernameis) in the command prompt, then run:

```bash
./fastboot.exe devices
```
you some get some kind of response back (A BLANK RESPONSE IS WRONG!).  It should respond with one line of nonsense.
then run:

```bash
./fastboot.exe flash boot LuPuS-PLAY-jbv8-720.img
./fastboot.exe erase system
./fastboot.exe erase userdata
./fastboot.exe reboot
```

### flash the rom
next time your phone boots up, it should have a cool fox head logo and say LUPIS.  Mash on the volume down key and/or back key to enter the bootloader and/or recovery.  you want to enter recovery and install the following 3 zip files.  the wififix might fail, select the option to fix the wifi from the bootloader if this is the case (your wifi might just work anyways).

the rom[link goes here]
gapps[link goes here]
wifi fix[link goes here]

Thats is!  Finally done.  Whew...


## Links to the binary files hosted here on github
### the kernal
[link goes here]

### the rom
[link goes here]

### gapps
[link goes here]

### wifi fix
[link goes here]

## Links to orgional authors
### the kernal
[https://forum.xda-developers.com/showthread.php?t=1861970]
### the rom
[https://forum.xda-developers.com/showthread.php?t=2286648]
### orgional help page that was very helpful (at first)
[https://github.com/LegacyXperia/Wiki/wiki/Installing-Marshmallow]


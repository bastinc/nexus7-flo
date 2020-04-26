README
=======


1) Use restock on Windows to restore Nexus 7 (flo) to factory if modified (automatic procedure)
2) Install TWRP for custom recovery

https://twrp.me/asus/asusnexus72013wifi.html

On your device, go into Settings -> About and find the Build Number and tap on it 7 times to enable developer settings. Press back and go into Developer Options and enable USB debugging. From your computer, open a command prompt and type:

    adb reboot bootloader

You should now be in fastboot mode.

Download the correct image file and copy the file into the same folder as your platform-tools. Rename the image to twrp.img and type:

    fastboot flash recovery twrp.img

    fastboot reboot

Use Power + volume down to boot into fastboot

3) Install flo-deb_clamor_repartition.zip with Recovery to extend partition for Android > 8

    * use recovery -> install zip -> flo-deb_clamor_repartition.zip
    * go to main menu -> advanced -> terminal and write «modify»
    
5) Format everything
 
    In TWRP: Wipe > Format Data
    Type Yes
    Once this completes go to: Wipe > Advanced Wipe
    Tick all the boxes and wipe. There should be no further mount errors.
    
4) Install the custom TWRP specially modified for this kind of partition

5) Boot into recovery

6) Recovery is bit slow but it's ok. Now install a custom image.

All credits to xda forums

https://forum.xda-developers.com/nexus-7-2013/orig-development/repartition-nexus-7-2013-repartition-t3844386





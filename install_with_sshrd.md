# Installation through an SSH Ramdisk (Linux and macOS only)

**_**If you do not have a Mac or a Linux PC, make an Ubuntu live USB and boot from it on your computer. **_**

**Supported devices:** A8(X) - A11, iOS 14.0 - 15.5b4

Video tutorial: https://youtu.be/B0MueVvJSK4

1. Run `git clone https://github.com/verygenericname/SSHRD_Script --recursive && cd SSHRD_Script`

2. Run `./sshrd.sh <iOS version for ramdisk> TrollStore <uninstallable system app>`
    - Make sure to **not** include the `<>`
    - The uninstallable system app should be an app you don't need to use (e.g. Tips)
    - i.e. `./sshrd.sh 15.0 TrollStore Tips`

3. Put your device into DFU mode. Instructions for this can be found [here](https://www.theiphonewiki.com/wiki/DFU_Mode#iPhone.2C_iPad.2C_iPod_touch).
    - If you are on an A11 device, entire recovery mode first by pressing and quickly releasing the volume up and volume down button, one at a time. Then, press and hold       the side button until you see the recovery mode screen. Finally, put your device into DFU mode as said above.  
   
4. Run `./sshrd.sh boot` the device should start verbosing and show a TrollFace in ascii, then reboot eventually

5. Open up the app you replaced (Tips in this example), it should be TrollStore Helper now.

6. Make sure you're connected to the internet, and press "Install TrollStore."

7. Done, your device will respring and TrollStore should appear on your home screen.

# Firmware releases for DK1.x
 
**⚠️ Caution: You won't need to update the firmware unless the device is working incorrectly. 
If you are unsure, please contact SenseGlove.**

## Updating firmware

### Flash tool download:
Get the Samba In System Programmer at http://ww1.microchip.com/downloads/en/DeviceDoc/SAM-BA%20v2.18%20for%20Windows.exe

### Firmware download:
Get the latest firmware version at: http://www.github.com/Adjuvo/firmware-releases
Make sure you download the correct version for your glove. There are different hardware versions of the glove.
firmware-update-DK11-* updates are for SenseGlove DK1.1 hardware, firmware-update-DK12-* are DK1.2 for and upwards. 
⚠️ Updating the wrong firmware can result in incorrect functioning of the glove. In case of doubt, please contact Senseglove.

### Preparing
1. Keep the boot pin pressed while you plug in the SenseGlove with a micro USB cable. You can find the boot pin
as shown in this picture: 

![Screenshot](https://github.com/Adjuvo/firmware-releases/raw/master/bootpin.png "bootpin")

The SenseGlove is now in boot mode. 

2. Open the Device Manager in Windows, by right clicking the Windows Icon in the taskbar and clicking on Device Manager. Under ports (COM & LPT) a port named *AT91 USB to Serial Converter* or *Bossa Program Port* should be available. Take note of the COMPORT number after the the program name. The figure belows shows an example:

![Screenshot](https://github.com/Adjuvo/firmware-releases/raw/master/comport.png "select")

### Updating
1. Start the Samba flash tool and use the following settings in corresponding fields:
- Select the connection: Noted COMPORT number the previous step
- Select your board: samd21_xplained_pro
- JLink TimeOutMultiplier: 0

The figure below shows an example:

![Screenshot](https://github.com/Adjuvo/firmware-releases/raw/master/select.png "select")

Click on connect. This should bring up the next window.

2. Send File Name: Select the correct binary (note: left or right SenseGloves need different versions)

3. Address: Set the Address to 0x6000

4. Press 'Send file'

Wait for the process to complete, it could be rather slow and could last a few minutes.
The following screenshot gives an overview of the steps 3, 4, 5

![Screenshot2](https://github.com/Adjuvo/firmware-releases/raw/master/write.png "write")

Unplug the SenseGlove from the micro USB cable and reconnect it using the same micro USB cable.
Your SenseGlove is now ready for use.

# Firmware releases for DK1.x

## Updating firmware

### Flash tool download:
Get the Samba In system programmer at http://ww1.microchip.com/downloads/en/DeviceDoc/SAM-BA%20v2.18%20for%20Windows.exe

### Firmware download:
Get the latest firmware version at: http://www.github.com/Adjuvo/firmware-releases

### Preparing
Keep the boot pin pressed while you power up the SenseGlove. You can find the boot
as shown in this picture: 

The SenseGlove is now in boot mode. Start the Samba flash tool

### Updating
1. Select the correct COM port and select samd21_xplained_pro, click on connect:
![Screenshot](https://github.com/Adjuvo/firmware-releases/raw/master/select.png "select")

2. Select the correct Binary (note: left or right SenseGloves need different versions)

3. Set the Address to 0x6000

4. Press 'Send file'

Wait for the process to complete, it could be rather slow and could last a few minutes
The following screenshot gives an overview of the steps:
![Screenshot2](https://github.com/Adjuvo/firmware-releases/raw/master/write.png "write")

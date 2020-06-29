# Firmware releases for DK1.x

## Updating firmware

### Flash tool download:
Get the Window x64 (64-bit) installer at https://github.com/shumatech/BOSSA/releases
and follow the installation instructions.

### Firmware download:
Get the latest firmware version at: http://www.github.com/Adjuvo/firmware-releases

### Preparing
Keep the boot pin pressed while you power up the SenseGlove. You can find the boot
as shown in this picture: 

The SenseGlove is now in boot mode. Start the BOSSA flash tool (in Programs > Bossa)

### Updating
1. Select the correct COM port. 
The flash programmer will notify if you selected the wrong COM port

2. Select the correct Binary (note: left or right SenseGloves need different versions)

3. Set the start address to 0x6000

4. Press 'Write'

The following screenshot gives an overview of the steps:

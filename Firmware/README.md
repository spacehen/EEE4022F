# Requisites

For Ubuntu based systems install the prerequisite packages using the following command:

**sudo apt-get install binutils gcc-avr avr-libc uisp avrdude flex byacc bison**

# Installation of Auxiliary MCU Firmware

In order to flash the auxiliary firmware onto an MCU the ISP programmer must first be connected to the ATMega328. 
Once this has been complete the source code within the folder /Firmware/Auxillary MCU must be copied to a folder named main. 

Then within the arduino IDE select File->Open and select the folder previously named "main". An editor window with all five source code files should appear. 
Within the IDE select Tools->Programmer->USBasp. Finally select Sketch->Upload Using Programmer to flash the firmware.

# Installation of Driver MCU Firmware

Once again the ISP programmer must be connected to an ATMega328 microcontroller. To build the firmware navigate to /Firmware/USB Driver MCU/USB/bin/ within a terminal and set the scripts build.sh and flash.sh to executable. Finally run build.sh followed by flash.sh. The corresponding firmware will then be flashed to the MCU.

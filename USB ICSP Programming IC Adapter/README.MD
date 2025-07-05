ArduBytes USB ICSP Programming IC Adapter Development Board

The Ardubytes USB ICSP is a development board and programmer sandwiched into one. It is designed to simplify the development stage and get you programming as soon as possible. Featuring dual SPI and UPDI programming protocols it can cater for developing a range of AVR projects. Supported by AVRDUDE for SPI and megaTinyCore for UPDI. The onboard dual 5V/3V3 supplies allow you to select the onboard voltage and the 44 pin "DIP EXT CONN" socket exposes every pin of the microcontroller, with some additional power pins to extend to your breadboard project. The 40 pin ZIF socket eases the AVRs installation with a simple lift and push of the lever and the IC is mechanically secured and electrically interfaced. In the accidental case of bricking your microcontroller via UPDI. e.g Wrong fuses. We have a built-in high voltage supply that can rescue your AVR in its time of need. All this being powered via 5V through the USB C connector.,


Features:
-	UPDI devices can be programmed via the “J2” header. Based on your need they can be configured to work with a high/low voltage reset pulse. As well as being able to isolate the UPDI/Reset pin into two separate entities for those select AVRs that require this function.
-	SPI protocol is supported via the six pin ICSP header “J3” or using the DIP Select adapters (Included) to program the 40 to 8 pin DIP ICs. 
-	If you need a serial USB adapter to monitor your serial lines or program your bootloader flashed AVR. Then the serial header “J1” is available with the necessary connections you need to do this.
- Actvity LEDS to indicate programming, serial communication and power supply rails. 
-	3.3V and 5V supplies are selectable through the “VCC Select” jumper. 500mA Max Current Output for 3.3V and 1A for 5V.
- The USB C connector requires a minimum of 5V and 2A. (It can operate on lower currents. But only if your are using it as programming/debugging adapter and not having any other peripherals drawing power)
-	To save you time and memory 😊. The jumper configurations to do each of these functions are printed on the back of the development board for your reference. A QR Code is also available to access additional information on this dev board.

How It Works?

UPDI Programming (Header J2):
1. Set jumpers on header J4 to position 1.
2. Select your supply voltage via the VCC_SLCT selection jumper. You have the option of 5V or 3.3V.
3. Select whether you want high voltage or low voltage UPDI programming via the UPDI-RST-VOLT jumper. Select LV for the selected VCC_SLCT voltage or HV for 12V.
4. Select if you want the reset signal to be combined with the UPDI signal via the UPDI-RST-ISO jumper. Enable position is to isolate the signals and disable is to combine them.
5. Using the megaTinyCore board extension. Choose Serial UPDI -230400 as the dedicated programming device.
6. To take advantage of the high voltage mode. You must remove the hashtag before the UPDI/RESET PIN Configuration Lines, in the boards.txt file.
7. Program to your hearts content :)

AVR SPI ICSP (Header J3):
1. Set jumpers on header J4 to position 2.
2. Select your supply voltage via the VCC_SLCT selection jumper. You have the option of 5V or 3.3V.
3. Use the appropriate supplied PCB module to interface the AVR with the programmer. Make sure the switch is in the same poisition. Use the diagram below to confirm correct adapter. 

![AVR SPI Adapter Modes](https://github.com/EEPUXProjects/ArduBytes/blob/main/USB%20ICSP%20Programming%20IC%20Adapter/AVR%20SPI%20Adapter%20Modes.png)

EXT USART Debugger (Header J1):
1. Set jumpers on header J4 to position 2 and 3.
2. Select your supply voltage via the VCC_SLCT selection jumper. You have the option of 5V or 3.3V.




What Is Included?

When will it be available?

More information coming soon !!! 



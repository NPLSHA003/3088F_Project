# Dual Sensing Sensation

Introduction

This project is a light and temperature sensing project that detects light and the temperature as an external environmental stimulus. The sensors are built on to a board with its own power supply that will be able to power the microcontroller and the sensors. The board with the sensors on is called the HAT and will be able to fit on the microcontroller. The temperature sensor is an analohg sensor with a built in ADC that detects the exact temperature where as the light sensor is digital and is just used to detect whether there is or is not any light. Both sensors send the data to an EEPROM which is then reaad by a microcontroller. This project can be used for many applications such as monitoring light and temperature on a farm, for security purposes in checking for any immediate change in temperature and light in a room and many more.

What you will need for this project

Hardware:
Microcontroller - STM32Discovery board (The exact one we used was from the University of Cape Town
HAT - The  Dual sensing sensation board
Some Male pin headers
3.7 V Li-ion Battery Cell
USB micro B charger
USB mini B to USB micro B cable

Software:
Kicad or Altium 
stmCubic

Tools:
Soldering Iron and some solder
Multimeter

Notes:
Microcontroller: The exact microcontroller we used was from the University of Cape Town. You should perhaps get in contact with Justin Pead from the engineering department at UCT to get the exact one making the project easier to implement.
To get the Dual Sensing sensation board you will have to order it from JLPCB using the provided Gerber, BOM(Bill of materials) and CPL(Position) files. 
You could use Kicad or Altium to change certain internal circuits on the dual sensing sensation board. Take note that you would then need to change the PCB files and get the correct gerber, BOM and CPL files.

Connecting and testing the Hardware

Connecting:
Solder male pin headers to the individual test point. Proceed to the testing before connecting the dual sensing sensation board to the microcontroller.
You can then refer to the schematic to see which pins from the DSS board connect to which pins on the microcontroller.
After this fisrt connect the microcontroller board to a laptop. 
Run stmCubic.
It should pick up the board. You can then refer to the cody reference, copy and paste the functions and run it.
You can now connect power supply of the board to the microcontroller. It will save the temperature and light data and you can just connect your laptop/pc to the microcontroller to access this data.  

Testing:
1. Using the multimeter, measure the voltage across the battery. It should be between 2.2 V and 3.7 V.
2. Insert the battery in the battery holder on the board. Measure the voltage across TP6(positive terminal) and TP5(ground terminal). If the voltage across this is O V(or anywhere below 1 V) you have inserted the battery incorrectly. Fix it and measure the voltage again just to be sure.
3. Then measure the voltage between TP11 and TP5 this should be 3.3 V or very close to it.
4. You can then insert a micro B usb charger at the charger. To check if the battery is charging measure the current between TP7 and the positive terminal of the battery it should be 1 A.
5. You can now head over back to connecting.


Licencing 

This project uses a CC BY-SA liscence. You can use this project as would like as long as you credit us and more importantly share and commit any changes/adaptations/innovations to the project.

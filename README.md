**Ethicstech LoRa Development Kit 1.1**

Ethicstech board is working with Arduino zero bootloader by default or if you want to use adafruit feather bootloader, download the bootloader using the links below and follow the procedure to flash the bootloader is given below.

1.  Arduino zero
https://github.com/arduino/ArduinoCore-samd/tree/master/bootloaders/zero

2. Adafruit feather m0
https://github.com/adafruit/Adafruit-Feather-M0-Basic-Proto-PCB

3. Link with procedure to flash your own bootloader
https://learn.adafruit.com/proper-step-debugging-atsamd21-arduino-zero-m0/restoring-bootloader

NOTE : You required programmer to flash your bootloader.

**LoRa Libraries**
We are using Radio Head library in our SDK.
https://github.com/PaulStoffregen/RadioHead

**Sample programs**
Download our getting started Transmitter & Receiver program.

Before you run your program follow our instructions.
- Here the CS pin - 5, Which is specefic to ethicstech board. In case of other boards change the CS pin based on your schematics. 

    #define RFM95_CS 5 //nss pin 
    #define RFM95_RST 9 
    #define RFM95_INT

if you are using 868 or 915 change it here
// Change to 434.0 or other frequency, must match RX's frequency. 

    #define RF95_FREQ 434


Now connect the boards with your, run the sample programs and see the datas on your Arduino serial monitor. Make sure you have attached your antenna with your board. 

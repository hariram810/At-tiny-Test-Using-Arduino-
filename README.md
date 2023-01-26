# At-tiny-Test-Using-Arduino

![Screenshot (999)](https://user-images.githubusercontent.com/118633170/214883024-6a073446-60b0-456d-9614-437880f85ebc.png)

If you have hard-time 3d printing stuff and other materials which i have provided in this project please refer the professionals for the help, [JLCPCB](https://jlcpcb.com/RNA) is one of the best company from shenzhen china they provide, PCB manufacturing, PCBA and 3D printing services to people in need, they provide good quality products in all sectors

[JLCPCB](https://jlcpcb.com/RNA)


Please use the following link to register an account in [JLCPCB](https://jlcpcb.com/RNA)

https://jlcpcb.com/RNA


Pcb Manufacturing

----------

2 layers

4 layers

6 layers

jlcpcb.com/RNA

PCBA Services

[JLCPCB](https://jlcpcb.com/RNA) have 350k+ Components In-stock. You don’t have to worry about parts sourcing, this helps you to save time and hassle, also keeps your costs down.

Moreover, you can pre-order parts and hold the inventory at [JLCPCB](https://jlcpcb.com/RNA), giving you peace-of-mind that you won't run into any last minute part shortages. jlcpcb.com/RNA

3d printing

-------------------

SLA -- MJF --SLM -- FDM -- & SLS. easy order and fast shipping makes [JLCPCB](https://jlcpcb.com/RNA) better companion among other manufactures try out [JLCPCB](https://jlcpcb.com/RNA) 3D Printing servies

[JLCPCB](https://jlcpcb.com/RNA) 3D Printing starts at $1 &Get $54 Coupons for new users

![Screenshot (1000)](https://user-images.githubusercontent.com/118633170/214883095-dc090792-961a-4207-b017-e11c384821b8.png)


The high-performance, low-power Microchip 8-bit AVR® RISC-based microcontroller combines 8 KB ISP Flash memory, 512B EEPROM, 512B SRAM, six general purpose I/O lines, 32 general purpose working registers, one 8-bit timer/counter with compare modes, one 8-bit high-speed timer/counter, USI, internal and external Interrupts, 4-channel 10-bit A/D converter, programmable watchdog timer with internal oscillator, three software selectable power saving modes, and debugWIRE for on-chip debugging. The device achieves a throughput of 20 MIPS at 20 MHz and operates between 2.7-5.5 volts.

By executing powerful instructions in a single clock cycle, the device achieves throughputs approaching one MIPS per MHz, balancing power consumption and processing speed.

![Screenshot (1001)](https://user-images.githubusercontent.com/118633170/214883130-373a83d0-2e6b-4f85-abea-98bcf2bec11f.png)

The ATtiny85 is a microcontroller in a similar vein to the but with much less IO pins, smaller memory and a smaller form factor. In fact, when we talk about the ATtiny85 we refer to the IC itself rather than the board. The ATtiny85 can be used as a bare chip on a breadboard, as long as you can supply the correct power for the device. 

Despite the small package, the ATtiny85 comes with a remarkable number of ways in which we can interface. At the most basic level, we have 5V logic digital I/O pins, three of which can also be used as analog pins for use with components such as the TMP36 sensor. Four of the available pins can also be used with Pulse Width Modulation (PWM). Also available is I2C and SPI for use with other types of sensors and devices.

As per the datasheet, it has 8 KB of flash, an 8-MHz internal RC oscillator that can be used as the default clock & 512 bytes of EEPROM and SRAM.

In achieving a throughput of 20 MIPS, it takes 20 MHz and operates between 2.7-5.5V.

It also has two 8-bit timers or counters, one high-speed, with four pulse-width modulations (PWM) outputs, and a four-channel 10-bit ADC.

An ADC converter with a 10 bit & programmable watchdog timer is added to the device which makes it suitable for resetting the device in case it gets stuck in an infinite loop and sensor interfacing.

![Screenshot (1002)](https://user-images.githubusercontent.com/118633170/214883190-ce1ff57f-c187-48be-a77a-a017507b79c8.png)

We shall be using the Arduino IDE to write the code for this project. So if not already installed, download a copy from the Arduino website and install.

Open the Arduino application and click on File >> Preferences and past the following into the Additional Boards Managers URLs: dialog.

http://digistump.com/package_digistump_index.json

Next, go to Tools >> Board >> Boards Manager and from the drop-down menu select “Contributed”.

Although it consists of 8 pins only, it can perform almost every function that a simple microcontroller can do. We will get a better idea of its functionality in the pinout specification.

What does the number 85 in ATtiny85 represents?
In the ATtiny series, the first digit that comes after ATtiny represents the flash memory in kibibyte (KiB). Thus, an ATtiny85 consists of 8KiB flash memory.

The second digit represents the model type. You can expect more powerful and newer models to have higher numbers. Here you can see that ATtiny85 is a 2005 model.

Select the “Digistump AVR Boards” and click Install.

![Screenshot (1003)](https://user-images.githubusercontent.com/118633170/214883218-d35f7f91-407d-4f6e-b2a4-5cf963f222fe.png)
![Screenshot (1004)](https://user-images.githubusercontent.com/118633170/214883232-5168036e-31c0-44a8-a1c8-fcd5bba25b8d.png)


The install process will take some time, but once completed the installation should trigger an auto install of the drivers for the board.

If the driver install fails to run after adding the board to your list, open the command prompt and enter the following command. Remember to change the USERNAME to match your own!

![Screenshot (1005)](https://user-images.githubusercontent.com/118633170/214883256-737465fa-3c5c-4d42-9008-d1cd6ba03e32.png)
![Screenshot (1006)](https://user-images.githubusercontent.com/118633170/214883271-a135ca8d-a269-439c-8b66-d99a59300055.png)

C:\Users\**YOUR USERNAME**\AppData\Local\Arduino15\packages\digistump\tools\micronucleus\2.0a4\post_install.bat

This will install the drivers for the ATtiny85, and there may be a red cross in the post install screen, but we can confirm that the instal is correct.

To use the ATtiny85 in the Arduino IDE we need to set it as our board. 

Go to Tools >> Board >> and select Digispark (Default - 16.5MHz) don’t worry about the Port.

Building the circuit
On the breadboard, build the circuit as shown in the diagram. The LED cathode (-) legs are on the left of the image, and they connect to a single ground pin on the ATtiny85 via a 330 Ohm resistor. The male to male jumper jerky connects the 330 Ohm resistors for two of the LEDs to the third, creating a single Ground connection that is connected to the ATtiny85. The anode (+) leg of the LED is connected directly to Pins 0,1,2 using the male to female jumper jerky.

Don’t insert the ATTiny85 just yet. First, we need to write some code.

In the Arduino IDE, we shall set up the three pins (0,1,2) that will be used as outputs first and will flash the LEDs attached to them.

Now for the code that will continually loop round, creating the effect of cycling through the LEDs. We start by turning on each LED (HIGH) and then using a delay of 1/10 of a second between each LED turning on.

![Screenshot (1007)](https://user-images.githubusercontent.com/118633170/214883326-36f10d0c-41a5-47a5-80c7-808adbd11aa7.png)

![Screenshot (1008)](https://user-images.githubusercontent.com/118633170/214883349-7344b552-b827-4fb6-ab58-1f6390f281d9.png)


void loop()

{

  digitalWrite(0, HIGH);

  delay(100);

  digitalWrite(1, HIGH);

  delay(100);

  digitalWrite(2, HIGH);

  delay(100);
Still inside of the loop, we now need to turn off the LEDs in reverse order by pulling the output LOW for each LED. We also keep the same delay between LEDs to create a rhythmic looping pattern.

  digitalWrite(2, LOW);

  delay(100);

  digitalWrite(1, LOW);

  delay(100);

  digitalWrite(0, LOW);

  delay(100);

}
Flashing the code

![Screenshot (1012)](https://user-images.githubusercontent.com/118633170/214883386-3378bf61-d922-4642-9935-86ac5cb2907a.png)


To write the code to our ATTiny85 click on Sketch >> Upload or click on the right-hand arrow. In the output window, at the bottom of the Arduino IDE, you will be prompted to insert the ATtiny85, do this and the code will be flashed to the ATtiny85 within a few seconds. Your LEDs will now start flashing in a cycling pattern.

Notes

![Screenshot (1015)](https://user-images.githubusercontent.com/118633170/214883496-eca78678-9bc6-44d2-943d-b84610254cff.png)
![Screenshot (1013)](https://user-images.githubusercontent.com/118633170/214883519-5b8c19aa-1515-4396-b517-b55ecdfcbab5.png)

↑ timers x waveform generators
↑ timer0 can use clocks up to the core clock, timer1 can use clocks up to 64MHz
↑ 4 pins are usable, but only 3 unique generators can be attached. The 4th pin would be the inverse of OC1B on the 3rd pin.
↑ Inverted outputs with configured dead zones can be set up for the 64MHz-capable timer1.
↑ timer/counter1 is a 10-bit counter that can use clocks to 64MHz.
↑ The PWM channels are based on the 10 bit counter with a maximum of 64MHz clock. Each PWM channel can generate two outputs, normal and inverted, on distinct IO pins. Each pair of outputs can be configured to have a dead-time between their on-states.
↑ ADC only on ATtiny5/10, and channels are 8 bits instead of 10
Package column - the number after the dash is the number of pins on the package. DIP packages in this table are 0.3 inches (7.62 mm) row-to-row. SOwww means SOIC package with a case width of 'www' in thousandth of an inch. Though some package types are known by more than one name, a common name was chosen to it easier to compare packages.
UART/I²C/SPI columns - green cell means a dedicated peripheral, * yellow cell means a multi-feature peripheral that is chosen by setting configuration bits. Most USART peripherals support a minimum choice between UART or SPI, where as some might support additional choices, such as LIN, IrDA, RS-485.
Timers column - recent families add a 12-bit timer, plus a 16-bit Real Time Counter (RTC) that is driven by a 32.768KHz clock (feature designated with 'R' in the table).
ADC chans column - the total number of analog channels that are multiplex into the ADC input. Most parts have one ADC, a few have two ADC.
Pgm/Dbg column - flash programming and debugging protocols: HVPP means High Voltage Parallel Programming 12V protocol, HVSP means High Voltage Serial Programming 12V protocol, ISP means In-System Programmable protocol, uses SPI to program the internal flash. TPI is Tiny Programming Interface. dW means debugWIRE protocol. UPDI means Unified Program and Debug Interface protocol (newest)
Abbreviations

![Screenshot (1011)](https://user-images.githubusercontent.com/118633170/214883567-dd0dbf97-9321-45de-8b01-a5305890dc4a.png)

TWI: Many of Atmels microcontrollers contain built-in support for interfacing to a two-wire bus, called Two-Wire Interface. This is essentially the same thing as the I²C interface by Philips, but that term is avoided in Atmel's documentation due to trademark issues.
USI: Universal Serial Interface (not to be confused with USB). The USI is a multi-purpose hardware communication module. With appropriate software support, it can be used to implement an SPI, interface. USART peripherals have more features than USI peripherals.

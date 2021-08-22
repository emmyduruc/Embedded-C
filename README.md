# MICROCONTROLLER (EMBEDDED C PROGRAMMING) WITH NASSI-SCHNIEDERMANN DIAGRAM
##Project file name LEDwithSWITCHES
###This project consist of the first approach to microcontrollers and port configuration with embedded C programming
 Program **"Flashing LED with Switches”**
...*The switches must first be enabled, set as ”Digital Input” and ”Weak Pull Up”
...*(WPU). For WPU use the following register: GPIO_PORTJ_AHB_PUR_R = 0x03; // WPU for PIN PJ0 and PJ1

##Project file name LEDwithSWITCHES
#### Motivation
The goal of this laboratory exercise is to get acquainted with the configuration and use of the GeneralPurpose Timer Module of the TIVA EK-TM4C1294XL Launchpad.

#### Specific application
The Launchpad contains four LEDs connected to GPIO pins in ports F and N. We can turn the LEDs on
and off by driving the pins high and low, respectively. The exact pins assignment can be found in the
figure below.

####Approach
1. wrote a function configPorts() that does all the necessary GPIO port configurations
2. wrote a function configTimer1A() that configures Timer1A for 16-bit compare mode, upwards
counting, with optimum prescaler. that the interval load value to periodically give a timeout every
second.
 **Go to the file directory to view code and attached presentation with regards to this lab work**

##Project file name ADC
1. To sample the output of the internal on-chip temperature
sensor instead of an analog channel with sample Sequencer 0. The ADC0 is to be
started by software triggering (see ADC0_PSSI_R register) each time a new
value is to be measured.

2. The temperature value was configures to be calculated from the digital ADC output and to
be printed on the console of the CCS with printf(). The temperature value was
 updated and initilize an output every 1s. The intervall is to be controlled by a General
Purpose Timer Module in compare mode.

3. The temperature sensor was sampled four times in a sequence by using four successive channels in
Sequencer 0. The average value was calculated from all four values and
output was derived.
 **Go to the file directory to view code and attached presentation with regards to this lab work**
 
 
##Project file name 

###Querying LEDs by pressing a push button,
 Interrupt Handler IntPortJHandler()
 
 ####SWITCH1 is integrated into the project
the associated port J(0) was configured to generate an interrupt that ignites a rising edge
condition. i implemented an interrupt handler IntPortJHandler() that queries the current status of
the LEDs and add the end i could be able to Test the function of the interrupt handler. When pressing the button SW1, an
output of the type '#1234<CR>' must appear in the terminal window which is the primary aim of the lab work

# Component Library

## Table of Contents
1. [TI 22CNONK E4](#ti-22cnonk-e4)
2. [TI L293DNE](#ti-l293dne)
3. [TI L293D](#ti-l293d)
4. [TI SN754410NE](#ti-sn754410ne)

---

## TI 22CNONK E4
**Datasheet:** [SN74HC595](https://www.ti.com/lit/ds/symlink/sn74hc595.pdf?ts=1722662724501&ref_url=https%253A%252F%252Far.mouser.com%252F)

**Description:**  
The SN74HC595 is an 8-bit shift register with output latches and three-state outputs. It can be used for applications requiring high-speed data transfer and minimal pin usage.

**Features:**
- **Model:** SN74HC595
- **Type:** 8-bit Serial-in, Parallel-out Shift Register
- **Input Voltage Range:** 2V to 6V
- **Maximum Output Current:** Not specified in datasheet
- **Switching Frequency:** Not specified in datasheet
- **Efficiency:** Not applicable
- **Adjustable Output:** Not applicable

**Pin Configuration:**
- **Pin 1 (QB):** Parallel data output bit 1
- **Pin 2 (QC):** Parallel data output bit 2
- **Pin 3 (QD):** Parallel data output bit 3
- **Pin 4 (QE):** Parallel data output bit 4
- **Pin 5 (QF):** Parallel data output bit 5
- **Pin 6 (QG):** Parallel data output bit 6
- **Pin 7 (QH):** Parallel data output bit 7
- **Pin 8 (GND):** Ground
- **Pin 9 (QH’):** Serial output
- **Pin 10 (SRCLR):** Shift register clear (active low)
- **Pin 11 (SRCLK):** Shift register clock input
- **Pin 12 (RCLK):** Storage register clock input
- **Pin 13 (OE):** Output enable input (active low)
- **Pin 14 (SER):** Serial data input
- **Pin 15 (QA):** Parallel data output bit 0
- **Pin 16 (VCC):** Supply voltage

**Applications:**
- LED display control
- Data bus expansion
- Serial-to-parallel data conversion

**Fritzing Files:**
1. [Fritzing file 1](https://fritzing.org/projects/sn74hc595)
2. [Fritzing file 2](https://fritzing.org/projects/74hc595-led-bar-graph)
3. [Fritzing file 3](https://fritzing.org/projects/shift-register-74hc595)

---

## TI L293DNE
**Description:**  
The L293DNE is a quadruple high-current half-H driver. It is designed to provide bidirectional drive currents of up to 600 mA at voltages from 4.5 V to 36 V. It is ideal for driving inductive loads such as relays, solenoids, DC and bipolar stepping motors, as well as other high-current/high-voltage loads in positive-supply applications.

**Features:**
- **Model:** L293DNE
- **Type:** Quadruple Half-H Driver
- **Input Voltage Range:** 4.5V to 36V
- **Maximum Output Current:** 600mA per channel
- **Switching Frequency:** Not specified in datasheet
- **Efficiency:** Not specified
- **Adjustable Output:** No

**Pin Configuration:**
- **Pin 1 (1, 9EN):** Enable input for 1st driver
- **Pin 2 (1A):** Input 1 for 1st driver
- **Pin 3 (1Y):** Output 1 for 1st driver
- **Pin 4 (GND):** Ground
- **Pin 5 (GND):** Ground
- **Pin 6 (2Y):** Output 2 for 2nd driver
- **Pin 7 (2A):** Input 2 for 2nd driver
- **Pin 8 (VCC2):** Supply voltage for motor
- **Pin 9 (3, 9EN):** Enable input for 2nd driver
- **Pin 10 (3A):** Input 3 for 3rd driver
- **Pin 11 (3Y):** Output 3 for 3rd driver
- **Pin 12 (GND):** Ground
- **Pin 13 (GND):** Ground
- **Pin 14 (4Y):** Output 4 for 4th driver
- **Pin 15 (4A):** Input 4 for 4th driver
- **Pin 16 (VCC1):** Logic supply voltage

**Applications for Home Arduino Robot Hobbyists:**
- Motor driver for small robots
- Controlling the direction and speed of DC motors
- Stepper motor driver for precise control in robotic arms

---

## TI L293D
**Description:**  
The L293D is a quadruple high-current half-H driver with similar specifications to the L293DNE. It is also designed to drive inductive loads such as relays, solenoids, DC and bipolar stepping motors.

**Features:**
- **Model:** L293D
- **Type:** Quadruple Half-H Driver
- **Input Voltage Range:** 4.5V to 36V
- **Maximum Output Current:** 600mA per channel
- **Switching Frequency:** Not specified in datasheet
- **Efficiency:** Not specified
- **Adjustable Output:** No

**Pin Configuration:**
- **Pin 1 (1, 9EN):** Enable input for 1st driver
- **Pin 2 (1A):** Input 1 for 1st driver
- **Pin 3 (1Y):** Output 1 for 1st driver
- **Pin 4 (GND):** Ground
- **Pin 5 (GND):** Ground
- **Pin 6 (2Y):** Output 2 for 2nd driver
- **Pin 7 (2A):** Input 2 for 2nd driver
- **Pin 8 (VCC2):** Supply voltage for motor
- **Pin 9 (3, 9EN):** Enable input for 2nd driver
- **Pin 10 (3A):** Input 3 for 3rd driver
- **Pin 11 (3Y):** Output 3 for 3rd driver
- **Pin 12 (GND):** Ground
- **Pin 13 (GND):** Ground
- **Pin 14 (4Y):** Output 4 for 4th driver
- **Pin 15 (4A):** Input 4 for 4th driver
- **Pin 16 (VCC1):** Logic supply voltage

**Applications for Home Arduino Robot Hobbyists:**
- Motor driver for small robots
- Controlling the direction and speed of DC motors
- Stepper motor driver for precise control in robotic arms

---

## TI SN754410NE
**Description:**  
The SN754410NE is a quadruple high-current half-H driver designed to provide bidirectional drive currents of up to 1 A at voltages from 4.5 V to 36 V. It is ideal for driving inductive loads such as relays, solenoids, DC and bipolar stepping motors, as well as other high-current/high-voltage loads in positive-supply applications.

**Features:**
- **Model:** SN754410NE
- **Type:** Quadruple Half-H Driver
- **Input Voltage Range:** 4.5V to 36V
- **Maximum Output Current:** 1A per channel
- **Switching Frequency:** Not specified in datasheet
- **Efficiency:** Not specified
- **Adjustable Output:** No

**Pin Configuration:**
- **Pin 1 (1, 9EN):** Enable input for 1st driver
- **Pin 2 (1A):** Input 1 for 1st driver
- **Pin 3 (1Y):** Output 1 for 1st driver
- **Pin 4 (GND):** Ground
- **Pin 5 (GND):** Ground
- **Pin 6 (2Y):** Output 2 for 2nd driver
- **Pin 7 (2A):** Input 2 for 2nd driver
- **Pin 8 (VCC2):** Supply voltage for motor
- **Pin 9 (3, 9EN):** Enable input for 2nd driver
- **Pin 10 (3A):** Input 3 for 3rd driver
- **Pin 11 (3Y):** Output 3 for 3rd driver
- **Pin 12 (GND):** Ground
- **Pin 13 (GND):** Ground
- **Pin 14 (4Y):** Output 4 for 4th driver
- **Pin 15 (4A):** Input 4 for 4th driver
- **Pin 16 (VCC1):** Logic supply voltage

**Applications:**
- Motor driver for small robots
- Controlling the direction and speed of DC motors
- Stepper motor driver for precise control in robotic arms

## Component: LM2596 DC-DC Converter Module
The LM2596 DC-DC converter module is a buck (step-down) voltage regulator. It can step down an input voltage (IN+) to a lower output voltage (OUT+).

**Features:**
- **Model:** LM2596
- **Type:** DC-DC Buck Converter
- **Input Voltage Range:** 4V to 40V
- **Output Voltage Range:** 1.25V to 37V
- **Maximum Output Current:** 3A
- **Switching Frequency:** 150 kHz
- **Efficiency:** Up to 92%
- **Adjustable Output:** Yes (via potentiometer)
**Pin Configuration:**
- **IN+:** Input positive
- **IN-:** Input negative
- **OUT+:** Output positive
- **OUT-:** Output negative
**Components on Board:**
- **Inductor:** 47µH
- **Capacitors:**
- Input Capacitor: 220µF, 35V
- Output Capacitor: 100µF, 50V
- **Adjustable Potentiometer:** For output voltage adjustment
**Applications:**
- Battery-powered projects
- Portable electronics
- Power supply for microcontrollers
- Solar power projects
- General voltage regulation
**Datasheet Links:**
- [LM2596 Datasheet](https://www.ti.com/lit/ds/symlink/lm2596.pdf)
**Notes:**
- Ensure adequate cooling for the module when drawing high currents.
- Adjust the output voltage before connecting the load to avoid damage.

## XL6009E1 DC-DC Converter Module
The XL6009E1 is a DC-DC step-up (boost) converter module. It is based on the XL6009 integrated circuit, <br>
which is a high-efficiency switching regulator designed for applications requiring stable and adjustable <br>
output voltage. This module is commonly used for boosting lower voltage to a higher voltage in various electronic projects.

### Specifications
- **Input Voltage Range:** 3V to 32V
- **Output Voltage Range:** 5V to 35V
- **Output Current:** 3A (maximum)
- **Efficiency:** Up to 94%
- **Switching Frequency:** 400kHz
- **Dimensions:** 43mm x 21mm x 14mm

### Features
- High conversion efficiency.
- Wide input voltage range.
- Adjustable output voltage.
- Built-in thermal shutdown function.
- Over-current protection.
- Soft start function.

### Pin Configuration
- **IN+**: Input Positive
- **IN-**: Input Negative
- **OUT+**: Output Positive
- **OUT-**: Output Negative

### Applications
- Battery-powered devices.
- Boosting voltage for microcontrollers.
- Powering high voltage devices from a low voltage source.
- Solar power projects.

### Usage Instructions
1. **Connect the Input:** Connect the input voltage to the IN+ and IN- pins. Ensure the input voltage is within the specified range (3V to 32V).
2. **Connect the Output:** Connect the load to the OUT+ and OUT- pins.
3. **Adjust the Output Voltage:** Use the onboard potentiometer to adjust the output voltage to the desired level. Measure the output voltage with a multimeter while adjusting.

### Additional Notes
- Ensure that the input voltage is always lower than the desired output voltage for proper operation.
- The module can get hot during operation, especially at higher currents. Ensure adequate ventilation or heatsinking if necessary.

### Fritzing File
[Fritzing file for XL6009E1 DC-DC Converter Module](https://fritzing.org/projects/xl6009-dc-dc-boost-converter)

## Manufacturer's Datasheet
[XL6009 Datasheet](http://ww.notworking.xxx/xl6009-datasheet)

## Summary
The XL6009E1 DC-DC converter module is an efficient and versatile solution for stepping up voltage in various <br>
electronic projects. Its wide input range and adjustable output make it suitable for a variety of applications.

## 5V microUSB 1A 18650 Lithium Battery Charging Board Charger Module with Protection

The 5V microUSB 1A 18650 Lithium Battery Charging Board Charger Module is designed to charge single-cell 18650 lithium batteries efficiently and safely. It integrates protection circuits to prevent overcharging, over-discharging, and short circuits, ensuring the battery's longevity and safety.

### Specifications
- **Input Voltage:** 5V (microUSB)
- **Charge Current:** 1A (maximum)
- **Battery Type:** 18650 Lithium-ion
- **Protection:** Overcharge, over-discharge, and short-circuit protection
- **Dimensions:** 25mm x 19mm x 10mm

### Features
- Compact and lightweight design.
- Integrated microUSB port for easy charging.
- Built-in battery protection circuits.
- LED indicators for charging status.
- Automatic charge termination.

### Pin Configuration
- **B+**: Battery positive terminal
- **B-**: Battery negative terminal
- **OUT+**: Output positive terminal
- **OUT-**: Output negative terminal

### Applications
- Portable electronics.
- Power banks.
- DIY battery-powered projects.
- Solar battery charging systems.

### Usage Instructions
1. **Connect the Battery:** Solder the 18650 lithium battery to the B+ and B- terminals. Ensure correct polarity to avoid damage.
2. **Connect the Load:** Connect the device you want to power to the OUT+ and OUT- terminals. The module will manage the charging and discharging processes.
3. **Power the Module:** Connect a 5V microUSB power source to the module. The charging process will start automatically.
4. **Monitor the LEDs:** The module has two LED indicators. The red LED indicates charging, while the blue LED indicates that the battery is fully charged.

### Additional Notes
- Ensure proper ventilation as the module may get warm during operation.
- Do not exceed the specified input voltage to avoid damaging the module.
- Disconnect the battery from the module when not in use for extended periods to prevent deep discharge.

### Fritzing File
[Fritzing file for 5V microUSB 1A 18650 Lithium Battery Charging Board Charger Module](https://fritzing.org/projects/5v-microusb-1a-18650-charging-module)

### Manufacturer's Datasheet
[Datasheet for 5V microUSB 1A 18650 Lithium Battery Charging Board Charger Module](https://www.handsontec.com/dataspecs/module/18650-Lithium%20charger.pdf)

### Examples
- [Example 1](https://www.instructables.com/18650-Battery-Charger/)
- [Example 2](https://www.hackster.io/news/5v-1a-18650-lithium-battery-charging-board-charger-module-7658dbd73f)
- [Example 3](https://www.dfrobot.com/product-1574.html)

### Summary
The 5V microUSB 1A 18650 Lithium Battery Charging Board Charger Module is an excellent solution for efficiently and safely charging 18650 lithium batteries. Its built-in protection circuits, easy-to-use microUSB input, and compact size make it ideal for various portable and DIY electronic projects.

## KY-033 Infrared Line Tracking Sensor

**Description:**  
The Infrared Line Tracking Sensor is designed for use in robotics and automation projects to detect and follow a line. It uses infrared light to detect the difference in reflectivity between the line and the background surface, providing a digital output signal indicating the presence or absence of the line.

**Features:**
- **Model:** Infrared Line Tracking Sensor
- **Type:** Reflective Infrared Sensor
- **Operating Voltage:** 3.3V to 5V
- **Output Type:** Digital
- **Detection Range:** 0.1 cm to 1.5 cm (optimal range varies with surface reflectivity)
- **Adjustable Sensitivity:** Yes, via onboard potentiometer
- **Mounting Hole:** Provided for secure attachment

**Pin Configuration:**
- **Pin 1 (OUT):** Digital output signal
- **Pin 2 (VCC):** Power supply (3.3V to 5V)
- **Pin 3 (GND):** Ground

**Applications:**
- Line-following robots
- Edge detection in robotic projects
- Object sorting on conveyor belts based on line marking

**Links:**
- [Datasheet](https://arduinomodules.info/ky-033-line-tracking-sensor-module)
- [Fritzing File](https://electropeak.com/learn/interfacing-tcrt5000-infrared-line-tracking-sensor-with-arduino)
- [Additional Resource](https://www.electroniclinic.com/ky-033-line-tracking-sensor-arduino-circuit-and-programming)
++
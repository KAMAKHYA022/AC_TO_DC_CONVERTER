# AC to DC Converter PCB Project

## 1. Introduction

  Electrical power is supplied in two main forms: Alternating Current (AC) and Direct Current (DC). Understanding these two types of currents is essential before diving into the AC to DC conversion 
  process.

##  What is AC (Alternating Current)?

   AC is an electrical current that periodically reverses direction. It is commonly used for power transmission and is the type of electricity supplied to homes and industries. The voltage of AC varies 
   sinusoidally with time.

##  What is DC (Direct Current)?

   DC is a unidirectional flow of electric charge. It is used in batteries, electronic circuits, and low-voltage applications like mobile phones, laptops, and embedded systems.

## 2. What is an AC to DC Converter?

   An AC to DC Converter is an electronic circuit that converts AC voltage into DC voltage. This is necessary because many electronic devices operate on DC power, but electrical grids provide AC power.

## Why is AC to DC Conversion Required?

  Most electronic circuits require a stable DC supply.

  AC is more efficient for long-distance transmission, but DC is needed for circuits and devices.

  Batteries and microcontrollers work on DC power.

## 3. Types of AC to DC Converters

  There are several types of AC to DC converters based on their design and working principle:

  Half-Wave Rectifier – Uses a single diode, converts only half of the AC waveform.

  Full-Wave Rectifier – Uses two diodes or a bridge rectifier to convert both halves of the AC waveform.

  Bridge Rectifier – Uses four diodes to provide full-wave rectification with better efficiency.

## 4. Designing a 12V AC to DC Converter

  For this project, we design a 12V AC to DC Converter using KiCad for schematic and PCB design. The circuit includes a transformer, full-wave rectifier, smoothing capacitor, voltage regulator, and LED 
  indicator.

  Components Used:

  Transformer (X1) – Steps down 220V AC to 12V AC.

  Bridge Rectifier (D1-D4, 1N4007 diodes) – Converts AC to pulsating DC.

  Capacitor (C1, 1000µF) – Smooths the pulsating DC.

  Voltage Regulator (U1, 7812 IC) – Provides a steady 12V DC output.

  Resistors (R1, R2) – Current limiting resistors for circuit protection.

  LED Indicator (D5) – Shows power status.

## 5. PCB Design in KiCad

  The schematic is designed in KiCad, ensuring correct component placement and PCB layout. The PCB layout is optimized to minimize noise and improve efficiency.
## Designing a 12V AC to DC Converter

### Schematic Design in KiCad
![Schematic Design](https://github.com/KAMAKHYA022/AC_TO_DC_CONVERTER/blob/main/SCHEMATIC.JPG) 

### PCB Layout
![PCB Layout](https://github.com/KAMAKHYA022/AC_TO_DC_CONVERTER/blob/main/PCB.JPG)

### Simulation in Proteus
![Proteus Simulation](https://github.com/KAMAKHYA022/AC_TO_DC_CONVERTER/blob/main/proteus.JPG)


## 6. Simulation in Proteus

To verify circuit functionality before manufacturing, the schematic is simulated in Proteus:

Transformer steps down 220V AC to 12V AC.

Bridge rectifier converts AC to DC.

Capacitor smooths the DC voltage.

IC 7812 ensures a regulated 12V DC output.

LED indicates circuit operation.

## 7. Why These Components Were Chosen?

7812 Voltage Regulator – Provides a steady 12V DC output with overvoltage protection.

1000µF Capacitor – Smooths rectified DC to reduce ripple.

10Ω Resistor (R2) – Helps with voltage stabilization.

2.2kΩ Resistor (R1) with LED – Limits current to the LED for indicating circuit operation.

## 8. Conclusion

This AC to DC converter provides a regulated 12V DC output from 220V AC input. The design ensures efficiency and reliability for powering various electronics. The project demonstrates PCB design, simulation, and implementation of a real-world power supply circuit.

Future Improvements:

Adding a heat sink to the 7812 regulator for better thermal management.

Designing a dual-output version for 5V and 12V DC supplies.

Implementing a switching regulator for better efficiency.

Tools Used:

✅ KiCad – Schematic & PCB Design
✅ Proteus – Circuit Simulation

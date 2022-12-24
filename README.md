# MicroFoundry-XC6194A-PH-Breakout-PCB
Information about the XC6194A Breakout with PH connectors.

## XC6194 Description
The TOREX XC6194A series device is load switch with functions best suited for a momentary push button and features to enhance battery operated devices.

The built-in high side switch is turned on by a momentary switch (Turning off is also possible on the A type.) and turned off by a HIGH level signal into the SHDN pin from the MCU or the like. The high side switch is turned on and latched by inputting LOW level signal from a momentary switch to the SW pin. It is possible to shut down (OFF) by inputting a 1-pulse HIGH level signal from an MCU or the like to the SHDN pin.

## XC6194 Features

| Feature              | Description                     |
| -------------------- | ------------------------------- |
| Input Voltage Range  | 1.8V ~ 6.0V                     |
| Stand-by Current     | 0.001μA (TYP.) / Turn-Off state |
| Quiescent Current    | 0.13μA (TYP.) / Turn-On state   |
| Output Current       | 1000mA (VIN=2.0V, Ta=25℃)      |
| Turn-On Delay Time   | 0.2s, 1.0s, 3.0s or 5.0s        |
| Turn-Off Method      | <ul><li>By inputting “H” voltage to the SHDN pin.</li><li>By inputting “L” voltage for the duration of TOFFD to the SW pin.</li></ul>|
| Turn-Off Delay Time  | 3s, 5s, 10s or 15s |
| Added Functions      | <ul><li>Power Good function (The PG pin)</li><li>Shutdown function (the SHDN pin)</li></ul>|
| Protective Functions | <ul><li>Output capacitor inrush current limit soft-start</li><li>Output capacitor discharge function</li><li>Output short circuit protection</li><li>Thermal shutdown</li></ul>|
| Operating Ambient Temperature | -40℃ ~ 85℃ | 
| Package | USP-8B06 (2.0 x 2.0 x h0.33mm) |

## The Micro Foundry XC6194A Breakout
This is a practical application of the XC6194A IC with JST style PH series connectors for VIn/VOut, a JST SH style connector to provide IO access to the XC6194A functions, essential passive components required for basic operation and voltage-in/voltage-out LEDs. An additional 1.0mm pitch FFC connector offers expansion capabilities for optional breakout PCBs with features like voltage level signal translation and the ability to drive up to 3 LEDs for momentarty switches w/RGB LEDs such as those sold by Adafruit. The PCB is 26x26 mm with 4x 2.5mm mounting holes.

## Pinouts
### VIn/VOut
1. VIn or VOut
2. GND
### IO
1. VIn  - Voltage In 
2. GND  - Ground
3. VOut - Voltage Out
4. SW   - Momentary Switch Input (Active LOW)
5. PG   - Power Good Output (Active HIGH)
6. SHDN - Shutdown Input (Active HIGH)
### Expansion
1. VIn  - Voltage In 
2. GND  - Ground
3. VOut - Voltage Out
4. SW   - Momentary Switch Input (Active LOW)
5. PG   - Power Good Output (Active HIGH)
6. SHDN - Shutdown Input (Active HIGH)

**NOTE:** All IO/Expansion pins operate at VIn level. If the XC6194A IO are connected to an MCU, please verify voltage compatability or utilize one of the optional expansion PCBs.

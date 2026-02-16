# Mystical-Ouija-Board
an Arduino Nano Ouija Board

Mystical Ouija Board User Manual

Overview

An electronic Ouija board that uses capacitive/resistance touch sensors to move a planchette across a digital board displayed on an OLED screen. 
Theory is that a spirit or entity may communicate through this electronic devise by manipulating the human body.
 
For Entertainment Purposes Only! Use with Caution!

Hardware Requirements
Arduino Nano
128x64 OLED Display (SSD1306, I2C)
4 Touch Sensors connected to analog pins A0-A3
I2C Connections: SDA/SCL to display

Wiring
Touch Sensors: Connect to A0, A1, A2, A3
OLED Display: Connect via I2C (typically A4=SDA, A5=SCL)
Power: 5V and GND to all components

How It Works
Touch Detection: Monitors capacitance/resistance changes on 4 sensors
Sensitivity: Threshold set to 5 for responsive movement
Planchette: Appears as a transparent ring on the board

Usage Instructions
1. Power On: Upload sketch and power the Arduino
2. Touch Sensors: Lightly touch any of the 4 sensors
3. Watch Movement: Planchette moves based on touch intensity
4. Serial Monitor: View debug info at 9600 baud for troubleshooting

Troubleshooting
No Movement: Check sensor connections and threshold value
Too Sensitive: Increase threshold value (line 101)
Display Issues: Verify I2C address is 0x3C

Customization
Adjust movementDivisor (line 112) for movement speed
Modify threshold (line 101) for sensitivity
Change minMovement (line 113) for minimum motion


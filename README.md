Fire and Smoke Detection System Using Arduino:

Overview:


This project aims to create a fire and smoke detection system using an Arduino board, flame sensor, smoke sensor, LED, and buzzer. The system detects the presence of fire or smoke and alerts the user with visual and audio signals.

Components:
Arduino Board (e.g., Arduino Uno)

Flame Sensor (e.g., YG1006)

Smoke Sensor (e.g., MQ2)

LED (Red and Green)

Buzzer

Breadboard and Jumper Wires

9V Battery and Battery Clip (optional, if using a portable power source)


Setup:

Connect the flame sensor to the Arduino:

VCC to 5V

GND to GND

OUT to digital pin 2

Connect the smoke sensor to the Arduino:

VCC to 5V

GND to GND

A0 to analog pin A0

Connect the LED and buzzer to the Arduino:

Red LED: Pin 12

Green LED: Pin 11

Buzzer: Pin 10

Connect the components to the breadboard using jumper wires.


Usage:


Upload the code to your Arduino board using the Arduino IDE. When the system detects smoke or fire, the red LED will turn on, the green LED will turn off, and the buzzer will sound.

Troubleshooting
No Response: Ensure all connections are secure and components are properly connected.

False Alarms: Adjust the sensorThres value in the code to fine-tune the sensitivity.

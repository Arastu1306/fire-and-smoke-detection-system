Fire and Smoke Detection System using Arduino:

Overview:

This project demonstrates the development of a Fire and Smoke Detection System using an Arduino platform. The system is designed to monitor environmental conditions and detect the presence of fire and smoke. When a fire or smoke is detected, it triggers an alert system (such as an LED, buzzer, or both) to notify users of potential danger. This project is ideal for home security, industrial applications, or any environment that requires fire safety monitoring.

Features:

Fire Detection:Uses a Flame Sensor to detect fire in the vicinity.
Smoke Detection:Uses a MQ-2 Gas Sensor to detect smoke or harmful gases.
Alert System: Utilizes a Buzzer and/or LED to alert when fire or smoke is detected.
Arduino-based: Simple integration with Arduino for easy setup and customization.
Low Cost: The system uses inexpensive sensors and components.

Components Required:

Arduino Uno or any compatible Arduino board
Flame Sensor
MQ-2 Gas Sensor (Smoke sensor)
Buzzer
LED (for visual indication)
Resistors (for LED and sensor circuits)
Breadboard and jumper wires
Power Supply (for Arduino)

Circuit Diagram:

Flame Sensor:

Connect the VCC of the sensor to 5V on the Arduino.
Connect the GND of the sensor to the GND of the Arduino.
Connect the A0 pin of the sensor to an analog input pin (e.g., A0) on the Arduino.

MQ-2 Gas Sensor:

Connect the VCC of the sensor to 5V on the Arduino.
Connect the GND of the sensor to the GND of the Arduino.
Connect the A0 pin of the sensor to an analog input pin (e.g., A1) on the Arduino.

Buzzer and LED:

Connect the positive terminal of the buzzer and the LED to a digital pin on the Arduino (e.g., D2 for the buzzer, D3 for the LED).
Connect the negative terminal to GND through appropriate resistors.

How It Works:

Flame Detection: The flame sensor continuously monitors the environment. When it detects a flame (or significant heat source), it sends a low value to the analog pin on the Arduino. The system reacts by triggering an alert (buzzer and LED).

Smoke Detection: The MQ-2 sensor detects smoke or harmful gases by measuring the concentration in the air. When the smoke level exceeds a set threshold, the system activates the buzzer and LED.

Alert: If either the flame sensor detects fire or the smoke sensor detects smoke, the system triggers a buzzer and an LED to alert users about the fire hazard.

Calibration:

MQ-2 Gas Sensor: The MQ-2 sensor requires calibration based on the environment it is placed in. You may need to adjust the threshold value in the code for better accuracy. The default threshold in the code is set to 300.
Flame Sensor: The flame sensor may require a calibration to fine-tune its sensitivity. 

Installation Instructions:

Wiring: Follow the circuit diagram above to correctly connect the components.
Upload the Code: Open the Arduino IDE, copy and paste the code above into the editor, and upload it to your Arduino board.
Test the System: After uploading the code, power on the system. The system will begin monitoring for fire and smoke. Try using a lighter (for flame detection) or smoke (for the smoke sensor) to test the system’sresponse.

Troubleshooting:

Sensor not detecting correctly: Ensure that the sensors are connected properly and that the sensor's output is within the expected range.
False alarms: The MQ-2 sensor might give false readings due to humidity, temperature, or the presence of other gases. Adjust the threshold or calibrate the sensor accordingly.
Buzzer and LED not turning on: Verify that the Arduino pins and the components (buzzer and LED) are wired correctly. Check for correct power supply.

Contributing:

Feel free to fork this repository, submit issues, or send pull requests if you have any suggestions or improvements.



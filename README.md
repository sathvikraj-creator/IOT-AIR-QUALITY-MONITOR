# IOT-AIR-QUALITY-MONITOR

COMPANY: CODTECH IT SOLUTIONS

NAME: AKEPOGU SATHVIK RAJ

INTERN ID: CT04DH122

DOMAIN: INTERNET OF THINGS

DURATION: 4 WEEKS

MENTOR: NEELA SANTOSH

# DESCRIPTION

This project demonstrates an Air Quality Monitoring System developed using Arduino UNO to detect air pollutants such as CO₂ and PM2.5 using gas sensors or simulated analog inputs and alert using an LED and buzzer. As real sensors and Wi-Fi modules are not supported in the Tinkercad platform, potentiometers and the Serial Monitor are simulated to provide various concentrations of pollutants and a cloud dashboard, respectively.
The primary goal is to track indoor air quality and warn of hazardous levels of gases or particles. The system utilizes MQ135 (or its simulator equivalent) to sense air pollutants like carbon dioxide, ammonia, alcohol, benzene, and smoke. Another potentiometer as a PM2.5 sensor is utilized to sense fine particles of dust in the air. When the levels of pollutants cross the threshold set, an LED glows and a buzzer makes a sound as an indication of bad air quality.
The project offers an easy-to-use prototype for application in homes, offices, schools, and intelligent cities where there is a need for ongoing air quality monitoring for safety and health. This can further be expanded in actual hardware with IoT platforms such as ThingSpeak, Blynk, or Firebase to upload data to the cloud.

Components Used:
1. Arduino UNO – Central microcontroller unit which receives sensor inputs and drives outputs.
2. MQ135 Gas Sensor (simulated) – To detect CO₂ and other harmful gases.
3. LED – Serves as a visual cue if there is poor air quality.
4. Buzzer – Rings at dangerous levels of pollution.
5. Resistor – Used on LED to prevent high current.
6. Jumper Wires & Breadboard – To build and connect circuits.
7. Tinkercad Serial Monitor – Mimics the cloud dashboard to display real-time data.

Working Principle:
• Potentiometer and the gas sensor generate analog signals depending on the air quality.
• Arduino reads the values through analog input pins (A0 and A1).
• The system is always observing these values and checking them against a threshold (i.e., 400).
• Because the value of CO₂ or PM2.5 exceeds 400, air quality is bad.
• Next, the buzzer and LED are turned on by the Arduino as alarm signals.
• Otherwise, the system is in a normal mode (no warning).


Overview of the code :
The Arduino code begins with sensor and output pin declarations. During setup() function, the system initializes serial communication, as well as the pin modes for the buzzer and LED.
In loop(), Arduino samples analog values from the MQ135 sensor and potentiometer. Both values are printed to the Serial Monitor and checked if either is above a specific high value. If yes, the LED and buzzer are turned on; if not, they are turned off. delay(1000) ensures the loop runs every second.
This straightforward logic is the basis of the air quality alert system.


Applications:
• Indoor air quality monitoring in residences and workplaces 
• Intelligent buildings and building automation systems
• Environmental education and demonstration projects 
• Prototyping of IoT-based health monitoring device


# OUTPUT 


  # Pet Feeding System (IoT + Arduino)


#Project Title : Pet Feeding System using Arduino, Ultrasonic Sensor & Servo Motor

#Project Overview:  

This project is an automated pet-feeding system designed using Arduino. It detects when a pet approaches the food bowl using an ultrasonic sensor and then automatically releases food through a servo-operated flap.
The system ensures pets get food at the correct time without human intervention, making it useful for pet owners who are often away from home.

#Objectives 

1) Detect the presence of a pet near the feeding area.

2) Automatically open the food dispenser using a servo motor.

3) Provide a simple, low-cost, and efficient IoT-based solution for pet feeding.


#How It Works 

1) The Ultrasonic Sensor (HC-SR04) continuously measures the distance in front of the dispenser.

2) When the pet comes within 30 cm, the system considers it as a feeding request.

3) The Servo Motor rotates from 0° to 180° to open the food outlet.

4) After dispensing, the servo rotates back to 0° to close the outlet.

5) The system resets and waits for the next feeding detection.


#Key Components 

Arduino Uno / Nano – Main controller

Ultrasonic Sensor (HC-SR04) – Detects pet proximity

Servo Motor (SG90 / MG995) – Controls the food flap

Power Supply

Food Container + Mechanical Setup


#Features

Automatic food dispensing

Simple and cost-effective

Hands-free operation

Works even when the owner is away

Can be upgraded with IoT features (Blynk, WiFi module, scheduling)


#Code Explanation 

📡Ultrasonic Sensor

Sends a sound wave using trigPin

Measures how long it takes to bounce back at echoPin

Converts time → distance in cm

🤖 Servo Motor

When distance < 30 cm:

Servo rotates from 0° → 180° (opening the dispenser)

Then moves back 180° → 0° (closing the dispenser)

🕒 Delay

A short delay is added to prevent repeated triggering.



#Conclusion 

This project successfully automates the pet-feeding process using basic Arduino components.
It demonstrates sensor integration, servo control, and practical IoT automation concepts suitable for academic submissions, IoT portfolios, and GitHub showcases.



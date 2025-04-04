1. Introduction
1.1 Background
The mobility and independence of visually impaired individuals are often significantly hindered by their inability to detect and navigate around obstacles in their environment. Traditional aids like canes and guide dogs, while helpful, have limitations and can be cumbersome. The Ultrawalk is a Smart Ultrasonic Shoe that aims to address these challenges by leveraging modern technology to provide real-time feedback about the user's surroundings, thereby enhancing safety and independence.
1.2 Objective
The primary objective of this project is to develop a smart shoe that enhances the mobility and independence of blind and visually impaired individuals. The shoe will use advanced sensors and feedback systems to detect obstacles and provide real-time feedback to the user.


2. System Overview
2.1 Key Components
The Smart Ultrasonic Shoe consists of the following key components:
Arduino Uno Microcontroller: Acts as the central processing unit, interfacing with the sensor and feedback systems.
Ultrasonic Sensor (HC-SR04): Detects obstacles by emitting ultrasonic waves and measuring the time it takes for the waves to bounce back from an object.
Buzzer: Provides audible alerts to the user when an obstacle is detected within a predefined range.
HC-05 Bluetooth Module: Transmits data regarding the distance of the obstacle to the user's mobile phone, where it can be converted into speech.
9V Battery: Acts as the power source to the circuit
Switch: To switch the model on and off as and when required by the user.
2.2 Functionality
The system works as follows:
The ultrasonic sensor continuously scans for obstacles.
When an obstacle is detected, the distance is calculated and sent to the Arduino Uno.
If the obstacle is within 50 cm, the Arduino activates the buzzer to alert the user.
The distance data is also sent via Bluetooth to the user's mobile phone.
A mobile application, TalkBack, which is a part of Google’s Android Accessibility Service is used to convert the distance data into speech, providing verbal feedback to the user.

# Fall Detection & Alert - Android/iOS Application using Fuzzy Logic

This repository contains the source code for a child safety monitoring app designed for Android/iOS with Fuzzy Login. The app uses the phone's embedded hardware sensors such as GPS, accelerometer, and gyroscope to monitor a child's safety while they are riding a bicycle.

## Features
The App:
1. Monitor the accelerometer data of your phone when the App is ON and detect if there is a fall.
2. If there is a fall, automatically switch ON the microphone of the phone and measure the sound level. 
3. Using the fuzzy sound levels (Low, Medium, High), and fuzzy accelerometer levels (Low, Medium, High), estimate the level of danger (Low, Medium, High).
4. If the level of danger is High, send an alert to another phone (using TCP/IP or UDP network), transmitting the sound which was recorded in Step 2 and the GPS location of the first phone.
5. Play a buzzer sound (alarm type) in the first phone, if the danger levels are Medium or High, with the sound level of the buzzer sound proportional to the danger level.

## Files

- `ChildsPhone_fuzzyLogic.slx`: This file contains the Simulink model for the child's phone (Phone A).

- `ParentsPhone_fuzzyLogic.slx`: This file contains the Simulink model for the parent's phone (Phone B).
  
- `mamdanitype1.fis`: This file contains the fuzzy logic rules for detecting falls and triggering appropriate actions in the Fall Detection & Alert app.

## Demonstration

A demonstration of the app can be found in this [YouTube video](https://youtu.be/s_ilU70S1YA?si=2YZy3iI7Fx6jQSOC).

## Tools Used

- Simulink Support Package for Android Devices
- ThinkSpeak

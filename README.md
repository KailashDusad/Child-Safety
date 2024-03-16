# Child Safety Monitoring App

This repository contains the source code for a child safety monitoring app designed for Android/iOS. The app uses the phone's embedded hardware sensors such as GPS, accelerometer, and gyroscope to monitor a child's safety while they are riding a bicycle.

## Features

1. **Over Speed Detection**: The app continuously monitors the GPS and accelerometer data to detect if the bicycle is overspeeding.

2. **Fall Detection**: The app uses the gyroscope data to detect if the bicycle has fallen. It is designed to avoid false detections like bumps or braking.

3. **Boundary Crossing Detection**: The app uses the GPS data to detect if the bicycle has crossed a predefined geographical boundary.

4. **Alarm System**: If the bicycle overspeeds, falls, or crosses the boundary, the app plays a beep alarm sound on the child's device (Phone A) and displays the real-time location of Phone A on the parent's device (Phone B) using Google Maps. It also plays a beep sound on Phone B.

5. **Emergency SOS**: If the bicycle falls and the alarm is not switched off within 5 seconds, the app automatically switches on the microphone and camera of Phone A, starts recording, and sends an SOS from Phone A to Phone B by transmitting the recorded sound and images using the mobile internet network.

## Files

- `ChildsPhone.slx`: This file contains the Simulink model for the child's phone (Phone A).

- `ParentsPhone.slx`: This file contains the Simulink model for the parent's phone (Phone B).

## Demonstration

A demonstration of the app can be found in this [YouTube video](https://www.youtube.com/watch?v=yhH4HfYKkOg&authuser=0).

## Tools Used

- Simulink Support Package for Android Devices
- ThinkSpeak

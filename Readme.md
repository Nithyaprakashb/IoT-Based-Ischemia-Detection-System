# Smart Ischemia Detection System

## Overview

The Smart Ischemia Detection System is an IoT-based healthcare monitoring solution designed to detect potential ischemic conditions through real-time analysis of ECG, heart rate, and blood oxygen saturation (SpO₂) signals. The system integrates an AD8232 ECG sensor, MAX30102 pulse oximeter sensor, and ESP32 microcontroller with a Flutter-based Android application for wireless health monitoring.

## Features

* Real-time ECG monitoring
* Heart Rate (BPM) measurement
* Blood Oxygen Saturation (SpO₂) monitoring
* Wireless data transmission using ESP32
* Flutter-based Android application
* Portable and low-cost healthcare solution
* Early indication of cardiac abnormalities

## Hardware Components

* ESP32 Development Board
* AD8232 ECG Sensor
* MAX30102 Pulse Oximeter Sensor
* ECG Electrodes
* Jumper Wires
* Power Supply

## Software Stack

* Arduino IDE
* Flutter
* Dart
* ESP32 Libraries

## System Architecture

```text
AD8232 ECG Sensor
        │
MAX30102 Sensor
        │
        ▼
      ESP32
        │
        ▼
Flutter Android Application
        │
        ▼
Real-Time Health Monitoring
```

## Working Principle

The AD8232 sensor acquires ECG signals from the user, while the MAX30102 sensor measures heart rate and blood oxygen saturation levels. The ESP32 processes the acquired physiological signals and transmits them wirelessly to the Flutter mobile application. The application displays real-time health parameters and assists in identifying possible ischemic conditions.

## Results

* Successfully acquired ECG waveforms in real time
* Continuous monitoring of Heart Rate and SpO₂
* Wireless communication between ESP32 and Android application
* Real-time visualization of physiological parameters
* Portable healthcare monitoring system for cardiac assessment

## Project Demonstration

<img src="images/prototype.jpg" alt="Project Prototype" width="500">

## Future Enhancements

* AI-based ischemia prediction
* Cloud data storage and analytics
* Emergency alert notification system
* Doctor monitoring dashboard
* Patient health history management

## Applications

* Remote Patient Monitoring
* Cardiac Health Assessment
* Telemedicine Systems
* Biomedical Research
* Wearable Healthcare Solutions

## Author

**Nithya Prakash B**

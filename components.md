# Components Used

## Hardware Components

| Component                      | Quantity | Description                                                                                          |
| ------------------------------ | -------- | ---------------------------------------------------------------------------------------------------- |
| ESP32 Development Board        | 1        | Main microcontroller responsible for sensor interfacing, data processing, and wireless communication |
| AD8232 ECG Sensor              | 1        | Acquires ECG signals for monitoring cardiac electrical activity                                      |
| MAX30102 Pulse Oximeter Sensor | 1        | Measures heart rate and blood oxygen saturation (SpO₂)                                               |
| ECG Electrodes                 | 3        | Collect bioelectrical signals from the human body                                                    |
| TP4056 Charging Module         | 1        | Provides Li-Po battery charging and protection                                                       |
| Li-Po Battery                  | 1        | Portable power source for the system                                                                 |
| LM2596 Buck Converter          | 1        | Regulates voltage supplied to sensors and electronic modules                                         |
| Connecting Wires               | Multiple | Used for electrical connections between components                                                   |

## Sensor Specifications

### AD8232 ECG Sensor

* Single-lead ECG monitoring
* Analog output
* Low power consumption
* Suitable for portable biomedical devices

### MAX30102 Pulse Oximeter Sensor

* Heart Rate Monitoring
* Blood Oxygen Saturation (SpO₂) Measurement
* I2C Communication Interface
* Low-power operation

## Power Management

The system is powered by a rechargeable Li-Po battery through a TP4056 charging module. An LM2596 buck converter is used to provide stable regulated voltage to the sensors and ESP32, ensuring reliable operation during continuous monitoring.

## Total Components

* 1 × ESP32
* 1 × AD8232 ECG Sensor
* 1 × MAX30102 Sensor
* 3 × ECG Electrodes
* 1 × TP4056 Charging Module
* 1 × Li-Po Battery
* 1 × LM2596 Buck Converter
* Connecting Wires

# Software Used

| Software / Tool      | Purpose                                                         |
| -------------------- | --------------------------------------------------------------- |
| Arduino IDE          | Programming and uploading firmware to the ESP32 microcontroller |
| Flutter              | Development of the Android mobile application                   |
| Dart                 | Programming language used for Flutter application development   |
| ESP32 Board Package  | Enables ESP32 support in Arduino IDE                            |
| MAX30102 Library     | Acquisition and processing of heart rate and SpO₂ data          |
| AD8232 ECG Interface | ECG signal acquisition and monitoring                           |
| Serial Monitor       | Real-time debugging and sensor data visualization               |
| Android Studio       | Building, testing, and deploying the Flutter application        |
| GitHub               | Version control and project documentation                       |
| Firebase (Optional)  | Cloud storage and real-time database integration                |

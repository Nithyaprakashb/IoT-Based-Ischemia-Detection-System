# Circuit Diagram

## Connection Overview

The Smart Ischemia Detection System consists of an ESP32 microcontroller interfaced with an AD8232 ECG sensor and a MAX30102 pulse oximeter sensor. The system is powered using a Li-Po battery and TP4056 charging module. An LM2596 buck converter provides regulated voltage to the sensors, while the ESP32 is powered separately through USB.

## Power Connections

### ESP32

* Powered through USB connection

### LM2596 Buck Converter

* Input: Li-Po Battery / TP4056 Output
* Output: Regulated voltage supply for sensors

### MAX30102 Sensor

| MAX30102 Pin | Connection    |
| ------------ | ------------- |
| VCC          | LM2596 Output |
| GND          | Common Ground |
| SDA          | ESP32 SDA     |
| SCL          | ESP32 SCL     |

### AD8232 ECG Sensor

| AD8232 Pin | Connection           |
| ---------- | -------------------- |
| 3.3V       | LM2596 Output        |
| GND        | Common Ground        |
| OUTPUT     | ESP32 Analog Input   |
| LO+        | Optional Digital Pin |
| LO-        | Optional Digital Pin |

### ECG Electrodes

* RA → Right Arm
* LA → Left Arm
* RL → Right Leg (Reference)

## Block Diagram

```text
Li-Po Battery
      │
      ▼
   TP4056
      │
      ▼
 LM2596 Buck Converter
      │
 ┌────┴───────────┐
 │                │
 ▼                ▼
MAX30102      AD8232
 │                │
 └──────┬─────────┘
        │
        ▼
      ESP32
 (Powered via USB)
        │
        ▼
 Flutter Android App
```

## Notes

* All modules must share a common ground.
* The LM2596 provides a stable supply voltage for biomedical sensors.
* The ESP32 collects sensor data and transmits it wirelessly to the Flutter application.
* ECG electrodes should be placed correctly to obtain clean cardiac signals.

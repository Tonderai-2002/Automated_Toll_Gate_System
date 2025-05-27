# 🚧 Automatic Toll Gate System with Arduino

A simple Arduino-based automatic toll gate system that uses an ultrasonic sensor to detect approaching vehicles and operates a servo motor to raise and lower the gate.

## 📦 Features

- Vehicle detection using ultrasonic sensor (HC-SR04)
- Automatic gate control using servo motor
- Real-time distance feedback via Serial Monitor
- Contactless operation

## 🛠 Hardware Required

- Arduino Uno
- Ultrasonic Sensor (HC-SR04)
- Servo Motor (e.g., SG90)
- Jumper Wires
- Breadboard (optional)
- Power supply (USB or battery pack)

## 🔌 Circuit Connections

| Component         | Arduino Pin |
|-------------------|-------------|
| Ultrasonic Trig   | D3          |
| Ultrasonic Echo   | D5          |
| Servo Signal      | D9          |
| Ultrasonic VCC    | 5V          |
| Ultrasonic GND    | GND         |
| Servo VCC         | 5V          |
| Servo GND         | GND         |

> ⚠️ **Note:** Ensure the servo motor power supply can handle current draw. Consider external power if needed.

## 🧠 How It Works

The ultrasonic sensor continuously monitors the area in front of the toll gate. When a vehicle is detected within a 10 cm range, the servo motor rotates to lift the gate (90°). Once the vehicle passes and the distance increases, the servo returns to 0°, lowering the gate.



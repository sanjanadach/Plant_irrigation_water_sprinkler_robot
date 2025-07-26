## 🌱 Plant Irrigation Water Sprinkler Robot 🚜

This project implements a Remote-Controlled Smart Irrigation System using Arduino, designed to monitor and control soil moisture levels, water pumps, and environmental sensors for optimized irrigation.

## 🚀 Project Overview:

Goal: To create a smart system that automates irrigation based on real-time soil moisture and proximity sensing. It allows remote monitoring and control using the RemoteXY app interface.

## Features:

->Soil Moisture Sensor to monitor soil water levels.

->Ultrasonic Sensor for obstacle detection.

->IR Proximity Sensor for edge detection.

->Two Servo Motors for directional control.

->DC Pump and Motor control for irrigation.

->RemoteXY mobile app integration for wireless control.

## 🛠 Hardware Components:

1)Arduino Uno

2)L293D Motor Driver (AFMotor library support)

3)DC Motor (Pump)

4)Servo Motors (2x)

5)Soil Moisture Sensor

6)Ultrasonic Sensor (HC-SR04)

8)IR Proximity Sensor

9)Bluetooth Module (for RemoteXY)

10)Power Supply (Battery Pack)

## 🌱 Working Principle:

1) Soil moisture sensor checks the water level in the soil.

2) Ultrasonic sensor detects obstacles near the irrigation area.

3) Based on sensor readings:

->The pump starts/stops automatically.

->Servo motors adjust direction for water flow.

4) All data and controls are synced to the RemoteXY mobile app for real-time operation.

## ⚙️ Libraries Used:

RemoteXY

AFMotor

Servo

## 📊 Real-Time Feedback:

->Soil Moisture Levels: Displayed in percentage.

->Tank Level LEDs:

->Blue: High water level

->Green: Normal water level

->Red: Low water level



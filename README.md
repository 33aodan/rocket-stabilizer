# 2-Axis Thrust Vector Control Prototype

## Overview

This project is a small 2-axis thrust vector control (TVC) learning prototype and eventually use it to fly an altitude controlled model rocket.

The goal is to design, build, and test a bench-top stabilization system using:

- ESP32-S3
- MPU6050 IMU
- Two SG90 micro servos
- 3D-printed 2-axis gimbal
- Arduino / C++
- Complementary filtering
- Feedback control

The purpose of the project is to learn embedded systems, sensor processing, control systems, electronics, and mechanical design.

This project is currently intended as a bench-top demonstrator.

---

## System Architecture

The current system consists of:

```text
MPU6050
   |
   | I2C
   v
ESP32-S3
   |
   | Servo commands
   |
   +----> Pitch Servo
   |
   +----> Roll Servo
              |
              v
        2-Axis TVC Gimbal

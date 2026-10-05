# Hardware
## Current Components
- ESP32-S3 development board
- MPU6050 IMU
- 2x SG90 micro servos
- BPS.Space-inspired 3D-printed TVC gimbal
- Breadboard
- Jumper wires
- Regulated 5 V servo power supply
- USB cable
- Screws / servo hardware

# Wiring
|MPU6050|ESP32-S3|
| --- | --- |
|VCC|3.3 V|
|GND|GND|
|SDA|GPIO 8|
|SCL|GPIO 9|

# Servos
|Device|Connection|
| --- | --- |
|Pitch servo signal|GPIO 4|
|Roll servo signal|GPIO 5|
|Servo power|External regulated 5 V|
|Servo ground|Common ground|


The ESP32, MPU6050, servo supply, and servos all share a common ground.

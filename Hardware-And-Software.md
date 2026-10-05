# Hardware
## Current Components
- ESP32-S3 development board
- MPU6050 IMU
- 2x SG90 micro servos
- BPS.Space 3D-printed TVC gimbal
- Breadboard
- Jumper wires
- Regulated 5 V servo power supply
- USB cable
- Screws / servo hardware

## Wiring
|MPU6050|ESP32-S3|
| --- | --- |
|VCC|3.3 V|
|GND|GND|
|SDA|GPIO 8|
|SCL|GPIO 9|

## Servos
|Device|Connection|
| --- | --- |
|Pitch servo signal|GPIO 4|
|Roll servo signal|GPIO 5|
|Servo power|External regulated 5 V|
|Servo ground|Common ground|

# Software
The ESP32 is programmed using the Arduino IDE.
Libraries currently used:
- Wire
- MPU6050
- ESP32Servo

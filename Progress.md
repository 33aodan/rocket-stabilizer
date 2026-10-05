# TVC Project Version Progress

## V0 - Understand the System Architecture
- [x] Understand what thrust vector control does
- [x] Identify the main system components
- [x] Understand pitch and roll axes
- [x] Understand the basic feedback loop
- [x] Choose ESP32-S3, MPU6050, and two SG90 servos

## V1 - Electronics and Hardware Integration
- [x] Set up ESP32-S3 in Arduino IDE
- [x] Verify serial communication
- [x] Connect MPU6050 using I2C
- [x] Detect MPU6050 at I2C address `0x68`
- [x] Read raw accelerometer data
- [x] Read raw gyroscope data
- [x] Test one SG90 servo
- [x] Test two SG90 servos
- [x] Run MPU6050 and both servos together

## V2 - IMU Measurement and Filtering
- [x] Convert accelerometer readings to `g`
- [x] Convert gyro readings to `deg/s`
- [x] Measure gyroscope bias
- [x] Implement automatic gyro calibration
- [x] Calculate pitch from accelerometer data
- [x] Calculate roll from accelerometer data
- [x] Test pitch and roll by manually tilting the IMU
- [x] Understand gyro drift and accelerometer noise
- [x] Implement a complementary filter
- [x] Obtain stable filtered pitch and roll values

## V3 - Servo Control From Orientation
- [x] Command one servo from measured pitch
- [x] Calculate orientation error
- [x] Implement basic proportional control
- [x] Test proportional servo response
- [x] Add second servo
- [x] Control pitch and roll servos independently
- [x] Verify both servo directions are correct

## V4 - 2-Axis Gimbal
- [x] Obtain/print 2-axis TVC gimbal
- [x] Install both SG90 servos
- [x] Assemble servo horns and linkages
- [x] Verify the gimbal moves in both axes
- [ ] Center the mechanism precisely at `90°`
- [ ] Determine safe servo travel limits
- [ ] Check for mechanical interference
- [ ] Check for linkage flex or binding

## V5 - Complete Bench Prototype
- [ ] Mount MPU6050 rigidly to the prototype body
- [ ] Mount ESP32 and electronics securely
- [ ] Organize wiring
- [ ] Verify common ground and servo power setup
- [ ] Test pitch axis through the physical gimbal
- [ ] Test roll axis through the physical gimbal
- [ ] Establish safe software servo limits
- [ ] Verify repeatable movement

## V6 - Closed-Loop Stabilization
- [ ] Create a controlled bench-test setup
- [ ] Tune pitch proportional gain `Kp`
- [ ] Tune roll proportional gain `Kp`
- [ ] Observe overshoot
- [ ] Observe oscillation
- [ ] Measure settling behavior
- [ ] Understand the effect of sampling rate
- [ ] Understand control-loop latency
- [ ] Add derivative control if necessary
- [ ] Add integral control only if necessary
- [ ] Compare P, PD, and PID control
- [ ] Achieve stable 2-axis bench stabilization

## V7 - Testing, Data, and Documentation
- [ ] Log pitch and roll data
- [ ] Log servo commands
- [ ] Record timestamps
- [ ] Plot system response using Python
- [ ] Measure settling time
- [ ] Measure overshoot
- [ ] Compare different controller gains
- [ ] Document final wiring
- [ ] Document final code
- [ ] Document final mechanical design
- [ ] Record demonstration video
- [ ] Write final project summary
- [ ] Write portfolio/resume description

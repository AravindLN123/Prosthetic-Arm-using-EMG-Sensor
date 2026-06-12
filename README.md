Prosthetic Arm using EMG Sensor


B.E. Mini Project — Electronics and Communication Engineering

Sri Venkateswara College of Engineering, Anna University | December 2022

Team: Aditya U Tawker, Aravind LN




Overview

An EMG-controlled prosthetic hand that opens and closes fingers based on forearm muscle signals. Surface electrodes detect contractions, an Arduino Mega processes the signal against pre-trained voltage ranges, and servo motors actuate each finger. Force sensors at each fingertip provide vibration feedback to the user.


How It Works


Signal Detection: Three surface electrodes are placed on the forearm: two across the muscle and one on the bone as ground.
Signal Processing: A differential amplifier subtracts noise, followed by pre-amplification, low-pass and high-pass filtering, and a final amplification stage to make the signal readable by the Arduino.

Control Logic :The Arduino Mega continuously checks each analog pin and compares the incoming signal against a pre-trained voltage range for each finger. If the signal falls within range, the corresponding servo motor is activated.

Finger Actuation : Servo motors rotate 0–180° to open or close each finger based on the muscle contraction state.
Haptic Feedback : Force sensors at each fingertip detect contact and trigger vibration motors on the amputee's arm to signal touch.

Components:

ComponentPurposeEMG SensorReads electrical activity from musclesSurface ElectrodesDetect muscle signals non-invasivelyArduino MegaProcesses EMG data and controls motorsServo MotorsActuate finger open/close movementForce SensorsDetect fingertip contactVibration MotorsProvide haptic feedback to the user


Software:


IDE: Arduino IDE
Language: Arduino C (based on Wiring)



Project Goals:


Build a cost-effective prosthetic hand affordable for most amputees
Achieve reliable finger control using surface EMG signals
Provide sensory feedback without invasive methods



Limitations & Future Work:


Feedback is limited to fingertips; future versions could use an artificial skin layer for full-hand sensing
Additional sensory properties (temperature, texture, object size) could be incorporated for broader accessibility
EMG training data was collected from a non-amputee, which partially limits real-world accuracy



Acknowledgements

Guided by Dr. G.A. Sathish Kumar, Professor, Dept. of ECE

Sri Venkateswara College of Engineering, Chennai

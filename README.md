# AI Based Insigtht vibrator glove for visually and auditory challenged people
## Problem Statement
The proposed AI-based insight vibrator glove aims to assist visually and auditory challenged individuals by providing real-time feedback through vibration.
This glove will help users navigate their environment and alert them to potential obstacles and important insights derived from data,
such as customer satisfaction and delays in airline services.
The glove will use advanced technologies including computer vision, machine learning, and haptic feedback to convey information.

Step 1: Capturing Obstacle Data
Hardware Components:

ESP32 Camera Module: This will capture real-time images of the surroundings.
Ultrasonic Sensors: These will detect obstacles within a certain range and provide distance measurements.
Software Components:

Python for Image Processing: Using Python libraries to handle image capture and preprocessing.
C/C++ for Sensor Data Processing: Writing firmware for the ESP32 to process ultrasonic sensor data and control the camera module.
Step 2: Object Detection using YOLOv3
Setting up YOLOv3:

Pre-trained YOLOv3 Model: Use a pre-trained YOLOv3 model for obstacle detection. YOLOv3 is efficient for real-time object detection.
Python Integration: Use OpenCV and TensorFlow/Keras to run the YOLOv3 model on captured images to detect objects.
Steps:

Capture images using the ESP32 camera.
Send images to a processing unit (e.g., a Raspberry Pi or a computer).
Run the YOLOv3 model on the processing unit to detect objects.
Identify the names of detected objects.
Step 3: Alert Mechanisms
Text-to-Speech Conversion:

Python Libraries: Use libraries like gTTS (Google Text-to-Speech) to convert detected object names into speech.
Speaker Integration: Connect a small speaker to the processing unit to output the speech.
Vibration Alerts:

Vibration Motor: Integrate a small vibration motor controlled by the ESP32.
Alert Triggers: Based on the distance data from the ultrasonic sensors, trigger the vibration motor to alert users of nearby obstacles.
Step 4: Combining Data for User Alerts
Integrating All Components:

Real-time Processing: Continuously capture images and sensor data.
Object Detection and Distance Measurement: Use YOLOv3 to detect objects and ultrasonic sensors to measure their distance.
Alert System:
For visually challenged users: Provide audio alerts naming the detected objects.
For auditory challenged users: Use vibration patterns to indicate the presence and distance of obstacles.

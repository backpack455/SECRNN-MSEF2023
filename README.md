Gunshot Detection Alarm Device



Overview

This project aims to improve law enforcement reaction time by developing a gunshot detection alarm device using a Raspberry Pi. The device utilizes advanced sound detection algorithms to identify gunshots and send real-time alerts to law enforcement agencies.

Features

Real-Time Detection: Continuously monitors ambient sounds and detects gunshots with high accuracy.
Instant Alerts: Sends immediate alerts to predefined contacts or law enforcement agencies upon detecting a gunshot.
Portable and Scalable: Built using a Raspberry Pi, the device is highly portable and can be deployed in multiple locations.
Open Source: All code and schematics are open-source, allowing for community contributions and improvements.
Project Documentation

Project Report
Presentation 1
Presentation 2
YouTube Video Demo
Components

Raspberry Pi: The core computing unit of the device.
Microphone: Captures ambient sounds for analysis.
Sound Processing Software: Analyzes audio input to detect gunshots.
Alert System: Sends notifications via email, SMS, or other communication methods.
Setup Instructions

Hardware Assembly:

Connect the microphone to the Raspberry Pi.
Ensure all components are securely attached.
Software Installation:

Install necessary libraries and dependencies:
sh
Copy code
sudo apt-get update
sudo apt-get install python3-pip
pip3 install pyaudio numpy scipy
Clone the repository:
sh
Copy code
git clone https://github.com/yourusername/gunshot-detection-alarm.git
cd gunshot-detection-alarm
Configuration:

Configure the alert system by setting up your preferred notification method (email, SMS, etc.).
Running the Device:

Start the gunshot detection program:
sh
Copy code
python3 detect_gunshot.py
How It Works

The device captures ambient sounds through the microphone, processes the audio signals using advanced algorithms, and identifies gunshot patterns. Upon detection, the device triggers an alert system to notify law enforcement or predefined contacts, providing them with real-time information.

Contributing

Contributions are welcome! Please fork the repository and submit pull requests to contribute to the project.

License

This project is licensed under the MIT License.

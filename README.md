# Gunshot Detection Alarm Device

![Project Demo](https://youtu.be/Q8h_Qf6KS74)

## Overview

This project aims to improve law enforcement reaction time by developing a gunshot detection alarm device using a Raspberry Pi. The device utilizes advanced sound detection algorithms to identify gunshots and send real-time alerts to law enforcement agencies.

## Features

- **Real-Time Detection**: Continuously monitors ambient sounds and detects gunshots with high accuracy.
- **Instant Alerts**: Sends immediate alerts to predefined contacts or law enforcement agencies upon detecting a gunshot.
- **Portable and Scalable**: Built using a Raspberry Pi, the device is highly portable and can be deployed in multiple locations.
- **Open Source**: All code and schematics are open-source, allowing for community contributions and improvements.

## Project Documentation

- [Project Report](https://docs.google.com/document/d/1PLTL0GT4mDv7MRuZTo727VBNo3oW_VWpe3a4USZLz04/edit?usp=sharing)
- [Presentation 1](https://docs.google.com/presentation/d/1m6s5ke25lyPTwZDbIXAbxjvut6nWUf-m3mejdVA5OSM/edit?usp=sharing)
- [Presentation 2](https://docs.google.com/presentation/d/1Q3NYl_UWfafFcsRuGGvbzul4kimvUd6Kqr9Yn3JhsOM/edit?usp=sharing)
- [YouTube Video Demo](https://youtu.be/Q8h_Qf6KS74)

## Components

- **Raspberry Pi**: The core computing unit of the device.
- **Microphone**: Captures ambient sounds for analysis.
- **Sound Processing Software**: Analyzes audio input to detect gunshots.
- **Alert System**: Sends notifications via email, SMS, or other communication methods.

## Setup Instructions

1. **Hardware Assembly**:
    - Connect the microphone to the Raspberry Pi.
    - Ensure all components are securely attached.

2. **Software Installation**:
    - Install necessary libraries and dependencies:
      ```sh
      sudo apt-get update
      sudo apt-get install python3-pip
      pip3 install pyaudio numpy scipy
      ```
    - Clone the repository:
      ```sh
      git clone https://github.com/yourusername/gunshot-detection-alarm.git
      cd gunshot-detection-alarm
      ```

3. **Configuration**:
    - Configure the alert system by setting up your preferred notification method (email, SMS, etc.).

4. **Running the Device**:
    - Start the gunshot detection program:
      ```sh
      python3 detect_gunshot.py
      ```

## How It Works

The device captures ambient sounds through the microphone, processes the audio signals using advanced algorithms, and identifies gunshot patterns. Upon detection, the device triggers an alert system to notify law enforcement or predefined contacts, providing them with real-time information.

## Contributing

Contributions are welcome! Please fork the repository and submit pull requests to contribute to the project.

## License

This project is licensed under the MIT License.

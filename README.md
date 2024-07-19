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

The device captures ambient sounds through the microphone and processes the audio signals using advanced algorithms to identify gunshot patterns. The key components of the sound processing include:

1. **Preprocessing**: The audio signal is first preprocessed to remove background noise and normalize the sound levels. This involves using filters such as the Butterworth filter for noise reduction.

2. **Feature Extraction**: Specific features indicative of gunshots are extracted from the audio signal. This includes the detection of sharp amplitude peaks and specific frequency patterns associated with gunshots.

3. **Classification**: The extracted features are fed into a machine learning classifier trained to distinguish gunshots from other sounds. Algorithms such as Support Vector Machines (SVM) and Convolutional Neural Networks (CNN) are employed to achieve high accuracy in gunshot detection.

4. **Alert System**: Once a gunshot is detected, the device triggers an alert system that sends notifications via email, SMS, or other communication methods to notify law enforcement or predefined contacts.

## Algorithm Details

### Preprocessing

- **Noise Reduction**: The Butterworth filter is applied to reduce ambient noise.
- **Normalization**: The audio signal is normalized to ensure consistent detection performance.

### Feature Extraction

- **Amplitude Peaks**: Detects sharp peaks in the audio signal's amplitude that are characteristic of gunshots.
- **Frequency Patterns**: Analyzes specific frequency ranges that are typically associated with gunshot sounds.

### Classification

- **Support Vector Machines (SVM)**: A machine learning model trained to classify gunshot sounds based on the extracted features.
- **Convolutional Neural Networks (CNN)**: A deep learning model that processes the audio signal's spectrogram to identify gunshot patterns with high accuracy.

## Contributing

Contributions are welcome! Please fork the repository and submit pull requests to contribute to the project.

## License

This project is licensed under the MIT License.

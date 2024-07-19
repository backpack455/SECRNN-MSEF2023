# Gunshot Detection Alarm Device

[![Project Demo](https://img.youtube.com/vi/Q8h_Qf6KS74/0.jpg)](https://youtu.be/Q8h_Qf6KS74)

## Overview

This project aims to improve law enforcement reaction time by developing a gunshot detection alarm device using a Raspberry Pi. The device utilizes the advanced SECRNN (Convolutional Recurrent Neural Network) model to identify gunshots and send real-time alerts to law enforcement agencies.

## Features

- **Real-Time Detection**: Continuously monitors ambient sounds and detects gunshots with high accuracy.
- **Instant Alerts**: Sends immediate alerts to predefined contacts or law enforcement agencies upon detecting a gunshot.
- **Advanced Audio Processing**: Uses SECRNN to combine CNNs and RNNs for superior audio event recognition.
- **Portable and Scalable**: Built using a Raspberry Pi, the device is highly portable and can be deployed in multiple locations.
- **Open Source**: All code and schematics are open-source, allowing for community contributions and improvements.

## Project Documentation

- [Project Report](https://docs.google.com/document/d/1PLTL0GT4mDv7MRuZTo727VBNo3oW_VWpe3a4USZLz04/edit?usp=sharing)
- [Presentation 1](https://docs.google.com/presentation/d/1m6s5ke25lyPTwZDbIXAbxjvut6nWUf-m3mejdVA5OSM/edit?usp=sharing)
- [Presentation 2](https://docs.google.com/presentation/d/1Q3NYl_UWfafFcsRuGGvbzul4kimvUd6Kqr9Yn3JhsOM/edit?usp=sharing)
- [YouTube Video Demo](https://youtu.be/Q8h_Qf6KS74)
- [Project Diagram](https://drive.google.com/file/d/1S6NCUwfFN-hs7NGmLr_iRAUqCGLjYXcS/view?usp=sharing)

## Components

- **Raspberry Pi**: The core computing unit of the device.
- **Microphone**: Captures ambient sounds for analysis.
- **SECRNN Model**: Analyzes audio input to detect gunshots.
- **Alert System**: Sends notifications via email, SMS, or other communication methods.

## Visual Overview

![Device Overview](https://drive.google.com/uc?id=1S6NCUwfFN-hs7NGmLr_iRAUqCGLjYXcS)

## Setup Instructions

1. **Hardware Assembly**:
    - Connect the microphone to the Raspberry Pi.
    - Ensure all components are securely attached.

2. **Software Installation**:
    - Install necessary libraries and dependencies:
      ```sh
      sudo apt-get update
      sudo apt-get install python3-pip
      pip3 install pyaudio numpy scipy librosa
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

The device captures ambient sounds through the microphone and processes the audio signals using the SECRNN model to identify gunshot patterns. The key components of the SECRNN model include:

1. **Preprocessing**: Utilizes Short-term Fourier Transform (STFT) to remove background noise and normalize sound levels.
2. **Feature Extraction**: Employs CNNs to extract spatial features from spectrograms and RNNs to capture temporal features.
3. **Classification**: Uses SECRNN, which combines CNN and RNN architectures, for high-accuracy gunshot detection.
4. **Inverse Frequency Weighting (IFW)**: Addresses class imbalance to produce uniform results across all classes.

### SECRNN Model Details

The SECRNN model leverages both convolutional neural networks (CNNs) and recurrent neural networks (RNNs) to deliver superior accuracy, precision, recall, and F1 scores. Key innovations include:

- **Short-term Fourier Transform (STFT)**: Used without Mel Scale spectrograms to retain high-signal acoustic features and reduce spectral leakage.
- **Inverse Frequency Weighting (IFW)**: Balances the model by addressing class imbalances without relying on data augmentation.
- **Convolutional Recurrent Neural Network (CRNN)**: Combines Conv2D layers and Long Short-Term Memory (LSTM) layers to extract both spatial and temporal features.

## Contributing

Contributions are welcome! Please fork the repository and submit pull requests to contribute to the project.

## License

This project is licensed under the MIT License.

## References

- [SECRNN: Convolutional Recurrent Network for Spatial Audio Event Recognition](https://docs.google.com/document/d/1PLTL0GT4mDv7MRuZTo727VBNo3oW_VWpe3a4USZLz04/edit?usp=sharing)
- [UrbanSounds8K Dataset](https://urbansounddataset.weebly.com/urbansound8k.html)

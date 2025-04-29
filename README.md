# Real-Time Sign Language to Speech Conversion on Edge Devices: A Jetson Nano Implementation 

This project is a real-time American Sign Language (ASL) fingerspelling recognition system. It focuses on recognizing alphabet gestures using deep learning techniques like spatio-temporal feature extraction and attention mechanisms.

Built with a custom dataset of 24 alphabet classes and a blank class, the model leverages MobileNetV2 for efficient feature extraction and real-time predictions.

<img src="https://github.com/user-attachments/assets/0b42c256-935b-4e67-8bbb-749a22443b04" alt="gui" width="600"/>

## Video Demo:
Link: [https://drive.google.com/file/d/1CP8VoFTIysbxXgW-vwRwSsdX5K60UDAe/view?usp=drive_link](https://drive.google.com/file/d/1CP8VoFTIysbxXgW-vwRwSsdX5K60UDAe/view?usp=drive_link)

## Model Details

* Base Model: MobileNetV2

* Input Shape: (32, 224, 224, 3)

* Output Shape: (32, 26)

* Classes: 25 (24 letters + 1 blank class)

* Loss Function: Categorical Crossentropy

* Optimizer: Adam

* Evaluation Metrics: Accuracy

## Setup Instructions

### 1. Clone the repository

```bash
git clone https://github.com/bh-g/Sign-Language-Recognition.git 
```

### 2. Create and activate a virtual environment (optional but recommended)

```bash
python -m venv venv
source venv/bin/activate  # for Mac/Linux
venv\Scripts\activate     # for Windows
```

### 3. Install the required dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the project

```bash
application.py
```

## Hardware Setup for NVIDIA Jetson Nano

<img src="https://github.com/user-attachments/assets/eb713d0b-199a-417f-b65c-cd70a6bcd818" alt="gui" width="600"/>

### 1. Jetson Nano Board

* Use a Jetson Nano Developer Kit.

* Insert a microSD card (at least 32GB, Class 10/UHS-1) flashed with JetPack (Jetson's Ubuntu-based OS).

### 2. Power Supply

* Recommended: 5V 4A DC Barrel Jack power supply.

* Alternate: 5V 2.5A micro-USB (only for lightweight tasks).

  `Important: Insufficient power may cause random reboots or throttling!`

### 3. Peripherals

* Keyboard and Mouse via USB.

* Monitor connected through HDMI or DisplayPort.

* Internet Connection:

  * Wired Ethernet is preferred (faster and more stable).

  * USB Wi-Fi adapter (make sure it’s compatible with Ubuntu 18.04/20.04).

* Audio Output (Speakers): USB Speakers (plug into USB port).

* Camera: USB Webcam (plug into USB port).


## Example Setup:

<img src="https://github.com/user-attachments/assets/d15ea0c6-ab1c-4eb9-bff4-2fd60587c0dc" alt="gui" width="400"/>

### Final Checklist Before Running
 
- Jetson Nano powered and booted up.

- Monitor, keyboard, mouse connected.

- Speakers connected and tested.

- Network (Ethernet or Wi-Fi) connected.

- Camera or other USB devices attached (if required).

- Software dependencies installed.

For detailed instructions, please refer to the official [Jetson Nano Developer Kit User Guide](https://developer.download.nvidia.com/embedded/L4T/r32-3-1_Release_v1.0/Jetson_Nano_Developer_Kit_User_Guide.pdf).

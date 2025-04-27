# Sign Language Recognition

This project is a real-time American Sign Language (ASL) fingerspelling recognition system. It focuses on recognizing alphabet gestures using deep learning techniques like spatio-temporal feature extraction and attention mechanisms.

Built with a custom dataset of 24 alphabet classes and a blank class, the model leverages MobileNetV2 for efficient feature extraction and real-time predictions.

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

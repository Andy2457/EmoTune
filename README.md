# EmoTune

EmoTune is a Python-based application for facial emotion recognition. Using computer vision and a trained deep learning model, EmoTune detects real-time facial emotions and displays the output interactively. This project leverages Flask for the web interface, OpenCV for image processing, and Keras for deep learning.

---

## Table of Contents

- [About](#about)
- [Features](#features)
- [Project Structure](#project-structure)
- [Setup Instructions](#setup-instructions)
- [Running the Project](#running-the-project)
- [Contact](#contact)

---

## About

EmoTune captures images/video from your webcam, runs facial detection, and uses a trained model to predict the emotion expressed on detected faces. The application provides a browser-based interface for real-time demonstration and result visualization.

---

## Features

- Real-time webcam image capture
- Facial detection with Haar cascades
- Emotion recognition using a deep learning model (`final_model.h5`)
- Web interface powered by Flask
- Easily update or retrain the model with provided scripts

---

## Project Structure


- `app.py` - Main Flask application
- `capture.py`, `display.py`, `model.py`, `Update_Model.py` - Supporting scripts for capturing images, displaying results, training/updating the model
- `final_model.h5` - Trained deep learning model for emotion recognition
- `haarcascade_frontalface_default.xml` - XML file for OpenCV face detection
- `templates/` - HTML templates for Flask
- `static/` - Static resources (images, CSS, JS)
- `README.md` - Project documentation

---

## Setup Instructions

### Prerequisites

- Python 3.7+
- pip (Python package installer)
- Webcam for live capture

### Install Dependencies

pip install flask opencv-python keras numpy


(You may also need `tensorflow` depending on your Keras version.)

---

## Running the Project

1. Clone the repository:
    ```
    git clone https://github.com/Andy2457/EmoTune.git
    cd EmoTune
    ```

2. Run the app:
    ```
    python app.py
    ```

3. Open your browser and go to `http://localhost:5000` to use the web interface.

---


## Contact

For questions, issues, or feature requests, please contact Aniket at aniketpawar2457@gmail.com or open an Issue in this repository.

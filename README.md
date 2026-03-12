#  Frudon - Fruit Shelf Life Predictor

> An AI-powered web application that predicts the remaining shelf life of fruits from images. It uses a custom-trained regression model on top of MobileNetV2 to estimate shelf life in days.

##  Features

- ** AI-Powered Prediction:** Upload a fruit image and get an instant shelf life estimate.
- ** Fruit Detection:** Automatically verifies if the uploaded image contains a fruit using a pre-trained MobileNetV2 model.
- ** Easy-to-Use Interface:** Simple and clean web interface for image upload.
- ** Custom Model:** Trained on a dataset of fruits (apple, banana, etc.) with varying shelf life stages.

##  Tech Stack

- **Backend:** Python, Flask, TensorFlow/Keras
- **Frontend:** HTML, CSS, JavaScript, Bootstrap
- **Model:** MobileNetV2 (Transfer Learning)
- **Others:** NumPy, Pillow, Flask-CORS

##  Project Structure

Fruidon-Shelf-Life-Predictor/
├── app.py # Main Flask application for the API and backend logic
├── train_model.py # Script used to train the fruit shelf life model
├── index.html # Frontend HTML file for the web interface
├── requirements.txt # (Optional but recommended) List of Python dependencies
└── README.md # This file


## ⚙️ Installation and Setup

Follow these steps to get the project running on your local machine.

### Prerequisites

*   Python 3.7+
*   pip (Python package installer)
*   Git (optional)

### Step-by-Step Guide

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/your-username/your-repo-name.git
    cd your-repo-name

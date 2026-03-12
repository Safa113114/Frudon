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

Option B: Direct Download

Click the green "Code" button on GitHub

Select "Download ZIP"

Extract the ZIP file

Open the folder in terminal/command prompt

2. **Create Virtual Environment** (Recommended)
   Windows:
    ```bash
     python -m venv venv
     venv\Scripts\activate

  Mac/Linux:
    ```bash
        python3 -m venv venv
        source venv/bin/activate

3. Install Dependencies
Create a file named requirements.txt with this content:

tensorflow==2.13.0
flask==2.3.3
flask-cors==4.0.0
numpy==1.24.3
pillow==10.0.0
werkzeug==2.3.7

Then install:
      
       pip install -r requirements.txt
       
4. Download the Model
 Important: The model file (fruit_shelf_life_model.h5) is too large for GitHub (>100MB).

Download from here: [Google Drive Link - Add your link here]

After downloading, place the .h5 file in the same folder as app.py.

5. Run the Application
Start the Flask server:
   ```bash
   python app.py
   You should see 
   * Running on http://127.0.0.1:5002


6. Open the Website
Open your web browser

Go to: http://127.0.0.1:5002

Or simply double-click the index.html file  

## How to Use
Click "Predict Shelf Life" button

Upload a fruit image (JPG, PNG, JPEG)

Wait for AI to analyze

Get instant shelf life prediction in days

 Screenshots
[Add screenshots here - very important for README]

Home Page	Prediction Result
[Add image]	[Add image]

## How it works
<img width="933" height="312" alt="image" src="https://github.com/user-attachments/assets/173a5a8f-e57f-476f-966d-261d8bf76565" />

Fruit Detection: Image goes through MobileNetV2 (ImageNet weights)

Validation: Checks if detected object is a fruit

Prediction: Custom-trained model estimates shelf life (0-14 days)

Result: Shows predicted days on screen

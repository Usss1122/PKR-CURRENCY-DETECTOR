Real or Fake PKR Currency Detector Using CNN

Project uses Deep Learning (CNN) to classify Pakistani currency notes as Real or Fake based on image inputs.
The system is deployed using Streamlit, Flask, and FastAPI, making it easy for users to upload an image and instantly receive a prediction.

Project Overview

Fake currency circulation is a major concern in Pakistan. Traditional manual detection methods are slow and error-prone.
This project builds an automated currency verification system using a Convolutional Neural Network (CNN) trained on images of real and fake PKR notes.

The model analyzes:

Texture
Color patterns
Watermark areas
Security features
Edge & print clarity
and predicts whether the uploaded note is Real or Fake.

Deep Learning Model

The CNN model was built using TensorFlow/Keras and includes:
Convolutional Layers
ReLU activation
MaxPooling Layers
Flatten Layer
Dense Fully Connected Layers
Sigmoid/Softmax Output Layer

Key Performance:
Accuracy: ~73%
Performs best on Real notes
Fake note detection improves with data augmentation

Project Structure

PKR-Currency-Detector/
│── currency_detection.ipynb        # Full training notebook
│── currency.h5                     # Trained CNN model
│── app_streamlit.py                # Streamlit deployment
│── app_flask.py                    # Flask deployment
│── main_fastapi.py                 # FastAPI deployment
│── requirements.txt                # Python dependencies
│── README.md                       # Project documentation
└── images/                         # Screenshots for UI and examples
Usage & Installation
Clone the Repository
git clone https://github.com/your-username/PKR-Currency-Detector.git
cd PKR-Currency-Detector

Install Dependencies

pip install -r requirements.txt

Run the Applications
Streamlit App

streamlit run app_streamlit.py

Flask App
python app_flask.py


Open in browser:
http://127.0.0.1:5000/

FastAPI
uvicorn main_fastapi:app --reload


API Documentation:
http://127.0.0.1:8000/docs

Model Evaluation

Metric	Score
Accuracy	~73%
Precision	Good
Recall	High for Real notes; Moderate for Fake notes
F1 Score	Balanced overall

The model performs well considering the limited dataset and can be improved by adding more images of fake notes.

Key Features

Upload an image of a PKR note
Automatic preprocessing
CNN-based classification
Displays prediction with confidence score
Works with multiple deployment frameworks
Easy to integrate into other applications

Future Enhancements

Add transfer learning (VGG16, ResNet, EfficientNet)
Build a mobile scanning application
Increase dataset size for fake notes
Online deployment (HuggingFace, Render, Railway)
Multi-denomination detection

Author

Uswa Shariq
BS Business Data Analytics
Resume Screening App

Overview

The Resume Screening App is a machine learning-based web application that automatically classifies resumes into job categories using natural language processing (NLP). The app allows users to upload resumes in PDF, DOCX, or TXT format and predicts the relevant job category. The frontend is built with Streamlit, while the backend leverages scikit-learn for machine learning.

Features

Upload resumes in PDF, DOCX, or TXT format

Extract and clean text using PyPDF2, python-docx, and regex

Preprocess and vectorize text using TF-IDF

Predict resume category using a machine learning model (SVM)

Display extracted text and predicted category

Simple and interactive UI built with Streamlit

Tech Stack

Python (NLP and Machine Learning)

Streamlit (Frontend)

scikit-learn (ML Model - SVM)

PyPDF2 & python-docx (Text Extraction)

Pickle (Model Serialization)

Installation & Setup

Prerequisites

Ensure you have Python 3.9+ installed.

Steps

Clone the repository:

git clone https://github.com/your-username/resume-screening-app.git
cd resume-screening-app

Create and activate a virtual environment:

python -m venv .venv
source .venv/bin/activate  # On macOS/Linux
.venv\Scripts\activate     # On Windows



Run the app:

streamlit run app.py

Folder Structure

resume-screening-app/
│── app.py                    # Main application script
│── clf.pkl                    # Trained SVM model
│── tfidf.pkl                  # TF-IDF vectorizer
│── encoder.pkl                # Label encoder for categories
│── UpdatedResumeDataSet.csv    # Dataset used for training
│── README.md                   # Project documentation

Usage

Open the Streamlit app in your browser after running streamlit run app.py.

Upload a resume in PDF, DOCX, or TXT format.

The app will extract text, process it, and predict the job category.

The predicted category will be displayed on the screen.

Model Training (Optional)

To retrain the model on a new dataset:

python train_model.py

Ensure train_model.py includes loading the dataset, preprocessing, training, and saving the model.

Contribution

Feel free to contribute by opening a pull request! If you find any issues, report them in the Issues section.


Author

Abdul Hadi

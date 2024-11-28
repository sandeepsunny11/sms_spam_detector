# sms_spam_detector

This assignment implements an SMS classification system that categorizes SMS messages as either "spam" or "ham" (not spam) using machine learning. The system is built with the following components:
1. Scikit-learn: Used for data preprocessing and classification.
2. Gradio: Provides an interactive user interface for live SMS classification.

# Features:
1. Classifies SMS messages as "spam" or "ham."
2. Uses a TF-IDF vectorizer to convert text into numerical vectors.
3. Employs a Linear Support Vector Classifier (LinearSVC) for binary classification.
4. Provides an interactive Gradio interface for live predictions.

# How It Works:
1. Loading the Data:
The dataset includes two columns: the SMS text and a label (spam or ham).
The data is split into training (67%) and testing (33%) sets.

2. Preprocessing and Model Creation:
The data is split into features (SMS text) and labels (spam/ham).
A machine learning pipeline is created:
TF-IDF Vectorization: Converts text into numerical vectors.
LinearSVC: Classifies the messages as spam or ham.
The model is trained on the training data.

3. Making Predictions:
The trained model predicts whether a new SMS is spam or not by passing the text through the pipeline.

4. Gradio User Interface:
The Gradio app provides a textbox for users to input SMS messages and displays the classification result (spam or ham) in real-time.
This setup enables users to interactively classify SMS messages and make predictions locally.

# speaking-skill-analyzer

This project is a Streamlit application designed to simulate the IELTS Speaking Test. The application allows users to participate in a mock speaking test, providing responses to various parts of the test and receiving feedback based on their performance.

#Features
Speech Recognition: Uses the speech_recognition library to capture and recognize user's speech.
IELTS Test Simulation: Includes all three parts of the IELTS Speaking Test - Introduction, Cue Card, and Follow-Up Questions.
Automated Evaluation: Evaluates the user's responses based on criteria such as fluency, vocabulary, grammar, and pronunciation.
Feedback: Provides an estimated IELTS band score and feedback for each part of the test.

#Requirements
Python 3.6 or higher
Streamlit
SpeechRecognition
NLTK

#Installation
Install the required packages:
pip install streamlit speechrecognition nltk

Download the required NLTK data:
import nltk
nltk.download('cmudict')
nltk.download('wordnet')
nltk.download('averaged_perceptron_tagger')

#Running the Application
To run the application, use the following command:
streamlit run app.py

#Detailed Functionality
Speech Recognition
The function sptext() captures and recognizes the user's speech. It uses the speech_recognition library and handles exceptions for timeouts and recognition errors.

IELTS Speaking Test
The ielts_speaking_test() function simulates the three parts of the IELTS Speaking Test:

Part 1: Introduction Questions
Asks a series of introductory questions and captures responses.
Part 2: Cue Card
Presents a cue card topic and captures a detailed response.
Part 3: Follow-Up Questions
Asks follow-up questions related to the cue card topic and captures responses.

#Evaluation
The evaluate_ielts_response() function evaluates the user's responses based on:
Fluency
Vocabulary
Grammar
Pronunciation
Feedback

#Usage
Start the Application:
Click on the "Start IELTS Speaking Test" button to begin the test.
Respond to Questions:
Answer the questions as prompted by the application.
Receive Feedback:
Get feedback and an estimated band score after each part of the test.

# Project Title: Emotion Prediction Chat Interface

# Project Description

This project provides a simple graphical user interface (GUI) to predict emotions based on user input sentences. The model uses a SentenceTransformer for text embeddings and a Multi-Layer Perceptron (MLP) for emotion classification. The GUI allows users to input text, processes it through the model, and displays the predicted emotion.

# Key Components 

1. Dataset Preprocessing

Description: The dataset consists of text data and associated emotions. Preprocessing is done to clean the text and prepare it for embedding.

Key Steps:

Convert text to lowercase.

Remove special characters, punctuation, and numbers.

Remove stopwords.

Tokenize and clean the text.

2. Sentence Embedding

Model: SentenceTransformer('all-MiniLM-L6-v2')

Purpose: Converts preprocessed text into vector embeddings for use in the classification model.

3. Emotion Classifier

Model: Multi-Layer Perceptron (MLP)

Hidden layers: (128, 64)

Activation: ReLU

Max iterations: 200

Purpose: Classifies text embeddings into predefined emotion categories.

4. Graphical User Interface (GUI)

Framework: ipywidgets for creating a simple chat-style interface in Jupyter Notebook.

Features:

Text input box for user messages.

Display area for conversation history.

Emotion prediction shown as a response to the user’s input.

5. Sample Sentences for Testing

Examples:

"I am so excited about the trip tomorrow!"

"Why does everything have to go wrong for me?"

"I'm feeling really happy and grateful today."

"This is the most frustrating experience I've ever had."

"I feel lonely and left out sometimes."


# Requirements File

File: requirements.txt

Contents:

numpy

pandas

scikit-learn

sentence-transformers

ipywidgets

nltk

# Chatbot with Keras

This project implements a simple chatbot using Keras, with TensorFlow as the backend. The chatbot is trained on predefined intents and utilizes a neural network model to generate responses.

## Overview

This repository contains the following files:

- **chat.py**: Script for interacting with the chatbot. It loads the trained model, tokenizer, and label encoder to process user input and generate responses.

- **train.py**: Script for training the chatbot model. It reads intents from a JSON file, preprocesses the data, trains a neural network model, and saves the trained model, tokenizer, and label encoder for later use.

- **intents.json**: JSON file containing intents along with associated patterns and responses. This file is used for training the chatbot.

- **label_encoder.pickle**: Pickle file containing the label encoder object used to encode training labels.

- **requirements.txt**: File listing the Python dependencies required to run the chatbot code.

- **tokenizer.pickle**: Pickle file containing the tokenizer object used to tokenize input text for training and inference.

## Usage

Follow these steps to train and interact with the chatbot:

1. **Training**: Execute `train.py` to train the chatbot model using the intents specified in `intents.json`. The trained model, tokenizer, and label encoder will be saved for later use.

    ```
    python train.py
    ```

2. **Chatting**: Run `chat.py` to start interacting with the trained chatbot. Type messages, and the chatbot will respond accordingly. Type "quit" to exit the chat.

    ```
    python chat.py
    ```

## Requirements

Ensure you have the required dependencies installed. You can install them using the following command:

```
pip install -r requirements.txt
```

## Dependencies

- TensorFlow (2.3.1)
- NLTK (3.5)
- Colorama (0.4.3)
- NumPy (1.18.5)
- Scikit-learn (0.23.2)
- Flask (1.1.2)


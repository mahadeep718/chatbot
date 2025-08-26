# chatbot
Chatbot with CNN + RNN (LSTM) Model

This is a chatbot implementation using a combination of Convolutional Neural Networks (CNNs) and Recurrent Neural Networks (RNNs) with LSTMs. The chatbot is trained on an intents dataset and can interact with users based on predefined responses.

Features

Uses NLP (Natural Language Processing) for text understanding.

CNN + LSTM model for better intent recognition.

Supports training on custom datasets (intents.json).

Saves vocabulary (words.pkl) and intent classes (classes.pkl).

Loads a pre-trained model for real-time chat interactions.

Installation

Ensure you have Python installed. Install the required dependencies:

pip install tensorflow numpy nltk

Dataset (intents.json)

Modify the intents.json file to add custom intents and responses. Example format:

{
  "intents": [
    {
      "tag": "greeting",
      "patterns": ["Hello", "Hi there", "Hey!"],
      "responses": ["Hello! How can I assist you?", "Hi there! How can I help?"]
    }
  ]
}

How to Run

1. Train the Model

Run new.py to train the chatbot model:

python new.py

This will:

Process the dataset (intents.json)

Generate words.pkl and classes.pkl

Train the CNN + RNN model

Save the trained model as chatbot_rnn_cnn_model.h5

2. Start the Chatbot

Run chatbot.py to interact with the trained chatbot:

python chatbot.py

You can now type messages, and the chatbot will respond based on the trained model.

File Structure

├── chatbot.py          # Chatbot interaction script
├── new.py              # Model training script
├── intents.json        # Dataset with patterns and responses
├── words.pkl           # Processed vocabulary
├── classes.pkl         # Processed intent classes
├── chatbot_rnn_cnn_model.h5  # Trained model
├── README.md           # Documentation

Future Enhancements

✅ Add a GUI using Flask, Tkinter, or Streamlit.✅ Convert into a voice-based chatbot using speech_recognition.✅ Store chat history for model improvements.

License

This project is open-source. Feel free to modify and enhance it!

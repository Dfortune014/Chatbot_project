# Chatbot Training Project

This project focuses on training a simple chatbot using a neural network-based approach. The chatbot is designed to understand user input and generate appropriate responses based on pre-defined intents and patterns. The training process involves the use of Natural Language Processing (NLP) techniques, including tokenization, lemmatization, and the creation of a bag-of-words representation.

## Key Components:
1. **Intent Definition:**
   - The project starts with defining intents, each consisting of patterns and corresponding responses, stored in a JSON file (`intents.json`).
   
2. **Data Preprocessing:**
   - NLTK library is employed for tokenization and lemmatization of words in the provided patterns.
   - Vocabulary is created by extracting unique words from patterns, ignoring specific characters.
   - The cleaned vocabulary is then stored in pickle files (`words.pkl` and `classes.pkl`) for later use.

3. **Training Data Creation:**
   - The project generates training data by converting patterns into a bag-of-words representation.
   - Neural network training data is created by associating each pattern with its corresponding intent label.

4. **Neural Network Architecture:**
   - A Sequential Neural Network is utilized for classification.
   - It consists of an input layer, two hidden layers with dropout for regularization, and an output layer with softmax activation for multi-class classification.

5. **Training the Model:**
   - Stochastic Gradient Descent (SGD) is used as the optimizer with categorical crossentropy as the loss function.
   - The model is trained for 200 epochs on the provided training data.

6. **Model Saving:**
   - The trained model is saved as `chatbot_model.h5` for later use in making predictions.

## Dependencies:
- Python
- NLTK (Natural Language Toolkit)
- TensorFlow and Keras

## Instructions for Usage:
1. Clone the repository.
2. Install the required dependencies.
3. Run the training script (`train_chatbot.py`) to train the chatbot model.
4. The trained model (`chatbot_model.h5`) can then be used for chatbot interactions.

Feel free to contribute, provide feedback, or extend the project to enhance the chatbot's capabilities!

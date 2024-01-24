# NLP_ChartBot
Simple chatbot implementation with PyTorch.

The implementation should be easy to follow for beginners and provide a basic understanding of chatbots.
The implementation is straightforward with a Feed Forward Neural net with 2 hidden layers.
Customization for your use case is super easy. Just modify intents.json with possible patterns and responses and re-run the training (see below for more info).
The approach is inspired by this article and ported to PyTorch: https://chatbotsmagazine.com/contextual-chat-bots-with-tensorflow-4391749d0077.

# Training Data
The training data is stored in the intents.json file. You can customize the chatbot by modifying this file and re-running the training.

# Model
The chatbot uses a Feed Forward Neural Net with 2 hidden layers. The input and hidden layers use the ReLU activation function, while the output layer does not use any activation function.

# Predictions
The chatbot makes predictions for new sentences by tokenizing and stemming the input, converting it into a bag-of-words representation, and feeding it into the neural network to produce a probability distribution over the different intents. The chatbot selects the intent with the highest probability and uses the associated response to generate a message back to the user.

# License
This project is licensed under the MIT License - see the LICENSE file for details.

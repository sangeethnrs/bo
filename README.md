README
This repository contains a Rasa chatbot with pre-built configurations for NLU (Natural Language Understanding) and Core, along with custom actions and training data.

Installation
To use this chatbot, you need to have Rasa installed. You can install it using the following command:

Copy code
pip install rasa
Training the model
To train the chatbot, you can use the rasa train command in the terminal. This will use the configuration files config.yml, domain.yml, and the training data in the data/ directory to train a machine learning model for your chatbot.

Copy code
rasa train
Running the chatbot
After training the model, you can run the chatbot using the rasa shell command in the terminal.

Copy code
rasa shell
This will start a chat interface in the terminal where you can interact with the chatbot.

Custom actions
This chatbot includes a custom action to add two numbers. The action is defined in the actions.py file. To add more custom actions, you can create new Python classes in this file and add them to the actions section in domain.yml.

Training data
The training data for the chatbot is defined in the data/ directory. It includes examples of user input and the corresponding intents and entities. You can add more training data by creating new .md files in this directory.

Configuration
The configuration for the chatbot is defined in the config.yml and domain.yml files. The config.yml file includes the pipeline for the NLU and Core components, along with the policies for the dialogue management. The domain.yml file includes the intents, entities, responses, slots, and actions for the chatbot.

Testing
You can test the chatbot using the rasa test command in the terminal. This will evaluate the performance of the chatbot on a test set of data. The test data should be placed in the data/test/ directory.

bash
Copy code
rasa test

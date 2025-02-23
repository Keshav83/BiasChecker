BiasChecker Chatbot
Overview
BiasChecker is an intelligent chatbot that detects biased language in real time and provides a neutral, respectful rephrasing of user inputs. Using state-of-the-art transformer models, it first checks if your message is biased and then, if needed, generates a more neutral version.

Features
Bias Detection: Uses a zero-shot classification model (facebook/bart-large-mnli) to determine if a message is biased.
Real-Time Correction: If bias is detected, it automatically rephrases the input into a neutral tone using a text generation model (t5-small).
Interactive Chat: Engage in a conversation where your inputs are evaluated and corrected on the fly.
Prerequisites
Python 3.x
Transformers library
Install the required package with:

bash
Copy
Edit
pip install transformers
How It Works
User Input: The chatbot waits for your input.
Bias Detection: Your message is analyzed to check whether it is biased.
Neutral Rephrasing: If the input is flagged as biased, the chatbot generates a neutral version.
Interactive Loop: You can continue chatting, or exit by typing "quit" or "exit".
Setup and Installation
Clone the Repository:
bash
Copy
Edit
git clone https://github.com/yourusername/biaschecker-chatbot.git
Navigate to the Project Directory:
bash
Copy
Edit
cd biaschecker-chatbot
Install Dependencies:
bash
Copy
Edit
pip install transformers
Run the Chatbot:
bash
Copy
Edit
python bias_chatbot.py
Running in Google Colab
Open a new notebook in Google Colab.
Paste the chatbot code into a cell.
Run the cell to start interacting with BiasChecker.
Alternatively, upload your bias_chatbot.py file to Colab and run it.
Code Overview
Bias Detection: The chatbot uses a zero-shot classification pipeline with facebook/bart-large-mnli to classify messages as "biased" or "non-biased."
Neutral Correction: When a message is flagged as biased, it leverages a text generation pipeline with t5-small to generate a rephrased, neutral version.
Interactive Loop: The main function continuously prompts for user input, evaluates the bias, and outputs the results until the user decides to exit

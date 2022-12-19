# 21-Intelligent-Chatbot-in-Python-Using-the-spaCy-NLP-Library

>>> How To Create an Intelligent Chatbot in Python Using the spaCy NLP Library

https://www.digitalocean.com/community/tutorials/how-to-create-an-intelligent-chatbot-in-python-using-the-spacy-nlp-library

How to build your own chatbot using a library like spaCy, which is a fast and robust Python-based natural language processing (NLP) library.

> Prerequisites

A. Set-up environments.

Python 3 installed and a programming environment set up. 
You can complete this for your machine with our previous repo tutorials:

https://github.com/vi-u/20-Intelligent-Chatbot-in-Python-Using-the-spaCy-NLP-Library-Environment.git

B. Get an API key for OpenWeather.

Visit the OpenWeather website to create an account. 

https://home.openweathermap.org/users/sign_up

After registering successfully, visit the API keys page to view the API key automatically created for your account. This key should be an alphanumeric sequence of characters.
*****

Step 1 — Setting Up Your Environment

Make sure you are in the directory where you set up your environment and then run the following command:

    source my_env_weather/bin/activate

Now install spaCy:

    pip install -U spacy

Finally, you will download a language model. spaCy’s language models are pre-trained NLP models that you can use to process statements to extract meaning. You’ll be working with the English language model, so you’ll download that.

Run the following command:

    python -m spacy download en_core_web_md

If you run into an error like the following:

    Output
    ERROR: Failed building wheel for en-core-web-md

You need to install wheel:

    pip install -U wheel

Then download the English-language model again.

To confirm that you have spaCy installed properly, open the Python interpreter:

    python

Next, import spaCy and load the English-language model:

    >>> import spacy
    >>> nlp = spacy.load("en_core_web_md")

If those two statements execute without any errors, then you have spaCy installed.

Now close the Python interpreter:

    >>> exit()

You now have everything needed to begin working on the chatbot. In the next section, you’ll create a script to query the OpenWeather API for the current weather in a city.





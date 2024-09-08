# EPQ-2023-24 ( Is it possible to create your own generative AI application?')
In recent years, global financial markets have undergone signficant transformations due to technological developments, with some of the first devices used being brought in in 1992. Since that date several new finacial structures have been devleloped such as cryptocurrencies in 2009. My project foucus on developing a trading system, which utilises the newest technolical development, bringing it into the financial sector (AI Models). The system is powered by the Meta LLaMA 3 AI model, as it is completely open source , thus guarrenteeing its security. The system is then implemented using Python. The aim of my project was to create my own genereative AI application, and which section better than the finacial sector to further develop in terms of technological advancement. The system therefore leverages the Meta LLaMA 3 model to optimise trading stratergies, allowing for a much lower risk trading experience, with little to no experience. For the sake of EPQ however, I will be deplpying this code on a paper trading server, to avoid trading any real money. However the script will work completely on a real trading server.

For ease of locating everything within my EPQ, I have split everything I did up into 4 sections:

1. System Architecture and Design: The core architetcure of the trading system is designed to integrate well with the Alpaca trading platform for both crypto and stocks. The principles of design and architecture were outlined in: https://docs.google.com/document/d/13BjcZTYlAUcUrBQd06XryGKUly5RtZJNYSqxh_GeotY/edit?usp=sharing.
2. Research into AI models, Implementation and Deployment: At the heart of my system is the Meta LLaMA 3 model, however throughout my research I was never sure which AI model was the most effective to use for this stratergy and how actually to deploy the model within my own stratergy. The resources I used to aid me through this process is detailed within: https://docs.google.com/document/d/1RZkVwL7vf-NYWX5ZzuIivQAlrrtIVbDwgcKsg5lx2k8/edit?usp=sharing.
3. Algorithms and Stratergy: However, without anything written or completed planning and research is nothing. In order to meticulously keep track of what I was doing on a week by week basis, I decided to produce a journal, which is linked here: https://docs.google.com/document/d/1duS2emRx1sbmGKn4MuDqW9_WZ7NQvoDogT6nKQVzv-Q/edit?usp=sharing
4. Extras: I decided to keep an extras section amongst these areas in order to evidence anything else I completed, which doesn't fall into these 3 sections: 

Since my project is a programming based artefact, I have decided to present the project in as many ways as possible, meaning anyone will be able to access the Back-End code and execute it within their own terminal, or operate the project through its Front-End which will be hosted on HuggingFace (A website which allows developers to host their own sites for free.) In order to allow anyone to understand the project and use it as intented, I have written a simple tutorial explaining to the user how to operate the front-end and back-end of my project in multiple different ways.

*The following text is written to assist anyone in operating the code and ensuring that they can assess my EPQ to the fullest extent:*

## Operating the back-end

**The back-end is the more difficult method to run, and will require more time and expertise to execute on its own**

*If you simply want to view the final project, scroll down and access the front-end*

In order to operate the back-end python code which I have provided, I have provided the same code in two separate formats, raw python and a Google Colab Jupyter notebook.
### Raw Python
In order to operate the raw python the user first must install an IDE (VSCode), which is a piece of software capeable of executing scripts and providing an outcome within it's own terminal. Once the IDE is installed the user should then navigate to Python's official website, where they should install the python language to their machine. Now that python is installed to your machine using their wizard, the user should then open a virtual environment by typing in the terminal this prompt:

python -m venv venv

And then depending on the machine the user is on execute this following command:

MacOS/Linux: source venv/bin/activate

Windows: .\venv\Scripts\activate

Once the IDE is installed and the virtual environment is up and running, the user should navigate their way to opening a new python file and then pasting in the raw code provided at rawBackEnd.txt. After doing so the user should navigate their way to the terminal tab, usually located as a dropdown menu to replace the console view, once on the terminal tab the user should then install all of the depedencies for my project using the following bash functions:

pip install together

pip install beautifulsoup4

pip install requests

pip install alpaca-trade-api

pip install yfinance

After executing all of these functions it is important to utilise your own API Keys, as it is sadly against the TOS (Terms of Service) of both the together server and alpaca trade server. To begin with in creating an API key for the together server, it is important for the user to visit www.together.ai, and navigate your way to the 'Get Started' tab. After doing so the user should create an account through any of the available means, once the account is created the user should then locate their way to the settings tab and copy the API Key. When the users API key is copied to their clipboard the user should then replace any variables named together_api_key with the key you have copied. Now for the alpaca trade api, we are going to test the project using their paper trading method, to avoid spending any actual money, but functioning the same way as if real money was utilised. In order to create an API key on the alpaca trade server, the user must first visit www.app.alpaca.markets/signup and create an account, once an account is created the server requires the use of an external authentication to prevent security risks, by which for ease I would reccomend setting it up via SMS. Now that your account is secure, visit the home page and navigate your way to API keys, generating a new API key and copying it to the clipboard. Then revisit the python code and replace all variables named alpaca_api_key with the key the user has copied.

After completing all of the previous steps fully the python should now be ready to execute and any previous errors should be resolved. The user can execute the raw python by executing this in the terminal:

python file_name.py (Replace the file_name with the users chosen file name)

### Jupyter Notebook
Running the python within a Jupyter Notebook is the method which I reccomend as no outside knowledge is required into running the python. Firstly the user should visit https://colab.research.google.com/drive/1vzdfIGMti8pqlcNTiDATHs2kX4uUQW_o?usp=sharing.

However before executing any code, it is important to utilise your own API Keys, as it is sadly against the TOS (Terms of Service) of both the together server and alpaca trade server. To begin with in creating an API key for the together server, it is important for the user to visit www.together.ai, and navigate your way to the 'Get Started' tab. After doing so the user should create an account through any of the available means, once the account is created the user should then locate their way to the settings tab and copy the API Key. When the users API key is copied to their clipboard the user should then replace any variables named together_api_key with the key you have copied. Now for the alpaca trade api, we are going to test the project using their paper trading method, to avoid spending any actual money, but functioning the same way as if real money was utilised. In order to create an API key on the alpaca trade server, the user must first visit www.app.alpaca.markets/signup and create an account, once an account is created the server requires the use of an external authentication to prevent security risks, by which for ease I would reccomend setting it up via SMS. Now that your account is secure, visit the home page and navigate your way to API keys, generating a new API key and copying it to the clipboard. Then revisit the python code and replace all variables named alpaca_api_key with the key the user has copied.

This is now all complete and the python should be ready to run box by box, by pressing the play icon next to each section (It's very important that the current cell is complete before running the next cell)
 
## Operating the front-end

**The front-end displays the final state by which my project is in**
In order to operate the back-end python code which I have provided, I have deployed the front-end onto a browser accessible page with the link here: 

To begin with feel free to browse throughout the page and visit, which ever aspect of the project you wish, when you wish to start simpily hit the 'Use My EPQ' button. This button should then take you to s simpiler page, by which the user can input their own API keys (See above for tutorial on receiving these) and the desired investment value. From then on the code should execute and the investment should take place. Visiting the Alpaca webpage and logging in should verify this. **Important Note: This program will not execute before 9am and after 5pm, due to the fact that the markets close when out of these times.**

Thanks for using my EPQ,
Alex Walton

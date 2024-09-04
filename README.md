# EPQ-2023-24 ( Is it possible to create your own generative AI application?')
In recent years, global financial markets have undergone signficant transformations due to technological developments, with some of the first devices used being brought in in 1992. Since that date several new finacial structures have been devleloped such as cryptocurrencies in 2009. My project foucus on developing a trading system, which utilises the newest technolical development, bringing it into the financial sector (AI Models). The system is powered by the Meta LLaMA 3 AI model, as it is completely open source , thus guarrenteeing its security. The system is then implemented using Python. The aim of my project was to create my own genereative AI application, and which section better than the finacial sector to further develop in terms of technological advancement. The system therefore leverages the Meta LLaMA 3 model to optimise trading stratergies, allowing for a much lower risk trading experience, with little to no experience.


This document is written to assist the examinar in operating the code and ensuring that they can assess my EPQ to the fullest extent:

## Operating the back-end
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
 

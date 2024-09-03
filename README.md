# EPQ-2023-24 ( Is it possible to create your own generative AI application?')
This document is written to assist the examinar in operating the code and ensuring that they can assess my EPQ to the fullest extent:

## Operating the back-end
In order to operate the back-end python code which I have provided, I have provided the same code in two separate formats, raw python and a Google Colab Jupyter notebook.
### Raw Python
In order to operate the raw python the user first must install an IDE (VSCode), which is a piece of software capeable of executing scripts and providing an outcome within it's own terminal. Once the IDE is installed the user should then navigate to Python's official website, where they should install the python language to their machine. Now that python is installed to your machine using their wizard, the user should then open a virtual environment by typing in the termianl this prompt:

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

After executing all of these functions...

After executing all of these functions fully the python should now be ready to execute and any previous errors should be resolved. The user can execute the raw python by executing this in the terminal:

python file_name.py (Replace the file_name with the users chosen file name)
 

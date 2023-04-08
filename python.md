# Python

Python is a programming language that is easy to learn and use. It is interpreted, instead of compiled, so you normally run your programs with the python interpreter or executable.


### Installing Python

1. Open a browser and navigate to: https://www.python.org/downloads/
2. Download a version of Python for your operating system.
3. Run the installer.
4. Update your path environment variable.
5. To validate, open a command prompt and type in `python`.
6. You should see the a message about the version of python installed and the python prompt: `>>>`.


### Virtual Environments

To create a virtual environment on Windows:

Note: Python must already be installed.

1. Navigate to your project directory in a command window.
2. Run: `python -m venv <VirtualEnvironmentName>`
3. Activate the virtual environment:
4. Navigate to the virtual enviornment directory.
5. Run: `Scripts\activate`
6. Update pip:
7. Run: `python -m pip install --upgrade pip`
8. If you want to install django:
9. Run: `pip install django`
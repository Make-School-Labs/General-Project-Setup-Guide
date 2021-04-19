# Setting up a Flask Project

Flask framework is a simplistic and micro Python framework that is commonly used to build web servers. Follow this guide to setup a Flask Project.

## Setup and Installation

Make sure to have the latest stable version of Python on your system. If you don't, no worries! Go through this guideline to install Python on your system.

### Setup a virtual environment with venv

To setup a virtual environment:

* `mkdir <your-project-name>` to create a project directory.
* Navigate to your project directory `cd <your-project-directory>`.
* Python3 comes pre built with the `venv` module to create virtual environments. We create a virutal environment by running the command `python3 -m venv /path/to/new/virtual/environment`.
* Navigate to your project directory in your terminal and run this command `python3 -m venv venv`. It is standard to have a venv folder
 A new vitrual environment will be created in a folder called venv
* The second argument is the location to create the virtual environment.
 Generally, you can just create this in your project and call it venv. venv will create a virtual python installation in the venv folder

Activate the environment

* run the command `source venv/bin/activate`, `. venv/bin/activate` in  your terminal to activate the virtual environment.
Note: this works for `zsh` and `bash` terminals. If you use any other please visit [here](https://docs.python.org/3/library/venv.html) to see guide on how to activate a virtual environment

| Shell    | Command |
| ----------- | ----------- |
| bash/zsh     | `$ source venv/bin/activate`|
|fish | `$ source venv/bin/activate.fish`|
|csh/tcsh| `$ source venv/bin/activate.csh`|
|PowerShell Core | `$ venv/bin/Activate.ps1`|
|cmd.exe | `C:\> venv\Scripts\activate.bat`|
|PowerShell | `PS C:\> venv\Scripts\Activate.ps1`|

* You would notice that you are in taken to the venv folder, which is the virtual environment.
* Now we can install packages etc
* Make sure that your pip when you do `pip --version` is for a python3 version.

To deactivate, type `deactivate`

Install Flask

* Now run `pip3 install Flask` to install flask so you can start using it in your project

## Building a Flask Server

Just save it as hello.py or something similar. Make sure to not call your application flask.py because this would conflict with Flask itself.

* create a new file `server.py`

```python
from flask import Flask
# initialize a flask app
app = Flask(__name__)

@app.route('/')
def hello_world():
    return 'Hello, World!'
```

## Run the server

To run the application you can either use the flask command or python’s -m switch with Flask. Before you can do that you need to tell your terminal the application to work with by exporting the FLASK_APP environment variable:

* `export FLASK_APP=server.py`
* `flask run`

## Turn on debug mode

* `export FLASK_ENV=development`
* Detect changes without restarting the server. etc.(lazy loading)

Templates, static folder

## Other References

<https://flask.palletsprojects.com/en/1.1.x/>

<https://docs.python.org/3/library/venv.html>

<https://flask.palletsprojects.com/en/1.1.x/quickstart/>
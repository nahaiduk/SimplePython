# SimplePython
Opinionated environment for making simple python apps. I'm trying to make this experience a bit like joining a project with a senior developer on it that has expressed their opinion and dictated how things should work.

## Install software
Install Python from https://www.python.org/downloads/
Install Visual Studio Code from https://code.visualstudio.com/download 

## Make a folder for the project
Press [Start] and [Run] then type `cmd` and press enter to get a command prompt.
It will start in your profile folder but we're going to keep things short and simple, so move to `c:` and create a folder for us to use with the commands (press [Enter] after each one):

    c:
    md code
    cd code
    md simplepython
    cd simplepython

## Set the environment
Python applications have versions of things, including Python itself, that work together.
To make sure what works today works tomorrow we create an environment and stay within it.
If you then use Python for something else, it wont affect the environment created for this project.
Lots more geek detail [on the Python docs for venv](https://docs.python.org/3/library/venv.html)

But create the environment with `python -m venv c:\code\simplepython` and activate it with `c:\code\simplepython\bin\activate`. The latter command will be used every time you use the command prompt, but VS Code will help with that by recognising the environment.

## Install FastAPI
Now, Flask is currently more popular than FastAPI, but I expect that to change. I think FastAPI is better, and that being my opinion, we're going to use it.
Install it with the command `pip install fastapi uvicorn` and those components and a few dependencies will be added to your environment.

## Hello, World
The accompanying file in this project [helloworld.py](./helloworld.py) is mostly boiler plate code that you don't need to worry about now, but it's a useful test to see if things are running. Create the same file in your `c:\code\simplepython` folder and run `uvicorn helloworld:app` and then see it running in your browser from http://localhost:8000 

## Open Visual Studio Code
Now we've got a Python project that includes some code we can open VS Code and let it install recommended add-ons.

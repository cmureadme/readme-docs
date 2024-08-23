# Setup

This page will cover setup for helping with deploying the website and for helping with developing the website

## Deploying

Ask Lee and/or Eshaan.

## Developing
We're going to get your tech stack for readme-website up and running. This will require
1. Python
1. source code
1. venv
1. learning how Django works

### Python
As of writing, we use Django 5.1, which requires Python 3.10 to 3.12. Get one of those. Newer is probably better. Install Python [here](https://www.python.org/downloads/). Already have an outdated Python version? Get a new one and pay attention to the venv step.

### source code
To get our source code, install git. Run
```
git clone https://github.com/cmureadme/readme-website
```
git will create the directory `readme-website` with our source code.

### venv
_Alternative tutorial: [link](https://realpython.com/python-virtual-environments-a-primer/)_

Virtual environments are good for making sure multiple Python projects can coexist on the same computer. Maybe you have a personal project that requires Python 3.8, or requires a library that conflicts with one of ours. With venv, you don't have to care.

venv comes with Python. `cd` into `readme-website`. Run 
```
python -m venv venv
```

venv creates a virtual environment using the same python that calls venv. If you have an outdated Python, you may need to specify
```
python3.10 -m venv venv
```
or similar.

This creates a `venv` directory. Run
```
(linux/mac) source venv/bin/activate
(windows) venv\Scripts\activate
```
to activate the venv. Now it's like you're in a completely new Python installation. 

Run
```
pip install -r requirements.txt
```
to install libraries you need to build the project.

If you ever add new libraries, use
```
pip freeze > requirements.txt
```
to overwrite the file with your venv's new requirements.

You can use
```
deactivate
```
in your venv to exit it at any time.

### Django
To start a local server, run
```
python manage.py runserver
```
The debug messages that result should include a line like
```
Starting development server at http://127.0.0.1:8000/
```

Open the link. You should now have a functioning local copy of readme-website. Cool! Now what? :blobsweat:
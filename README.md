# setup-venv

## What is `venv`?

`venv` is a built-in module in Python that allows you to create isolated Python environments. It creates a new directory containing a copy of the Python interpreter, as well as a copy of the standard Python library. By creating a virtual environment using venv, you are creating an isolated Python environment that has its own site-packages directory and can have its own version of Python and packages installed.

## Why use `venv`?

Virtual environments help you keep different projects separate and make sure each project has everything it needs to run properly. This keeps things organized, makes it easier to fix problems, and reduces security risks. Virtual environments are also portable, so you can easily share your projects with others or move them to different machines.

## Deploy

You can use a virtual environment to install packages without requiring administrator permissions. Virtual environments are isolated Python environments that can be created and managed using the venv module in Python. Here's an example of how to create a virtual environment and install a package inside it:

1. Create a new virtual environment:

```
python -m venv myenv
```

This will create a new virtual environment named myenv.

2. Activate the virtual environment:

```
source myenv/bin/activate
```
This will activate the virtual environment and change the prompt to indicate that you are now using the virtual environment.

3. Install packages in the virtual environment:

```
pip install pandas
```
If you have a requirements.txt file with libraries listed, you can use:
```
pip install -r requirements.txt
```
requirements.txt:
```
pandas==1.5.3
simple-salesforce==1.12.3
python-dotenv==1.0.0
mysql-connector-python==8.0.32
psycopg2-binary==2.9.5
numpy==1.24.2
pyarrow==11.0.0
fastparquet==2023.2.0
```
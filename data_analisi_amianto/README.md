# VSCode for Python

## 1. Install Extensions

- Install the official 'Python' extension for VSCode from Microsoft.
- Install the official 'Jupyter' extension for VSCode from Microsoft.
- Install the official 'SQLite' extension for VSCode from alexcvzz.
- Install the official 'fastApiEnvironment' for VSCode from Gautam Sagar Mallela.

## 2. Configure Virtual Environment

- Open the terminal in VSCode and create a virtual environment:
  python -m venv venv

- Activate the virtual environment from the VSCode terminal:
  .\venv\Scripts\activate

- If you cannot activate the environment, open the PowerShell terminal in VSCode and run:
  Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass

Then repeat the activation command:
.\venv\Scripts\activate

> If activated, you should see `(.venv)` at the beginning of the terminal prompt.

## 3. Manage Requirements

- In the VSCode terminal, create a `requirements.txt` file:
  pip freeze > requirements.txt

- Install **pandas**, **matplotlib**, and **jupyter** from PowerShell:
  > pip install pandas matplotlib jupyter
  > pip install fastapi uvicorn

or install them one by one:

> pip install pandas

> pip install matplotlib

> pip install jupyter

> pip install fastapi

> pip install uvicorn

- Update the `requirements.txt` file with the currently installed packages (with the virtual environment active):

  > pip freeze > requirements.txt

- To reinstall all dependencies from the `requirements.txt` file, use:
  > pip install -r requirements.txt

## 4. Come testare l’API

- Vai su [http://127.0.0.1:8000](http://127.0.0.1:8000) per vedere la risposta di default dell’API.
- Vai su [http://127.0.0.1:8000/docs](http://127.0.0.1:8000/docs) per accedere alla documentazione interattiva **Swagger** generata automaticamente da FastAPI.

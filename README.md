# Extremely Vulnerable Flask App

[![Pylint](https://github.com/manuelz120/extremely-vulnerable-flask-app/actions/workflows/pylint.yml/badge.svg)](https://github.com/manuelz120/extremely-vulnerable-flask-app/actions/workflows/pylint.yml)

Intentionally vulnerable Python / Flask application, built for educational purposes.

<img src="./demo.png" alt="Demo Image" width="800" />

## Setup

Using `python3` and [venv](https://docs.python.org/3/library/venv.html):

```bash
git clone git@github.com:manuelz120/extremely-vulnerable-flask-app.git
cd extremely-vulnerable-flask-app
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
python3 -m flask run # Can be stopped using CTRL+C
```

Using `docker`:

```bash
git clone git@github.com:manuelz120/extremely-vulnerable-flask-app.git
cd extremely-vulnerable-flask-app
docker build . -t extremely_vulnerable_flask_app
docker run --name extremely_vulnerable_flask_app -p 5000:80 extremely_vulnerable_flask_app  # Can be stopped using CTRL+C or by running `docker kill extremely_vulnerable_flask_app`
```

Afterwards, the app should be running at http://localhost:5000

## Disclaimer ⚠️

**This app is really vulnerable!** 💣

- Don't run it on publicly accessible server / public networks ⚠️
- Don't blindly copy code or use this as an example / template ⚠️
- Turn off after user ⚠️
- Use at your own risk ⚠️

## Getting started

Registration is based on invites. Either hack your way into the systems, or use the leaked invite code `a36e990b-0024-4d55-b74a-f8d7528e1764` to get started.

## Resetting state

Either create a fresh docker container, or remove the local database (`database.db`) and restart the app.

## Tools

- Python 3 + Flask
- SQLAlchemy + SQLite Database
- Jinja Templating
- [Bootstrap-Flask](https://bootstrap-flask.readthedocs.io/en/stable/)

## Vulnerability Documentation, Exploit scripts and solutions

TODO

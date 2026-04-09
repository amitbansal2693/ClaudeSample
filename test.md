### What this project is about

IT is a small learning/demo web app built with Flask. Conceptually, it’s a simple campus-expense/student-portal style app where a user can:

- Visit a landing page
- See UI for register and login
- Eventually manage a profile and expenses (routes are stubbed, not fully implemented yet)

---

### The current focus is on:

- Showing a clean Flask project structure
- Using Jinja2 templates for pages
- Organizing templates and static files
- Preparing endpoints for future auth + CRUD logic

---

### Architecture

#### Client (browser)
- Renders HTML from Flask (templates)
- Loads CSS/JS from static

#### Server (`app.py`)
- Creates the Flask app
- Defines routes:
    ```plaintext
    / → landing.html
    /register → register.html
    /login → login.html
    /logout, /profile, /expenses/... → placeholder text for now
    ```
- Runs dev server on port `5001`

#### Data layer (database)
- Currently only scaffolding (`__init__.py`, `db.py`)
- Intended to hold:
    - DB connection/config
    - Models/helper functions for users and expenses

---

### Structure

```plaintext
app.py
requirements.txt
test.md

database/
    __init__.py
    db.py

static/
    css/style.css
    js/main.js

templates/
    base.html
    landing.html
    login.html
    register.html
```

---

### Tech stack

#### Backend
- Python 3
- Flask
- Jinja2 (via Flask)

#### Frontend
- HTML templates in `templates`
- CSS in `style.css`
- JS in `main.js`

#### Environment/tooling
- macOS
- Python 3.9+ recommended
- Virtualenv with `python3 -m venv .venv`
- Dependencies via `pip` and `requirements.txt`

---

### Installation & setup (macOS)

From your project directory:
```bash
pip install --upgrade pip
pip install -r requirements.txt
python app.py
```

Then open:

- [http://127.0.0.1:5001/](http://127.0.0.1:5001/) – landing
- [http://127.0.0.1:5001/register](http://127.0.0.1:5001/register) – register
- [http://127.0.0.1:5001/login](http://127.0.0.1:5001/login) – login

Other routes (`/logout`, `/profile`, `/expenses/...`) are placeholders for now.
The current focus is on:

Showing a clean Flask project structure
Using Jinja2 templates for pages
Organizing templates and static
Preparing endpoints for future auth + CRUD logic
Architecture
Client (browser)

Renders HTML from Flask (templates)
Loads CSS/JS from static
Server (app.py)

Creates the Flask app
Defines routes:
/ → landing.html
/register → register.html
/login → login.html
/logout, /profile, /expenses/... → placeholder text for now
Runs dev server on port 5001
Data layer (database)

Currently only scaffolding (__init__.py, db.py)
Intended to hold:
DB connection/config
Models / helper functions for users and expenses
Structure

app.py
requirements.txt
test.md

database/
  __init__.py
  db.py

static/
  css/style.css
  js/main.js

templates/
  base.html
  landing.html
  login.html
  register.html


Tech stack
Backend

Python 3
Flask
Jinja2 (via Flask)
Frontend

HTML templates in templates
CSS in style.css
JS in main.js
Environment / tooling

macOS
Python 3.9+ recommended
Virtualenv with python3 -m venv .venv
Dependencies via pip and requirements.txt
Installation & setup (macOS)
From your project directory:
pip install --upgrade pip
pip install -r requirements.txt
python app.py



Then open:

http://127.0.0.1:5001/ – landing
http://127.0.0.1:5001/register – register
http://127.0.0.1:5001/login – login
Other routes (/logout, /profile, /expenses/...) are placeholders for now.

If you want a version of this text formatted for a README instead of test.md, I can adapt it.


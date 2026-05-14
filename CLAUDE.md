# CLAUDE.md

This file provides guidance to Claude Code when working in this repository.

## Project Purpose

A small demo website with an HTML/CSS frontend and a Python Flask backend.
Built as a first project to learn full-stack web basics with Claude Code.

## Setup

```bash
pip install -r requirements.txt
```

## Running the App

```bash
python app.py
```

Then open http://127.0.0.1:5000 in your browser.

## Project Structure

```
small_site1/
├── app.py              # Flask entry point — define routes here
├── requirements.txt    # Python dependencies
├── templates/          # Jinja2 HTML templates rendered by Flask
│   └── index.html
├── static/             # CSS, JS, images — served as-is
│   └── style.css
└── readme.md
```

## Conventions

- All routes go in `app.py`.
- HTML templates go in `templates/` and use Jinja2 syntax (`{{ variable }}`, `{% block %}`).
- Static assets (CSS, JS, images) go in `static/` and are referenced with `url_for('static', filename='...')`.
- Run with `debug=True` locally; never use debug mode in production.

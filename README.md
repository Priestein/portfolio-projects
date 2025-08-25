# portfolio-projects — A polished collection of beginner-to-intermediate coding projects

Tagline: Showcase of Python, Flask, and Web Development projects for portfolios and demos.

Description
-----------
This repository contains five beginner-to-intermediate projects implemented with Python, Flask, and front-end web technologies. Each project is intended to be clear, well-documented, and ready to upload to your GitHub account. Use these projects as portfolio pieces, learning exercises, or starter templates.

Projects included
-----------------
1. File Organizer (Python)
   - A CLI script (file_organizer.py) that sorts files inside a target folder into category subfolders (Images, Documents, Videos, Audio, Archives, Scripts, Others) based on file extensions.
   - Features: dry-run, confirm mode, verbose summary.

2. Weather App (Python, API)
   - A CLI script (weather_app.py) that fetches current weather for a city using the OpenWeatherMap API.
   - Reads the API key from the environment variable OPENWEATHER_API_KEY (recommended).
   - Displays temperature (C/F), humidity, wind, and description.

3. Blog CMS (Flask + SQLite)
   - A minimal blog system (folder: blog_flask_app/) using Flask and SQLite.
   - CRUD for posts: create, read, edit, delete.
   - Includes templates and a small stylesheet. Beginner-friendly and ready to run locally.

4. Portfolio Website (HTML/CSS/JS)
   - A responsive personal site template (folder: portfolio_site/) built using Bootstrap 5.
   - Includes hero, skills, projects, and contact sections. Ready to customize and deploy as a static site.

5. Markdown to HTML Converter (Python)
   - A CLI script (md_to_html.py) that converts a Markdown file (or all .md files in a directory) into HTML pages using the Python markdown package.
   - Output is saved in a target folder; simple template wrapper provided.

How to run each project (quick)
-------------------------------
Notes:
- You're running Python on Windows and install packages with `python -m pip install <package>`.
- Recommended Python version: 3.8+
- Each project includes usage notes (see USAGE.md) and inline comments.

1) File Organizer
   - Install: no external packages required.
   - Run:
     python file_organizer.py --path "C:\path\to\folder"
   - Options: --dry-run, --yes to skip confirmation.

2) Weather App
   - Install: python -m pip install requests python-dotenv (optional)
   - Configure: set environment variable OPENWEATHER_API_KEY with your OpenWeather key.
     On Windows (PowerShell): $env:OPENWEATHER_API_KEY="your_key_here"
   - Run:
     python weather_app.py --city "London"

3) Blog CMS (Flask + SQLite)
   - Install:
     cd blog_flask_app
     python -m pip install -r requirements.txt
   - Initialize DB:
     On first run, the app will create the SQLite DB automatically. Alternatively:
     python -c "from app import init_db; init_db()"
   - Run:
     set FLASK_APP=app.py
     set FLASK_ENV=development
     python -m flask run
     Open http://127.0.0.1:5000

4) Portfolio Website
   - No server required. Open `portfolio_site/index.html` in a browser.
   - Or host as static site on GitHub Pages.

5) Markdown to HTML Converter
   - Install: python -m pip install markdown
   - Run:
     python md_to_html.py --input notes.md --output out_folder

Skills / Tech Stack
-------------------
- Python: scripting, argparse, requests, pathlib, shutil, sqlite3
- Flask: templating (Jinja2), routing, form handling, SQLite integration
- Web: HTML5, CSS3, JavaScript, Bootstrap 5
- Tools: markdown conversion, environment variables, CLI utilities

Contact
-------
Built by Kim Frederick Pam – connect with me on GitHub: https://github.com/kimfrederickpam

License & Attribution
---------------------
This repository is provided as-is for learning and portfolio use. Feel free to adapt or extend these projects.
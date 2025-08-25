USAGE & SETUP

General notes (Windows)
- Use `python -m pip install <package>` to install any package.
- Recommended Python 3.8+.
- You can run the scripts directly from PowerShell or CMD.

1) File Organizer
- No packages required.
- Examples:
  - Dry run:
    python file_organizer.py --path "C:\Users\You\Downloads" --dry-run
  - Perform changes:
    python file_organizer.py --path "C:\Users\You\Downloads" --yes

2) Weather App
- Install dependencies:
  python -m pip install requests python-dotenv
- Set OPENWEATHER_API_KEY environment variable (PowerShell example):
  $env:OPENWEATHER_API_KEY="your_api_key_here"
- Run:
  python weather_app.py --city "New York"

3) Blog Flask App
- From blog_flask_app folder:
  python -m pip install -r requirements.txt
- Run with Flask:
  set FLASK_APP=app.py
  set FLASK_ENV=development
  python -m flask run
- Open http://127.0.0.1:5000

4) Portfolio Site
- No server required. Open portfolio_site/index.html in browser.
- To deploy: push folder to GitHub and enable GitHub Pages (select main branch / docs folder or root).

5) Markdown to HTML Converter
- Install:
  python -m pip install markdown
- Convert a single file:
  python md_to_html.py --input README.md --output out_html
- Convert all .md in a folder:
  python md_to_html.py --input docs --output site_html --recursive

Notes about paths
- On Windows, wrap paths in quotes if they contain spaces.
- Scripts are written to be cross-platform, but tested on Windows.

If you need changes to defaults (like customizing folder names in the file organizer, or HTML templates), open the file and edit the `CATEGORY_MAP` or the Jinja template sections.
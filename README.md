<p align="center"> <img width="200" alt="Taskley Logo" src="https://raw.githubusercontent.com/your-username/Taskley/master/assets/taskley-logo.png"> </p>

<h1 align="center">Taskley — A lightweight desktop task manager with reminders</h1>

<p align="center"> <img alt="Taskley screenshot" src="https://raw.githubusercontent.com/your-username/Taskley/master/extra/promo/taskley-readme.png"> </p>

About
Taskley is a small, cross‑platform desktop task manager built with PySide6 for the UI, SQLite for task storage, and pygame for ringtone playback. It focuses on clear, simple task creation, due dates and timers, category filters, and audible reminders. Settings are persisted using QSettings by default, with an optional migration into the SQLite file if you prefer single-file persistence.

Taskley is intended as a polished hobby / personal‑use application and is suitable as a starting point for learning desktop Python UI development.

Features
Create and edit tasks with title, notes, category, due date, and recurring flag.

Set due dates using a date/time picker or create a countdown timer.

Desktop reminders with snooze and dismiss actions.

Custom ringtone support (select any MP3 on disk).

Minimize to a draggable squircle widget that restores the main window.

Category and status filtering (all / completed / incomplete).

Small, dependency-light architecture: PySide6 + pygame + SQLite.

Emoji easter egg (plays honk sound after three clicks on the logo).

Further information
Ringtone behavior: Taskley stores the ringtone as the path you select and plays that file at reminder time. If you move or delete the original file the ringtone will not play. Consider shipping a licensed MP3 in the honk/ folder if you want a bundled default honk sound.

Settings: currently saved with QSettings. You can migrate settings into the SQLite DB if you want a single file for state and settings.

Installation
Clone the repository:

git clone https://github.com/your-username/Taskley.git

(Optional) Create and activate a virtual environment:

python -m venv venv

source venv/bin/activate (macOS/Linux) or venv\Scripts\activate (Windows)

Install dependencies:

pip install -r requirements.txt

Typical requirements: PySide6, pygame

Run:

python taskley.py

Prebuilt installers are not provided; this repo is source-first.

Requirements
Python 3.9+ recommended

PySide6

pygame (for MP3 playback — note platform codec support may vary)

Optional: a valid licensed MP3 in honk/honk.mp3 for the emoji honk

Configuration
Ringtone: Choose via Settings → Choose Ringtone. Taskley saves the selected absolute path with QSettings. Use Settings → Clear Ringtone to remove it.

Time format: Toggle "Military Time" in Settings.

Dark mode and Stay on Top options are available in Settings.

Where to put a bundled ringtone: honk/honk.mp3 next to the script if you want to ship a default honk.

If you prefer storing settings in the app database, a small migration is supported by creating a settings table in the SQLite DB and reading/writing keys there.

Usage notes and best practices
Do not commit runtime files to Git: add taskley.db and taskley.log to .gitignore.

If you include a ringtone in the repo, ensure you have redistribution rights or use a permissive-licensed sound or instruct users to add their own.

If deploying to other users, consider packaging (PyInstaller / Briefcase / similar) and test pygame audio on target platforms.

Contributing
Contributions are welcome. Please open issues for bugs and feature requests and submit pull requests for fixes. Follow this checklist when opening a PR:

Describe the change and the rationale.

Keep changes small and focused.

Update README where behavior or installation changes.

Add tests where applicable.

See CONTRIBUTING.md (create one if you adopt a workflow).

FAQ
Is my ringtone copied into the app folder? No. Taskley stores the absolute path chosen via the file dialog and will attempt to play that path at reminder time. If you want the sound bundled, add it under honk/honk.mp3 and reference that path.

Where are settings stored? By default in QSettings (platform-specific location). You can migrate them into the SQLite DB with a small settings table if you prefer.

What files should I not push to GitHub?

taskley.db

taskley.log

pycache/ and *.pyc

Editor or OS artifacts (.vscode, .DS_Store, Thumbs.db)

License
Taskley is distributed under the MIT License. See LICENSE for details.

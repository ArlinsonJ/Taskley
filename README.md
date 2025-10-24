<p align="center"> <img width="200" alt="Taskley Logo" src="https://raw.githubusercontent.com/ArlinsonJ/Taskley/master/assets/taskley-logo.png"> </p>

<h1 align="center">😊 <strong>Taskley</strong> — A Lightweight Desktop Task Manager with Reminders</h1>

<p align="center"> <img alt="Taskley Screenshot" src="https://raw.githubusercontent.com/ArlinsonJ/Taskley/master/extra/promo/taskley-readme.png"> </p>

<h2 align="center"><strong>About</strong></h2>

<p align="center"> <strong>Taskley</strong> is a small, cross-platform desktop task manager built with <strong>PySide6</strong>, <strong>SQLite</strong>, and <strong>pygame</strong>.<br> It focuses on clear, distraction-free task creation, due dates and timers, category filters, and audible reminders.<br> Designed as a <strong>personal productivity app</strong> and a <strong>learning project</strong> for Python desktop UI development. </p>

<h2 align="center">✨ <strong>Features</strong></h2>

<p align="center"> 🧾 Create and edit tasks with title, notes, category, due date, and recurring flag<br> ⏰ Due dates or countdown timers for reminders<br> 🔔 Desktop reminders with <strong>Snooze</strong> and <strong>Dismiss</strong> actions<br> 🎵 Custom MP3 ringtone support<br> 🟡 Minimize to a <strong>draggable squircle widget</strong><br> 📁 Filter by <strong>category</strong> or <strong>status</strong> (All / Completed / Incomplete)<br> 🌙 Optional <strong>Dark Mode</strong><br> 📌 <strong>Always on Screen</strong> toggle to stay above other windows<br> ⚙️ Lightweight architecture — <strong>PySide6 + pygame + SQLite</strong><br> 🐣 Hidden emoji easter egg (tap logo three times for a honk) </p>

<h2 align="center">⚙️ <strong>Installation</strong></h2>

<p align="center"> <pre> git clone https://github.com/ArlinsonJ/Taskley.git cd Taskley python -m venv venv </pre> </p>

<p align="center"><strong>Quick install (convenient)</strong></p>

<p align="center"> <code>pip install PySide6 pygame</code> </p>

<p align="center"><strong>Recommended reproducible install (pinned versions)</strong></p>

<p align="center"> <code>pip install -r requirements.txt</code> </p>

<p align="center"><strong>Run</strong></p>

<p align="center"> <code>python taskley.py</code> </p>

<p align="center">💡 <em>Activate the virtual environment before installing.</em></p>

<p align="center"><strong>Windows</strong></p> <p align="center"><code>venv\Scripts\activate</code></p>

<p align="center"><strong>macOS / Linux</strong></p> <p align="center"><code>source venv/bin/activate</code></p>

<p align="center">💡 <em>Prebuilt installers are not provided — this repository is source-first.</em></p>

<h2 align="center"><strong>Requirements</strong></h2>

<p align="center"> <strong>Python 3.9+</strong> recommended<br> <strong>PySide6</strong> for UI<br> <strong>pygame</strong> for MP3 playback (platform codec support may vary)<br> Optional licensed MP3 at <code>honk/honk.mp3</code> to supply the default honk sound </p>

<h2 align="center"><strong>Configuration</strong></h2>

<p align="center"> <table align="center"> <tr><td><strong>Setting</strong></td><td><strong>Description</strong></td></tr> <tr><td>Ringtone</td><td>Choose via Settings → Choose Ringtone. Saved as an absolute path.</td></tr> <tr><td>Time Format</td><td>Toggle Military Time in Settings.</td></tr> <tr><td>Dark Mode</td><td>Enable via Settings.</td></tr> <tr><td>Always on Screen</td><td>Keeps Taskley visible above other windows.</td></tr> <tr><td>Bundled Ringtone</td><td>Place a default MP3 at <code>honk/honk.mp3</code>.</td></tr> <tr><td>Settings Storage</td><td>Saved via <code>QSettings</code> by default; can be migrated into SQLite.</td></tr> </table> </p>

<h2 align="center"><strong>Platform run notes</strong></h2>

<p align="center"><strong>Windows</strong></p>

<p align="center">

Activate venv: <code>venv\Scripts\activate</code><br>

Install: <code>pip install -r requirements.txt</code> or <code>pip install PySide6 pygame</code><br>

Run: <code>python taskley.py</code><br>

pygame MP3 playback may depend on available codecs. </p>

<p align="center"><strong>macOS</strong></p>

<p align="center">

Activate venv: <code>source venv/bin/activate</code><br>

Install: <code>pip install -r requirements.txt</code> or <code>pip install PySide6 pygame</code><br>

Run: <code>python taskley.py</code><br>

Confirm system audio codecs if MP3 playback fails. </p>

<p align="center"><strong>Linux</strong></p>

<p align="center">

Activate venv: <code>source venv/bin/activate</code><br>

Install: <code>pip install -r requirements.txt</code> or <code>pip install PySide6 pygame</code><br>

Run: <code>python taskley.py</code><br>

May need extra system packages (audio codecs, SDL dependencies) for pygame MP3 support. </p>

<h2 align="center"><strong>Usage Notes and Best Practices</strong></h2>

<p align="center"> Do <strong>not</strong> commit runtime files to Git </p>

<p align="center"> <code>taskley.db</code><br> <code>taskley.log</code><br> <code>pycache/</code><br> <code>*.pyc</code><br> <code>.vscode/</code><br> <code>.DS_Store</code><br> <code>Thumbs.db</code> </p>

<p align="center"> 🎶 Only include MP3s you have rights to redistribute.<br> 📦 For deployment, consider <strong>PyInstaller</strong> or <strong>Briefcase</strong>.<br> 🔊 Test pygame audio on target platforms. </p>

<h2 align="center"><strong>FAQ</strong></h2>

<p align="center"> <strong>Q:</strong> Is my ringtone copied into the app folder?<br> <strong>A:</strong> No. Taskley stores only the absolute path you select. If the file moves or is deleted playback will fail. </p>

<p align="center"> <strong>Q:</strong> Where are settings stored?<br> <strong>A:</strong> In your platform’s <code>QSettings</code>. You can migrate them into SQLite if you prefer. </p>

<p align="center"> <strong>Q:</strong> Which files should I ignore in Git?<br> <strong>A:</strong> See the list above and the repository .gitignore. </p>

<h2 align="center"><strong>License</strong></h2>

<p align="center"> Taskley is distributed under the <strong>MIT License</strong>.<br> See <a href="LICENSE">LICENSE</a> for details. </p>

<p align="center"><sub>💛 Made with PySide6, pygame, and a little honk.</sub></p>

<p align="center"> <img width="200" alt="Taskley Logo" src="https://raw.githubusercontent.com/your-username/Taskley/master/assets/taskley-logo.png"> </p>

<h1 align="center">😊 <b>Taskley</b> — A Lightweight Desktop Task Manager with Reminders</h1>

<p align="center"> <img alt="Taskley Screenshot" src="https://raw.githubusercontent.com/your-username/Taskley/master/extra/promo/taskley-readme.png"> </p>

<h2 align="center"><b>About</b></h2>

<p align="center"> <b>Taskley</b> is a small, cross-platform desktop task manager built with <b>PySide6</b>, <b>SQLite</b>, and <b>pygame</b>.<br> It focuses on clear, distraction-free task creation, due dates and timers, category filters, and audible reminders. </p>

<p align="center"> Designed as a <b>personal productivity app</b> and a <b>learning project</b> for Python desktop UI development. </p>

<h2 align="center">✨ <b>Features</b></h2>

<p align="center"> 🧾 Create and edit tasks with title, notes, category, due date, and recurring flag<br> ⏰ Due dates or countdown timers for reminders<br> 🔔 Desktop reminders with <b>Snooze</b> and <b>Dismiss</b> actions<br> 🎵 Custom MP3 ringtone support<br> 🟡 Minimize to a <b>draggable squircle widget</b><br> 📁 Filter by <b>category</b> or <b>status</b> (All / Completed / Incomplete)<br> 🌙 Optional <b>Dark Mode</b><br> 📌 <b>Always on Screen</b> toggle to stay above all windows<br> ⚙️ Lightweight architecture — <b>PySide6 + pygame + SQLite</b><br> 🐣 Hidden emoji easter egg (tap logo three times for a honk) </p>

<h2 align="center">⚙️ <b>Installation</b></h2>

bash
git clone https://github.com/your-username/Taskley.git
cd Taskley

python -m venv venv

# On Windows
venv\Scripts\activate

# On macOS Linux
source venv/bin/activate

pip install -r requirements.txt

python taskley.py
<p align="center">💡 <i>Prebuilt installers are not provided — this repository is source-first.</i></p>

<h2 align="center"><b>Requirements</b></h2>

<p align="center"> <b>Python 3.9+</b> recommended<br> <b>PySide6</b> for UI<br> <b>pygame</b> for MP3 playback (platform codec support may vary)<br> Optional licensed MP3 at <code>honk/honk.mp3</code> to supply the default honk sound </p>

<h2 align="center"><b>Configuration</b></h2>

<p align="center"> <table> <tr><td><b>Setting</b></td><td><b>Description</b></td></tr> <tr><td>Ringtone</td><td>Choose via Settings → Choose Ringtone. Saved as an absolute path.</td></tr> <tr><td>Time Format</td><td>Toggle Military Time in Settings.</td></tr> <tr><td>Dark Mode</td><td>Enable via Settings.</td></tr> <tr><td>Always on Screen</td><td>Keeps Taskley visible above other windows.</td></tr> <tr><td>Bundled Ringtone</td><td>Place a default MP3 at <code>honk/honk.mp3</code>.</td></tr> <tr><td>Settings Storage</td><td>Saved via <code>QSettings</code> by default; can be migrated into SQLite.</td></tr> </table> </p>

<h2 align="center"><b>Usage Notes and Best Practices</b></h2>

<p align="center"> Do <b>not</b> commit runtime files to Git </p>

text
taskley.db
taskley.log
__pycache__/
*.pyc
.vscode/
.DS_Store
Thumbs.db
<p align="center"> 🎶 Only include MP3s you have rights to redistribute.<br> 📦 For deployment, consider <b>PyInstaller</b> or <b>Briefcase</b>.<br> 🔊 Test pygame audio on target platforms. </p>

<h2 align="center"><b>Contributing</b></h2>

<p align="center"> Contributions are welcome. Open issues for bugs and feature requests and submit pull requests for improvements. </p>

<p align="center"><b>Pull Request Checklist</b></p>

<p align="center"> ✔️ Describe the change and its purpose<br> ✔️ Keep commits small and focused<br> ✔️ Update README if setup or behavior changes<br> ✔️ Add or update tests when possible </p>

<p align="center"><i>See <code>CONTRIBUTING.md</code> if you plan to contribute regularly.</i></p>

<h2 align="center"><b>FAQ</b></h2>

<p align="center"> <b>Q:</b> Is my ringtone copied into the app folder?<br> <b>A:</b> No. Taskley stores only the absolute path you select. If the file moves or is deleted playback will fail. </p>

<p align="center"> <b>Q:</b> Where are settings stored?<br> <b>A:</b> In your platform’s <code>QSettings</code>. You can migrate them into SQLite if you prefer. </p>

<p align="center"> <b>Q:</b> Which files should I ignore in Git?<br> <b>A:</b> See the list above and the repository .gitignore. </p>

<h2 align="center"><b>License</b></h2>

<p align="center"> Taskley is distributed under the <b>MIT License</b>.<br> See <a href="LICENSE">LICENSE</a> for details. </p>

<p align="center"><sub>💛 Made with PySide6, pygame, and a little honk.</sub></p>

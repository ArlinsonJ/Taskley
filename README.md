<p align="center">
  <img width="200" alt="Taskley Logo" src="https://raw.githubusercontent.com/your-username/Taskley/master/assets/taskley-logo.png">
</p>

<h1 align="center">🕒 <b>Taskley</b> — A Lightweight Desktop Task Manager with Reminders</h1>

<p align="center">
  <img alt="Taskley Screenshot" src="https://raw.githubusercontent.com/your-username/Taskley/master/extra/promo/taskley-readme.png">
</p>

---

<h2 align="center">📝 <b>About</b></h2>

<p align="center">
<b>Taskley</b> is a small, cross-platform desktop task manager built with <b>PySide6</b>, <b>SQLite</b>, and <b>pygame</b>.<br>
It focuses on simplicity — clear task creation, due dates and timers, category filters, and audible reminders.
</p>

<p align="center">
Taskley is ideal as a <b>personal productivity tool</b> or as a <b>learning project</b> for desktop Python UI development.
</p>

---

<h2 align="center">✨ <b>Features</b></h2>

<p align="center">
🧾 Create and edit tasks with title, notes, category, due date, and recurring flag<br>
⏰ Due dates or countdown timers for reminders<br>
🔔 Desktop reminders with <b>Snooze</b> and <b>Dismiss</b> actions<br>
🎵 Custom ringtone support (select any MP3 file)<br>
🟡 Minimize to a <b>draggable squircle widget</b> that restores the main window<br>
📁 Filter tasks by <b>category</b> or <b>status</b> (All / Completed / Incomplete)<br>
⚙️ Lightweight architecture — <b>PySide6 + pygame + SQLite</b><br>
🐣 Hidden emoji easter egg (tap logo three times for a honk!)
</p>

---

<h2 align="center">📦 <b>Installation</b></h2>

```bash
# Clone the repository
git clone https://github.com/your-username/Taskley.git
cd Taskley

# (Optional) Create and activate a virtual environment
python -m venv venv

# On Windows
venv\Scripts\activate

# On macOS/Linux
source venv/bin/activate

# Install dependencies
pip install -r requirements.txt

# Run Taskley
python taskley.py
<p align="center"> 💡 <i>Prebuilt installers are not provided — this repository is source-first.</i> </p>
<h2 align="center">🧰 <b>Requirements</b></h2> <p align="center"> <b>Python 3.9+</b> (recommended)<br> <b>PySide6</b> — for the UI<br> <b>pygame</b> — for MP3 playback (platform codec support may vary)<br> <b>Optional:</b> a valid licensed MP3 placed in <code>honk/honk.mp3</code> for the default honk sound </p>
<h2 align="center">⚙️ <b>Configuration</b></h2> <p align="center">
Setting	Description
Ringtone	Choose a custom MP3 via <b>Settings → Choose Ringtone</b>. Saved as an absolute path.
Time Format	Toggle <b>Military Time</b> in Settings.
Dark Mode	Enable via Settings for a dark interface.
Stay on Top	Keeps the window above all others.
Bundled Ringtone	Place a default file at <code>honk/honk.mp3</code>.
Settings Storage	Saved via <code>QSettings</code> by default; optional migration into SQLite.

</p>
<h2 align="center">💡 <b>Usage Notes & Best Practices</b></h2> <p align="center"> Do <b>not</b> commit runtime files to Git: </p>
bash
Copy code
taskley.db
taskley.log
__pycache__/
*.pyc
<p align="center"> 🎶 Only include MP3s you have rights to redistribute.<br> 📦 For deployment, consider using <b>PyInstaller</b> or <b>Briefcase</b>.<br> 🔊 Test pygame audio on your target platforms. </p>
<h2 align="center">🤝 <b>Contributing</b></h2> <p align="center"> Contributions are welcome! Please open issues for bugs and feature requests, and submit pull requests for fixes or enhancements. </p> <p align="center"><b>Pull Request Checklist:</b></p> <p align="center"> ✔️ Describe the change and its purpose<br> ✔️ Keep commits focused and small<br> ✔️ Update README if behavior or setup changes<br> ✔️ Add or update tests when possible </p> <p align="center"> <i>See <code>CONTRIBUTING.md</code> (if present) for more workflow details.</i> </p>
<h2 align="center">❓ <b>FAQ</b></h2> <p align="center"> <b>Q:</b> Is my ringtone copied into the app folder?<br> <b>A:</b> No. Taskley only stores the absolute file path you select. If the file moves or is deleted, playback will fail. </p> <p align="center"> <b>Q:</b> Where are settings stored?<br> <b>A:</b> In your platform’s default <code>QSettings</code> storage. You can optionally migrate them into SQLite. </p> <p align="center"> <b>Q:</b> Which files should I ignore in Git?<br> <b>A:</b> </p>
bash
Copy code
taskley.db
taskley.log
__pycache__/
*.pyc
.vscode/
.DS_Store
Thumbs.db
<h2 align="center">📄 <b>License</b></h2> <p align="center"> Taskley is distributed under the <b>MIT License</b>.<br> See <a href="LICENSE">LICENSE</a> for details. </p>
<p align="center"> <sub>💛 Made with PySide6, pygame, and a little honk.</sub> </p> ```

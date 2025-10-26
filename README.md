<p align="center"> <img width="200" alt="Taskley Logo" src="https://github.com/ArlinsonJ/Taskley/Images](https://github.com/ArlinsonJ/Taskley/tree/main/Images/taskley-logo.png"> </p>

<h1 align="center">😊 <strong>Taskley</strong> — A Lightweight Desktop Task Manager with Reminders</h1>

<p align="center"> <img alt="Taskley Screenshot" src="https://raw.githubusercontent.com/ArlinsonJ/Taskley/master/extra/promo/taskley-readme.png"> </p>

<h2 align="center">📝 About</h2>

<p align="center"> <strong>Taskley</strong> is a small, cross-platform desktop task manager built with <strong>PySide6</strong>, <strong>SQLite</strong>, and <strong>pygame</strong>.<br> It focuses on clear, distraction-free task creation, due dates and timers, category filters, and audible reminders.<br> Designed as a <strong>personal productivity app</strong> and a <strong>learning project</strong> for Python desktop UI development. </p>

<p align="center"> The <code>honk/</code> folder is used only for the emoji easter egg (plays the honk sound after tapping the logo three times) and is not required for normal operation. </p>

<h2 align="center">✨ Features</h2>

<p align="center"> 🧾 Create and edit tasks with title, notes, category, due date, and recurring flag<br> ⏰ Due dates or countdown timers for reminders<br> 🔔 Desktop reminders with <strong>Snooze</strong> and <strong>Dismiss</strong> actions<br> 🎵 Custom MP3 ringtone support (select any MP3 file on your system)<br> 🟡 Minimize to a <strong>draggable squircle widget</strong><br> 📁 Filter by <strong>category</strong> or <strong>status</strong> (All / Completed / Incomplete)<br> 🌙 Optional <strong>Dark Mode</strong><br> 📌 <strong>Always on Screen</strong> toggle to stay above other windows<br> ⚙️ Lightweight architecture — <strong>PySide6 + pygame + SQLite</strong><br> 🐣 Hidden emoji easter egg (tap logo three times for a honk) </p>

<h2 align="center">Requirements</h2>

<p align="center"> <strong>Python 3.9+</strong> recommended<br> <strong>PySide6</strong> for the UI<br> <strong>pygame</strong> for MP3 playback (platform codec support may vary) </p>

<h2 align="center">Configuration</h2>

<p align="center"> <table align="center"> <tr><td><strong>Setting</strong></td><td><strong>Description</strong></td></tr> <tr><td>Ringtone</td><td>Choose via Settings → Choose Ringtone. Saved as an absolute path.</td></tr> <tr><td>Time Format</td><td>Toggle Military Time in Settings.</td></tr> <tr><td>Dark Mode</td><td>Enable via Settings.</td></tr> <tr><td>Always on Screen</td><td>Keeps Taskley visible above other windows.</td></tr> <tr><td>Settings Storage</td><td>Saved via <code>QSettings</code> by default; can be migrated into SQLite.</td></tr> </table> </p>

<h2 align="center">Usage Notes and Best Practices</h2>

<p align="center"> Do <strong>not</strong> commit runtime files to Git </p>

<p align="center"> <code>taskley.db</code><br> <code>taskley.log</code><br> <code>pycache/</code><br> <code>*.pyc</code><br> <code>.vscode/</code><br> <code>.DS_Store</code><br> <code>Thumbs.db</code> </p>

<p align="center"> 🎶 Only include MP3s you have rights to redistribute.<br> 📦 For packaging or distribution, consider packaging tools and test audio on target platforms.<br> 🔊 When testing, pick a ringtone file accessible on your system; Taskley stores the absolute path and will fail if the file is moved or deleted. </p>

<h2 align="center">FAQ</h2>

<p align="center"> <strong>Q:</strong> Is my ringtone copied into the app folder?<br> <strong>A:</strong> No. Taskley stores only the absolute path you select. If the file moves or is deleted playback will fail. </p>

<p align="center"> <strong>Q:</strong> Where are settings stored?<br> <strong>A:</strong> In your platform’s <code>QSettings</code>. You can migrate them into SQLite if you prefer. </p>

<p align="center"> <strong>Q:</strong> Which files should I ignore in Git?<br> <strong>A:</strong> See the list above and include a .gitignore matching those entries. </p>

<h2 align="center">License</h2>

<p align="center"> Licensed under the <strong>MIT License</strong> — see <a href="LICENSE-MIT.txt">LICENSE-MIT.txt</a> for details. </p>

<p align="center"><sub>💛 Made with PySide6, pygame, and a little honk. © 2025 ArlinsonJ</sub></p>

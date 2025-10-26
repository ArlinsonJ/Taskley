<p align="center">
  <img width="200" alt="Taskley Logo" src="https://github.com/ArlinsonJ/Taskley/blob/63871331f0b31d50eaf2876d4200726179c5f537/Images/taskley-logo.png">
</p>

<h1 align="center"><strong>Taskley</strong> — A Lightweight Desktop Task Manager with Reminders</h1>

<br><br>

<h2 align="center">Screenshots</h2>

<div align="center">
  <br>
  <p align="center"><strong>Light Mode</strong></p>
  <br>
  <p align="center">
    <img alt="Taskley light mode screenshot" src="https://github.com/ArlinsonJ/Taskley/blob/e67439cc60936ea0b19fdbf790d047eb911eace5/Images/light-mode.png">
  </p>
  <p align="center">Main app window in the light theme showing the logo, task list, filters, and primary actions</p>
</div>

<br><br>

<div align="center">
  <br>
  <p align="center"><strong>Dark Mode</strong></p>
  <br>
  <p align="center">
    <img alt="Taskley dark mode screenshot" src="https://github.com/ArlinsonJ/Taskley/blob/e67439cc60936ea0b19fdbf790d047eb911eace5/Images/dark-mode.png">
  </p>
  <p align="center">Same main view using the dark theme to show colors, contrast, and style parity. Dark Mode displays times in military format as it was tuned on in settings</p>
</div>

<br><br>

<div align="center">
  <br>
  <p align="center"><strong>Add Task</strong></p>
  <br>
  <p align="center">
    <img alt="Taskley add task screenshot" src="https://github.com/ArlinsonJ/Taskley/blob/e67439cc60936ea0b19fdbf790d047eb911eace5/Images/add-task.png.png">
  </p>
  <p align="center">Add Task page demonstrating the title, notes, due-date/timer controls, recurring toggle, and custom category input</p>
</div>

<br><br>

<div align="center">
  <br>
  <p align="center"><strong>Task Details</strong></p>
  <br>
  <p align="center">
    <img alt="Taskley task details screenshot" src="https://github.com/ArlinsonJ/Taskley/blob/78da200f799ed922944aad9637710c938e9b4e22/Images/task-details.png">
  </p>
  <p align="center">Task details view with formatted due date, notes, category, and recurring information</p>
</div>

<br><br>

<div align="center">
  <br>
  <p align="center"><strong>Edit Task</strong></p>
  <br>
  <p align="center">
    <img alt="Taskley edit task screenshot" src="https://github.com/ArlinsonJ/Taskley/blob/e67439cc60936ea0b19fdbf790d047eb911eace5/Images/edit-task.png">
  </p>
  <p align="center">Edit Task page pre-filled with Title, Notes, Due Date/Timer, Category, and Recurring toggle</p>
</div>

<br><br>

<div align="center">
  <br>
  <p align="center"><strong>Settings</strong></p>
  <br>
  <p align="center">
    <img alt="Taskley settings screenshot" src="https://github.com/ArlinsonJ/Taskley/blob/e67439cc60936ea0b19fdbf790d047eb911eace5/Images/settings.png">
  </p>
  <p align="center">Settings page showing toggles (Dark Mode, Military Time, Stay on Top), and ringtone selector</p>
</div>

<br><br>

<div align="center">
  <br>
  <p align="center"><strong>Minimized</strong></p>
  <br>
  <p align="center">
    <img alt="Taskley minimized widget screenshot" src="https://github.com/ArlinsonJ/Taskley/blob/e67439cc60936ea0b19fdbf790d047eb911eace5/Images/minimized.png">
  </p>
  <p align="center">Squircle minimized widget displayed after minimizing the app, showing the compact logo and drag behavior</p>
</div>

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

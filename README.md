# Teacher Gradebook — downloads

Windows desktop version of **Teacher Gradebook**, an offline gradebook for teachers: classes, timetable, homework and test
scores, behaviour, student notes and reviews. It syncs with the Android app over Wi-Fi, USB or a sync file.

This repository only holds the downloads. Each [release](../../releases) has the Windows files that match the Android app of the same version.

## Install
1. Download `TeacherGradebook-Setup-<version>.exe` from the [latest release](../../releases/latest).
2. Double-click it. Windows may show **"Windows protected your PC"** because the app is not code-signed yet:
   click **More info → Run anyway**.
3. It installs for your Windows user only (no administrator password), adds Desktop and Start menu shortcuts, and opens the app.
4. On first launch the gradebook is empty: import your own `.xlsx` workbook, create a new term, sync from your phone,
   or bring in data from the old portable app (below).

## Updating
The installed app updates itself. It checks when it opens and every few hours, downloads the new version in the background,
and shows **"Version X is ready"**. Click **Restart now** (or **Later**, and it updates when you close the app).
Your gradebook is backed up before every update. You can also check by hand in **Sync → Backups → Check for updates**.

When the phone and the PC must be on the same version to sync, the app tells you, with a button to update the PC.

## Moving from the old portable `.exe` (1.0.7 and earlier)
1. Install `TeacherGradebook-Setup-<version>.exe` as above.
2. On the welcome screen click **Bring In Data from the Old PC App** and pick `gradebook.db` from the old `data` folder
   (next to the old `TeacherGradebook-Portable` `.exe`). Its backups come across too. The old file is left where it was.
3. Once everything is there, you can delete the old portable `.exe`.

The portable `.exe` is still on each release for people who can't install programs, but it can't update itself:
download the new one into the same folder by hand.

## Your data
- The installed app saves everything in **`Documents\Teacher Gradebook`** (`gradebook.db` + a `backups` folder).
  Nothing is uploaded anywhere. Updating or uninstalling the app leaves this folder alone.
- **Back up:** Sync → Backups → **Back up now**, or copy `gradebook.db` somewhere safe. **Open data folder** shows where it is.
- **Restore:** Sync → Backups, pick a backup and click Restore.
- A database opened by a newer version may not open in an older one.
- The file contains your students' names, grades and notes: keep backups private.

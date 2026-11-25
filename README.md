# Teacher Gradebook — downloads

Windows desktop version of **Teacher Gradebook**, an offline gradebook for teachers: classes, timetable, homework and test
scores, behaviour, student notes and reviews. It syncs with the Android app over Wi-Fi, USB or a sync file.

This repository only holds the downloads. Each [release](../../releases) has the `.exe` that matches the Android app of the same version.

## Install
1. Download `TeacherGradebook-Portable-<version>.exe` from the [latest release](../../releases/latest).
2. Make a folder for it, e.g. `Documents\TeacherGradebook`, and put the `.exe` there. Nothing gets installed.
3. Double-click it. Windows may show **"Windows protected your PC"** because the app is not code-signed yet:
   click **More info → Run anyway**.
4. On first launch the gradebook is empty: import your own `.xlsx` workbook, create a new term, or sync from your phone.

## Your data
- Everything is saved in a `data` folder **next to the `.exe`** (`data\gradebook.db`). Nothing is uploaded anywhere.
- **Back up:** close the app and copy `data\gradebook.db` somewhere safe (e.g. `gradebook-2026-11-25.db`).
- **Restore:** close the app and put the copy back as `data\gradebook.db`.
- Keep the `.exe` and the database together. A database opened by a newer version may not open in an older one.
- The file contains your students' names, grades and notes: keep backups private.

## Updating
Download the new `.exe` into the **same folder** (replace the old one, or keep it as a backup), so it finds the same `data` folder.
When the phone and the PC must be on the same version to sync, the app tells you.

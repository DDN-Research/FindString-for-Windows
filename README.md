# FindString

**Languages:** English | [Українська](README.uk.md) | [Deutsch](README.de.md)

FindString is a free Windows tool (DDN Research, Ukraine) for programmers. It finds every file in a folder (including all subfolders) that contains a given word, phrase or function name, and lets you open the found files in a built-in viewer or in your own editor.

## Download

Get `FindString.exe` from the [Releases](../../releases) page. No installation needed — the program is a single EXE.

## System requirements

| | |
|---|---|
| OS | Windows 7 / 8 / 8.1 / 10 / 11 (32- or 64-bit) |
| Runtime | .NET Framework 4.0 or newer (4.8 is already part of Windows 10 and 11) |
| Disk | < 1 MB |

On Windows 7 without .NET 4.x install the [.NET Framework 4.8 Runtime](https://dotnet.microsoft.com/download/dotnet-framework/net48).

## Installation

1. Copy the EXE to any folder, e.g. `C:\Tools\FindString`.
2. Start `FindString.exe`.
3. If Windows SmartScreen shows "Windows protected your PC", click **More info → Run anyway** (the EXE is not code-signed).

## Quick start

1. Click the **folder icon** and choose the folder to search. The program immediately collects all files with the selected extensions from this folder and all subfolders (left list).
2. Type the text you are looking for in the **Word** field (an earlier search can be picked from the drop-down list).
3. Click **Find string** or press **Enter**. Files containing the text appear in the right list.
4. **Double-click** a file in the right list to open it in the viewer (or your editor). Double-click in the left list opens a file with its default Windows program.
5. Press **Esc** to stop a long search.

## Main window

| Element | Purpose |
|---|---|
| Folder icon | Choose the search folder (files are collected automatically) |
| Settings icon | Open the Settings window |
| Info icon | Version and author info |
| **Search files** | Re-collect the file list from the chosen folder (e.g. after changing extensions) |
| Left list | All files that will be searched |
| **Word** | Text to find (history is kept during the session) |
| **Find string** | Start the search |
| Right list | Files in which the text was found |
| Status bar | Progress and number of files |

## Built-in viewer

Double-clicking a found file opens it in the viewer window:
- **Find** — jumps to the next occurrence of the search text (wraps around to the start);
- **Prew / Next** — open the previous / next file from the result list.

The viewer adds a one-line comment header at the top of the shown text. The file on disk is not changed.

## Settings

- **File(s) extension** — up to 25 masks in the form `*.ext` (max 8 characters, e.g. `*.c`, `*.h`, `*.cpp`, `*.ino`, `*.txt`). **Add** / **Delete** to edit the list.
  Binary formats are skipped automatically even if added: exe, msi, rar, zip, 7z, iso, apk, doc, docx, xls, xlsx, pdf, psd, bmp, jpg, jpeg, mp3, wav, avi, mp4, mpeg, mkv.
- **Run search files with start** — collect files from the last folder automatically when the program starts.
- **Open file to application** — open found files in an external program (e.g. `C:\Program Files\Notepad++\notepad++.exe`) instead of the built-in viewer.

Settings are saved in `%APPDATA%\DDN Research\FindString\set.ini`. **Portable mode:** if a `set.ini` file exists next to the EXE (and the folder is writable), that file is used instead. Delete `set.ini` to reset the program.

## Good to know

- The search is **case-sensitive** (`Define` ≠ `define`).
- Encoding is detected automatically: UTF-8/Unicode files and ANSI files (e.g. Windows-1251 Cyrillic) are both supported. Files larger than 200 MB are skipped.
- Very large folders take time; the status bar shows progress, Esc stops.

## Files in this repository

| File | Description |
|---|---|
| `README.md`, `README.uk.md`, `README.de.md` | User guide (EN / UK / DE) |
| `CHANGELOG.md` | Version history |
| Release asset `FindString.exe` | The program |

Source code is not published.

## License

Freeware. © DDN Research, 2022–2024. Free to use; redistribution only unmodified.

## Contact

[github.com/DDN-Research](https://github.com/DDN-Research)

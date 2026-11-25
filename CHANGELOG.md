# Changelog

## 1.0.3
- Fixed: crash when a file is locked or not accessible during search
- Fixed: crash of the progress bar when only one file is in the list
- Fixed: single click in the file list no longer opens files; use double-click
- Fixed: "Save" in the viewer now really saves the file
- Fixed: settings error when the EXE is in a protected folder (settings moved to %APPDATA%, portable mode kept)
- Fixed: duplicate files for masks like *.htm / *.html
- Fixed: second search could start while a search was running (buttons are locked)
- New: automatic encoding detection (UTF-8 / ANSI, Cyrillic Windows-1251)
- New: Enter in the search field starts the search
- Window position is restored only if it is on a visible screen
- Correct product name, company and version in EXE properties

## 1.0.2
- Search for a word/phrase in files of up to 25 extensions, recursive through subfolders
- Built-in viewer with Find / Previous / Next
- Optional external editor for opening results

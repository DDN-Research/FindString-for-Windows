# FindString

**Sprachen:** [English](README.md) | [Українська](README.uk.md) | Deutsch

FindString ist ein kostenloses Windows-Programm (DDN Research, Ukraine) für Programmierer. Es findet in einem Ordner (inklusive aller Unterordner) alle Dateien, die ein bestimmtes Wort, eine Phrase oder einen Funktionsnamen enthalten, und öffnet die Treffer im eingebauten Betrachter oder in Ihrem eigenen Editor.

## Download

Laden Sie `FindString.exe` von der Seite [Releases](../../releases) herunter. Keine Installation nötig — das Programm besteht aus einer einzigen EXE.

## Systemanforderungen

| | |
|---|---|
| Betriebssystem | Windows 7 / 8 / 8.1 / 10 / 11 (32 oder 64 Bit) |
| Laufzeit | .NET Framework 4.0 oder neuer (4.8 ist in Windows 10 und 11 enthalten) |
| Speicher | < 1 MB |

Unter Windows 7 ohne .NET 4.x installieren Sie die [.NET Framework 4.8 Runtime](https://dotnet.microsoft.com/download/dotnet-framework/net48).

## Installation

1. Die EXE in einen beliebigen Ordner kopieren, z. B. `C:\Tools\FindString`.
2. `FindString.exe` starten.
3. Falls Windows SmartScreen „Der Computer wurde durch Windows geschützt“ meldet: **Weitere Informationen → Trotzdem ausführen** (die EXE ist nicht signiert).

## Schnellstart

1. Auf das **Ordnersymbol** klicken und den Suchordner wählen. Das Programm sammelt sofort alle Dateien mit den gewählten Endungen aus diesem Ordner und allen Unterordnern (linke Liste).
2. Den Suchtext in das Feld **Word** eingeben (frühere Suchen sind in der Liste wählbar).
3. **Find string** klicken oder **Enter** drücken. Dateien mit Treffern erscheinen in der rechten Liste.
4. **Doppelklick** auf eine Datei in der rechten Liste öffnet sie im Betrachter (oder in Ihrem Editor). Doppelklick in der linken Liste öffnet die Datei mit dem Windows-Standardprogramm.
5. **Esc** bricht eine lange Suche ab.

## Hauptfenster

| Element | Funktion |
|---|---|
| Ordnersymbol | Suchordner wählen (Dateien werden automatisch gesammelt) |
| Einstellungssymbol | Fenster „Settings“ öffnen |
| Infosymbol | Version und Autor |
| **Search files** | Dateiliste neu sammeln (z. B. nach Änderung der Endungen) |
| Linke Liste | Alle zu durchsuchenden Dateien |
| **Word** | Suchtext (Verlauf bleibt während der Sitzung erhalten) |
| **Find string** | Suche starten |
| Rechte Liste | Dateien, in denen der Text gefunden wurde |
| Statusleiste | Fortschritt und Anzahl der Dateien |

## Eingebauter Betrachter

Ein Doppelklick auf eine gefundene Datei öffnet den Betrachter:
- **Find** — springt zum nächsten Vorkommen des Suchtextes (danach wieder von vorne);
- **Prew / Next** — vorherige / nächste Datei aus der Trefferliste öffnen.

Der Betrachter fügt oben eine Kommentarzeile in die Anzeige ein. Die Datei auf der Festplatte wird nicht verändert.

## Einstellungen (Settings)

- **File(s) extension** — bis zu 25 Masken im Format `*.endung` (max. 8 Zeichen, z. B. `*.c`, `*.h`, `*.cpp`, `*.ino`, `*.txt`). Mit **Add** / **Delete** bearbeiten.
  Binärformate werden automatisch übersprungen, auch wenn sie eingetragen sind: exe, msi, rar, zip, 7z, iso, apk, doc, docx, xls, xlsx, pdf, psd, bmp, jpg, jpeg, mp3, wav, avi, mp4, mpeg, mkv.
- **Run search files with start** — beim Programmstart automatisch die Dateien aus dem letzten Ordner sammeln.
- **Open file to application** — Treffer in einem externen Programm öffnen (z. B. `C:\Program Files\Notepad++\notepad++.exe`) statt im eingebauten Betrachter.

Einstellungen werden in `%APPDATA%\DDN Research\FindString\set.ini` gespeichert. **Portabler Modus:** Liegt eine `set.ini` neben der EXE (und ist der Ordner beschreibbar), wird diese verwendet. Zum Zurücksetzen `set.ini` löschen.

## Gut zu wissen

- Die Suche unterscheidet **Groß- und Kleinschreibung** (`Define` ≠ `define`).
- Die Kodierung wird automatisch erkannt: UTF-8/Unicode und ANSI (z. B. Windows-1251 mit Kyrillisch). Dateien über 200 MB werden übersprungen.
- Große Ordner brauchen Zeit; Fortschritt in der Statusleiste, Esc bricht ab.

## Dateien im Repository

| Datei | Beschreibung |
|---|---|
| `README.md`, `README.uk.md`, `README.de.md` | Anleitung (EN / UK / DE) |
| `CHANGELOG.md` | Versionsgeschichte |
| Release-Datei `FindString.exe` | Das Programm |

Der Quellcode wird nicht veröffentlicht.

## Lizenz

Freeware. © DDN Research, 2022–2024. Freie Nutzung; Weitergabe nur unverändert.

## Kontakt

[github.com/DDN-Research](https://github.com/DDN-Research)

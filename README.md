# Advanced Wii Extractor

A GUI-powered tool to extract and decode Wii ISO and WBFS files and also can extract into PC-friendly formats.
Currently in its first version so you might encounter unconverted formats or bugs.

---

## 💻 Features

- Extracts Wii disc data using `wit`
- Converts `.bmg` → `.txt` via `wbmgt`
- Optional `.brstm` → `.mp3` support (via `vgmstream-cli`)
- Organized output folders per ISO filename
- Cleans up helper files generated during extraction

---

## 🧰 Requirements

- **Windows 10+**
- Bundled tools:
  - `wit` (Wiimms ISO Tool)
  - `wbmgt` (Wii BMG Tool)
  - `vgmstream-cli.exe` + its required DLLs (`libvgmstream.dll`, `libmpg123-0.dll`, etc.)

Tools can be placed inside the app folder without system-wide installation.

---

## 📂 Output Structure

---

## 📝 Notes

- Extraction may leave behind technical helper files (`setup.bat`, `setup.sh`, etc.) created by `wit`. These are safe to ignore or delete.
- PC conversion supports `.bmg` parsing automatically. Audio (`.brstm`) requires `vgmstream-cli.exe` and DLLs to be present.
- No installation required—this is a standalone executable for personal use.
- Redistribution of source code is not permitted. App is not open source.

---

## 📜 Credits

- `wit` by Wiimm – [Wiimms ISO Tools](https://wit.wiimm.de/)
- `wbmgt` – BMG message file parser (part of Wiimms Tools)
- `vgmstream` (BSD 3-Clause) – for decoding streamed audio formats  
  > “Audio conversion powered by [vgmstream](https://github.com/vgmstream/vgmstream).”

---

## 🧃 Made by Megs Poster

© 2025 Megs Poster. All rights reserved. This software and its associated assets, "that are and is created and owned by Megs Poster", are the intellectual property of Megs Poster and may not be redistributed, modified, or reverse engineered without explicit permission.

This project utilizes third-party command-line tools including `wit`, `wbmgt`, and optionally `vgmstream-cli`. These tools are not developed, owned, or maintained by Megs Poster and remain the property of their respective creators. Attribution and licenses are provided where applicable.
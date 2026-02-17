# GBA Webcade v2.0

A simple, pure frontend Game Boy Advance emulator to play your local ROMs.

## How to Run Locally

You must serve this via a local web server (cannot just open index.html):

1. Open Terminal.
2. Run:
   ```bash
   python3 -m http.server
   ```
3. Open [http://localhost:8000](http://localhost:8000).

## Hosting

Push to GitHub Pages.

## Managing Games

Run `python3 generate_roms.py` after adding new ROMs to the `roms/` folder.

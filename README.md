# GBA Webcade

A simple, pure frontend Game Boy Advance emulator to play your local ROMs.

## How to Run Locally

Because of browser security restrictions (CORS), you cannot simply double-click `index.html` to run this if it loads game files. You must serve it via a local web server.

### Option 1: Python (Built-in on Mac)

1. Open Terminal.
2. Navigate to this folder.
3. Run:
   ```bash
   python3 -m http.server
   ```
4. Open [http://localhost:8000](http://localhost:8000) in your browser.

### Option 2: VS Code Live Server

If you use VS Code, install the "Live Server" extension and click "Go Live".

## Hosting on GitHub Pages

1. Push this repository to GitHub.
2. Go to **Settings** > **Pages**.
3. Select the `main` branch and `/` root folder.
4. Save. Your site will be live!

### How to Update Game List

Anytime you add new games to the `roms` folder, you must run the update script which generates `games.js`:

1. Open Terminal.
2. Run:
   ```bash
   python3 generate_roms.py
   ```
3. This updates `games.js`. Refresh your browser to see the new games.

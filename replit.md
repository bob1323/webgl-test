# blox kid game — Unity WebGL Export

## Overview
This is a Unity WebGL build of a game called "blox kid game". It is a static web project — no backend or build step required.

## Project Structure
- `index.html` — Entry point for the Unity WebGL player
- `Build/` — Compiled Unity game files (loader JS, framework JS, WASM)
- `TemplateData/` — CSS and UI assets for the Unity loading screen

## Running the Project
Served via Python's built-in HTTP server:
```
python3 -m http.server 5000 --bind 0.0.0.0
```
This is configured as the "Start application" workflow on port 5000.

## Notes
- The `Build/webgl test.data.gz` asset file (game data) was not included in the original GitHub import. The game will begin loading but may stall waiting for this file.
- Deployment is configured as a static site (public directory: `.`)

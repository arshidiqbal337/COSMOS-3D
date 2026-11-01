# COSMOS 3D — Interactive Space Explorer

A complete, responsive 3D Solar System explorer built with Three.js, HTML, CSS, and JavaScript. No Node.js/npm installation is required.

## Features
- Interactive 3D Sun and all 8 planets
- Procedural planet textures (no image asset downloads)
- Animated orbit and self-rotation, Saturn and Uranus rings
- Drag-to-rotate, wheel/pinch zoom, and camera focus
- Click-to-select planets or select/search from the sidebar
- Educational fact cards, Wikipedia learning links
- Pause/play, orbit speed control (0–5x), reset camera
- Toggle orbit paths, labels, and starfield
- Fullscreen mode, keyboard shortcuts, responsive UI

## Start on Windows (without Node.js)
1. Extract the ZIP file.
2. Open PowerShell **inside the COSMOS_3D_Complete folder**.
3. Run: `py -m http.server 8000`
   - If `py` isn't recognized, run: `python -m http.server 8000`
4. Open `http://localhost:8000` in Chrome or Edge.
5. Press Ctrl+C in the terminal to stop the server.

Internet is required to load Three.js and Google Fonts from CDNs. The planet textures are generated locally. Do not double-click `index.html` (ES module loading can be blocked under `file://`).

## Controls
- Mouse drag: rotate view
- Mouse wheel: zoom
- Click planet: select and focus
- Space: pause/resume
- R: reset view
- F: focus selected body
- Esc: close info panel

## Project structure
- `index.html`: page structure and accessible controls
- `styles.css`: responsive dark space theme
- `app.js`: Three.js simulation, scene, camera, planets, animation, interactions
- `README.md`: setup and usage
- `LICENSE`: MIT License

## Important scientific note
This is an **educational visualization**, not an ephemeris or astronomy-grade simulation. Planet sizes, distances, axial tilt, rotation/orbital speeds, textures, and motion are artistically adjusted. Planet fact values are approximate and some moon counts change as discoveries are confirmed.

## Troubleshooting
- Blank screen: verify internet access and open DevTools (F12) > Console. The CDN might be blocked; try another network.
- `node`/`npm` not recognized: they are not required for this project.
- Python command not found: install Python from python.org or use VS Code Live Server extension.
- Performance issues: close heavy apps or reduce browser zoom; starfield and textures are already optimized.

## Technology
JavaScript (ES modules), Three.js, HTML5, CSS3, Canvas API, Python built-in HTTP server (development only).

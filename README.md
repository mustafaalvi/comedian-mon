# Comedian Quest — Running & What to Expect

File: [comedian-mon/comedy-rpg.html](comedian-mon/comedy-rpg.html)

This game is entirely created in Javascript using Phaser. 

Quick start
- Open the file in a modern browser (double-click the HTML file) or serve the folder and open http://localhost:8000/comedy-rpg.html.
- To serve locally: run `python -m http.server 8000` in the repository root and open the URL.

Requirements
- Modern browser with ES6 support.
- Internet access for Phaser CDN (phaser.min.js). If offline, replace the CDN script with a local Phaser build.

Controls
- Arrow keys: move the player.
- Follow on-screen prompts while in battle (click battle buttons).

Gameplay summary / expectations
- Top-down tile map with paths, buildings and "tall grass" encounter zones.
- Enter tall grass to trigger random comedian boss encounters (≈30% chance, 3s cooldown).
- Bosses: Jerry (hp 50), Sarah (hp 60), Mike (hp 45). Each has a set of jokes and deals random counter damage.
- Player HP starts at 100; defeated bosses are tracked (UI shows `Defeated: X/3`).
- Battle UI pauses movement; choose moves (Roast / Callback / Crowd Work) to deal damage.
- When a boss is defeated, press any key to exit battle. If player HP hits 0, refresh the page to restart.

Notes / troubleshooting
- If nothing appears, check the browser console for errors (CDN load or JS exceptions).
- To avoid mixed-content or CDN issues, host the HTML on a local server.
- To change encounter/chance/HP values, edit [comedian-mon/comedy-rpg.html](comedian-mon/comedy-rpg.html).

Enjoy the roast.
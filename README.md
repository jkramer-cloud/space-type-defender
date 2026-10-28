# Space Type Defender — v5.0: Nova Bombs & Live Typing Feedback

A lightweight, browser-based typing arcade game for the Naches Learning Hub. Players destroy falling meteors by typing their words, practice vocabulary across grades 1–12, and defend a space station through six increasingly challenging missions.

## What's new in v5.0

- **Nova bomb** — press **Enter** (or click **💥 Bomb**) to destroy every meteor currently on the screen. A brief shockwave and sound accompany the blast.
- **Visible bomb inventory** — start with **2** bombs and hold up to **3**.
- **Earn replacement bombs** — get **+1 bomb every 5 correctly completed words**. Certain **glowing golden supply meteors** also give +1 when typed correctly, up to the inventory limit.
- **Fair scoring and mission progress** — bomb-destroyed meteors do **not** count as typed words or earn points. Replacement meteors spawn so players can still complete their mission.
- **Green/red live typing feedback** — as students type a selected falling word, correct letters glow green and mistyped letters glow red. The input is also highlighted red for invalid text. Use **Backspace** to correct mistakes.
- Existing vocabulary, six levels, Arcade and Relaxed modes, lasers, fullscreen, best-score saving, and grade selection remain unchanged.

## Controls

| Key/control | Action |
| --- | --- |
| Letters | Type a visible meteor word; the word destroys automatically when finished |
| Backspace | Correct a typo |
| Enter | Launch a nova bomb if one is available and a meteor is on-screen |
| Bomb button | Same action, useful for touch screens |
| Escape | Pause or resume |
| Fullscreen | Expand the playfield |

The game has no advertising, external JavaScript dependencies, AI services, or required login. Progress is stored in the browser on that device.

## Update your GitHub Pages repository

1. Open `jkramer-cloud/space-type-defender` on GitHub.
2. Replace the **root** `index.html` with the new file included in this ZIP.
3. Optionally replace `README.md` with this file.
4. Commit the changes to the branch used by GitHub Pages, normally `main`.
5. Refresh `https://jkramer-cloud.github.io/space-type-defender/` with **Ctrl + Shift + R** to clear cached HTML.

The game's link stays the same, so the **main Learning Hub doesn't need a separate update**.

## Classroom notes

The colored letters show whether the typed characters match the selected visible word. If the player mistypes the very first character before selecting any word, the typing field turns red; there is not yet enough information to know which falling word they intended. Students can click a target to select it explicitly.

Bombs are a limited emergency tool for fast-moving threats, not a substitute for typing. The small gold supply meteors reward successfully typing their words. Accuracy and WPM are practice indicators, not a formal assessment.

## Technical

- Pure HTML, CSS and JavaScript in one file
- Responsive design; works on desktops and student Chromebooks
- Local browser storage for scores and progress
- Compatible with existing saved results from v4
- Animated explosions respect the user's reduced-motion preferences

© Naches Learning Hub project. Educational game prototype.

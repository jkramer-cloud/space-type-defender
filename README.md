# Space Type Defender v6.1 — Restored Ship Hangar and Weapons

This restores the **v6 Space Type Defender** features that are missing from the currently published older version. It keeps the original typing missions, grade settings (1–12), score tracking, and gameplay.

## Installation (GitHub Pages)
1. Open your `jkramer-cloud/space-type-defender` GitHub repository.
2. Choose **Add file → Upload files**.
3. Upload this ZIP's **index.html** to the **root** of that repository, replacing the older `index.html`.
4. Commit the update. Allow GitHub Pages to publish it, then force-refresh the game (`Ctrl+Shift+R`).
5. The existing Learning Hub link remains the same: https://jkramer-cloud.github.io/space-type-defender/ . No Learning Hub change is needed.

## Restored features
- Eight spacecraft: Falcon, Dart, Cruiser, Starwing, Comet, Guardian, Nebula, Hexcraft.
- Six laser styles: Cyan Pulse, Violet Plasma, Solar Gold, Emerald Twin, Crimson Rail, Prism Burst.
- Ship Hangar expanded by default so the customization is easy to find.
- Precision Missiles: Tab while typing, or click the Missile button. Starts at 2, holds 4; replenishes every 5 correctly typed words, and from special meteors.
- Nova Bombs: Enter during play, or click the Bomb button. Starts at 2, holds 3; replenishes every 15 correctly typed words, and from occasional special meteors.
- Six space missions, letter-by-letter feedback, fullscreen mode, Arcade and Relaxed modes.

Ship/laser selections and scores are kept in browser local storage. Uploading this revision does not deliberately clear saved scores.

## Notes
- **Use the `index.html` from this package, not the earlier V5 version.** The older live game does not contain the ship or missile features.
- Weapons remove targets but do **not** count as successfully typed words and do not increase typing points.
- The Space Type Defender game's repository is separate from the Naches Learning Hub. You only need to update `space-type-defender`.

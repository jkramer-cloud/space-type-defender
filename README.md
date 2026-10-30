# Space Type Defender v6.2 — Mission Control

A classroom-friendly, single-file typing arcade game for grades 1–12.

## What's new in v6.2

- Six illustrated mission destinations are presented **over the playfield** before launching, rather than in a separate grid above the game.
- Each mission shows its name, difficulty label, target count, word-category count, and destination-inspired planet illustration.
- Grade level and Arcade/Relaxed mode selectors live alongside the mission choices.
- Cleared missions are marked using the grade-specific progress already saved on that device.
- A compact Ship Hangar remains available before and during play; the Mission Control screen links to it directly.
- The original spacecraft designs, lasers, precision missiles, nova bombs, score tracking, and mission gameplay from v6.1 are retained.

## Controls

- **Type** the letters of a visible meteor word to fire a laser.
- **Tab** while the typing field is focused to fire a precision missile. Can also click the Missile button.
- **Enter** launches a nova bomb; can also click the Bomb button.
- **Escape** pauses or resumes during play.
- **Levels** returns to the over-playfield Mission Control screen.

## Installation

1. Open the `jkramer-cloud/space-type-defender` GitHub repository.
2. In the repo root, upload the included `index.html` to replace the current version. The game is standalone; no additional assets or scripts are needed.
3. Commit changes and refresh the GitHub Pages game, preferably with Ctrl+Shift+R.

Your Learning Hub link remains unchanged: `https://jkramer-cloud.github.io/space-type-defender/`

## Progress and testing notes

The game saves loadout choices and grade-specific progress in browser local storage. This update does not intentionally wipe saved records.

The updated document passed structural checks for all required controls, placement of Mission Control within the stage, JavaScript syntax checking, and CSS parsing. A live browser playthrough was not possible because the test browser blocked local navigation, so test launch, return-to-levels, and fullscreen behavior on GitHub Pages after publishing.

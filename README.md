# Space Type Defender — v6.0: Ship Hangar & Precision Missiles

An original, self-contained browser typing game for the Naches Learning Hub. Practice spelling and academic vocabulary across grades 1–12 as meteors approach your station. No account, API key, external image files, or AI service is required.

## What's new in v6.0

### Ship Hangar

Open **Ship Hangar — customize your spacecraft & lasers**, above the mission list. Choose from **8 visibly different spacecraft** and **6 laser effects**; select another ship or laser at any time, including during play. Choices save on the same browser and device independently of the existing score storage.

Ships: Falcon, Dart, Cruiser, Starwing, Comet, Guardian, Nebula, Hexcraft.

Lasers: Cyan Pulse, Violet Plasma, Solar Gold, Emerald Twin, Crimson Rail, Prism Burst. Laser styles are visual only: every accurate keystroke still fires a beam.

### Precision missiles (NEW)

- **Tab** while the typing field is focused, or use the **Missile** button.
- Removes exactly **one** visible falling word: your selected/partially typed word first, otherwise the meteor nearest the station.
- Start with **2**, capacity **4**.
- Earn **1 missile every 5 correctly completed words**.
- Some teal **missile supply meteors** also award a missile when correctly typed.
- Does **not** award points, typing progress, or a correctly completed word. A replacement meteor spawns to keep the mission possible.
- **Shift+Tab** still navigates backward; Tab is only intercepted while actively typing.

### Nova bombs (rebalanced)

- **Enter** while playing, or use the **Bomb** button, to clear all visible meteors.
- Start with **2**, capacity **3**.
- Earn **1 bomb every 15 correctly completed words**, instead of every 5.
- Gold **bomb supply meteors** occur about **3× less frequently** than previously (from 11% to approximately 3.7% chance per spawn).
- Bombs do not award points or completed-word credit; cleared meteors are replaced as needed.

### Live typing feedback

Correct letters appear **green**, mistyped letters **red**, and remaining letters **white** on the active falling word. Use Backspace to correct. This feature from v5.0 is preserved.

## Controls

| Control | Action |
|---|---|
| Type a visible word | Fire your selected laser, letter by letter |
| Backspace | Fix a typing mistake |
| Tab (while typing) | Precision missile: one target |
| Enter | Nova bomb: all targets |
| Escape | Pause / Resume |
| Mouse/touch | Select a falling word or click weapon buttons |
| Ship Hangar | Change ship and laser appearance |

## Play modes

- **Arcade** — clear a mission with no more than three station hits.
- **Relaxed** — practice without a lives limit; finish when ready.
- **Grades 1–12** — grade-adjusted vocabulary lists.
- **6 missions** — increasing difficulty and vocabulary variety.

## Publish on GitHub Pages

1. Extract `Space_Type_Defender_V6_GitHub_Ready.zip`.
2. In your existing `space-type-defender` repository, upload `index.html` and `README.md` to the root, replacing the old versions.
3. GitHub Pages should continue serving the existing URL: `https://jkramer-cloud.github.io/space-type-defender/`.
4. Hard refresh with **Ctrl+Shift+R** if the old version is cached.

No Learning Hub update is needed when the game repository and URL are unchanged.

## Storage and accessibility

- Score data remains in the original `nacheshub_typing_arcade_space_v1` localStorage entry, preserving older scores.
- Ship and laser selections use `nacheshub_space_defender_loadout_v6` localStorage.
- The Hangar and weapon buttons can be reached with normal keyboard or pointer navigation; Shift+Tab remains available while typing.
- Visual animations reduce in intensity if the operating system has **Reduce motion** enabled.
- All weapons are practice aids rather than substitutes for typing. Their kills are not counted as completed words.

## Technology

Vanilla HTML, CSS, JavaScript and inline SVG. Single-file app, no build step, no external dependencies. Works on desktop Chromebooks and modern browsers.

## Version history

- **v6.0** — ship selection, laser styles, one-target missiles, reduced bomb replenishment.
- **v5.0** — nova bombs, dynamic bomb inventory, typing letter feedback.
- **v4.0** — illustrated spacecraft, animated laser attacks, centered portrait arcade.

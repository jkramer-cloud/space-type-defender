# Space Type Defender v6.3 — Weapon Progression Fix

Standalone HTML5 typing arcade for the Naches Learning Hub. Includes six illustrated missions, selectable grade 1–12 vocabulary, Arcade/Relaxed modes, eight customizable spacecraft, six laser styles, precision missiles, nova bombs, and browser-local progress.

## GitHub deployment

1. In the `space-type-defender` repository, upload this package's `index.html`, replacing the previous file.
2. Commit to the publishing branch, typically `main`.
3. Refresh the GitHub Pages game (Ctrl+Shift+R) and open Mission Control.
4. No Learning Hub changes are required if it already links to this repository.

Everything needed to play is inside `index.html`. No third-party libraries or online APIs are required.

## Updated weapons — earned from typed words

| Mission | Starting missiles | Starting bombs | Missile capacity | Bomb capacity | Typed words per missile | Typed words per bomb |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| 1 — Academy Orbit | 0 | 0 | 1 | 0 | 6 | Not available |
| 2 — Meteor Trail | 1 | 0 | 2 | 0 | 8 | Not available |
| 3 — Nebula Passage | 1 | 0 | 2 | 0 | 7 | Not available |
| 4 — Satellite Siege | 1 | 0 | 2 | 1 | 7 | 12 |
| 5 — Comet Run | 2 | 1 | 3 | 2 | 7 | 12 |
| 6 — Final Frontier | 2 | 1 | 3 | 2 | 6 | 12 |

- Weapons do **not** count as typed words or advance mission completion.
- Progress indicators show **correctly typed words** earned toward the next weapon, beginning at 0 in each new/restarted mission.
- Progress pauses while weapon inventory is full. Use a weapon to resume earning its progress; there are no hidden rewards.
- Random supply-weapon meteors were removed to make the thresholds deterministic.
- `Tab` fires a missile at the selected or most urgent meteor. `Enter` launches a bomb when available.
- Missile firing always clears the old selection, typed text, and highlights to avoid a stale word prompt.
- Target words will not repeat within a mission until the eligible word pool is exhausted, and the recent word list reduces immediate repeats after recycling.

## Testing

Browser automation validated the six mission starting inventories, missile and bomb word thresholds, locked bombs in missions 1–3, inventory caps, target clearing when launching missiles, word rotation, and keyboard controls. No JavaScript page errors were observed in these tests.

Saved scores and ship customization remain under their existing localStorage keys. Changing the HTML does not intentionally reset them.

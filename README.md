# Crossy Words — v2.5 Mythic Collection

A free, self-contained, browser-based grammar hopping game for grades 3–12. Choose between five grade bands and three Arcade difficulties, dodge traffic and trains, cross rivers and moving word platforms, and collect characters with coins earned by playing.

**No account, AI service, API key, real-money purchase, or external asset download is required.**

## Update existing GitHub Pages site

1. Open the `crossy-words` repository on GitHub.
2. Upload this package's `index.html` to replace the old `index.html` in the repository root.
3. Optionally replace `README.md` and `CHANGELOG.md`.
4. Commit to your published GitHub Pages branch. The address stays `https://jkramer-cloud.github.io/crossy-words/`.
5. If an old game version appears, refresh with **Ctrl + Shift + R**.

To play offline, open `index.html` in a recent Chrome or Edge browser.

## New in v2.5

### Rarity labels visible in the collection

Every character tile, **including locked silhouettes**, now displays a color-coded rarity label:

- **Common** — slate
- **Rare** — blue
- **Epic** — purple
- **Legendary** — gold
- **Mythic** — glowing violet-pink (new highest tier)

A collection summary shows unlocked and total characters by rarity. Click a summary badge to filter that tier. There are also **rarity filters, species filters, search, and sorting** by species, highest rarity, or recently unlocked. Click an unlocked character to equip it; the original random-equip feature remains.

### Six new character families, 72 additional variations

- Celestial Dragon — dragon with wings, horns, and a star emblem
- Star Knight — armored guardian with star shield and cape
- Moon Kirin — miniature mythical deer with antlers and cosmic tail
- Clockwork Titan — mechanical automaton with gears and glowing eyes
- Nebula Phoenix — flaming-winged bird with colorful feather accents
- Galaxy Leviathan — cosmic serpent with orbital rings and tail

Each family has 12 color variants, with **two Mythic variants**. The collection now includes **648 characters (576 existing + 72 new)** and **12 Mythics** in total. All old character IDs are unchanged, so old saved unlocks remain valid.

### Transparent capsule machine and Mythic guarantee

Capsules still cost **80 earned coins**, unlock characters you don't own, and never give duplicates. The initial rarity-tier roll uses these weights whenever all tiers have locked characters:

| Rarity | Base chance |
| --- | ---: |
| Common | 56% |
| Rare | 25% |
| Epic | 12% |
| Legendary | 5% |
| Mythic | 2% |

Once a tier has no remaining locked characters, its weight is removed and the other available tiers are reweighted. These probabilities are not probabilities for any particular named character; a character is chosen uniformly among the still-locked characters in the selected rarity.

**Mythic safeguard:** If Mythic characters remain locked, the 25th capsule since the last Mythic is guaranteed to award a Mythic. The counter resets when a Mythic is obtained. Mythic characters are cosmetic only and have no mechanical gameplay advantage.

The capsule shop displays the initial odds, remaining pulls until the guarantee, and a special Mythic reveal.

### Mobile collection access

Collection and Capsule Shop buttons are available directly on the start menu, making them accessible on phones before starting a run. Overlays correctly appear above the mobile start screen.

## Existing features retained

- **Five grade bands:** grades 3–4, 5–6, 7–8, 9–10, 11–12.
- **Three Arcade difficulties:** Explorer, Standard, Expert—separate from grammar level.
- **Practice mode:** untimed, with grammar feedback.
- **204 curated grammar questions:** includes homophones, punctuation, agreement, verb tenses, and advanced grammar.
- **16 maps:** each spans 48 rows, with day and night variants.
- **Collision gameplay:** traffic, trains with warnings, river logs, moving word platforms, and safe spaces.
- **Achievements:** 11 general achievements and three badges for each of the 16 maps.
- **Results:** captured final-scene image, best distance, individual character records, and grammar-retry guidance.

## Controls

- **Left/Right arrows** or **A/D**: move across five columns.
- **Up arrow**, **W**, or **Space**: hop forward.
- **P** or **Escape**: pause.
- On-screen buttons support touch input.
- Tap a displayed answer to line up toward a matching moving platform, then time the hop.

## Saved progress, privacy, and classroom note

Progress uses browser `localStorage` with the existing key `crossy_words_hopper_save_v1`. Older coins, character unlocks, equipped characters, achievements, and scores are retained. New rarity filters do not change saved character IDs. The Mythic guarantee and unlock order are additional fields in the same save.

Progress is device/browser-specific. Clearing site data or using a different school Chromebook may reset it. There are no login accounts or cloud synchronization.

All collectibles are cosmetic. Rarity does not confer a competitive benefit. The grammar bank is offline and gives predefined explanations rather than AI assessments.

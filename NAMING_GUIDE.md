# naipes.club — File Naming Guide

All image filenames follow this structure:

```
[card-id]_[gametype]_[deckname]_[tags].png
```

- Separators: underscores `_` between the main fields, hyphens `-` within a field when combining values
- Always lowercase
- No spaces, no accents, no special characters
- Full English words throughout

---

## Part 1 — Card ID

### 1A. Spanish & Italian playing cards

**Suits (full word):**
`swords` · `cups` · `coins` · `batons`

**Cards:**

| Card | Code | Example |
|------|------|---------|
| Ace | `1` | `1-swords` |
| 2 through 9 | number | `7-coins` |
| 10 | `10` | `10-batons` |
| Sota / Fante / Jack | `jack` | `jack-cups` |
| Caballo / Cavallo / Horse | `horse` | `horse-swords` |
| Rey / Re / King | `king` | `king-coins` |
| Joker | `joker` | `joker` |

> Italian decks use the same suit and card codes. The gametype field (`spanish` or `italian`) distinguishes them.

---

### 1B. French playing cards

**Suits (full word):**
`hearts` · `spades` · `diamonds` · `clubs`

**Cards:**

| Card | Code | Example |
|------|------|---------|
| Ace | `1` | `1-hearts` |
| 2 through 10 | number | `5-spades` |
| Jack | `jack` | `jack-diamonds` |
| Queen | `queen` | `queen-clubs` |
| King | `king` | `king-hearts` |
| Joker | `joker` | `joker` |

---

### 1C. German playing cards

**Suits (full English word):**
`acorns` · `leaves` · `hearts` · `bells`

**Cards:**

| Card | Code | Example |
|------|------|---------|
| Ace / Deuce | `1` | `1-acorns` |
| 2 through 9 | number | `7-bells` |
| 10 | `10` | `10-leaves` |
| Unter (lower knave) | `unter` | `unter-hearts` |
| Ober (upper knave) | `ober` | `ober-acorns` |
| König / King | `king` | `king-bells` |

> Note: German hearts (`hearts`) share the name with French hearts. The gametype field (`german` vs `french`) distinguishes them.

---

### 1D. Swiss playing cards

**Suits (full English word):**
`acorns` · `shields` · `roses` · `bells`

Same figure codes as German: `unter` · `ober` · `king`

---

### 1E. Tarot — Major Arcana

Two-digit number + English keyword:

| No. | Code |
|-----|------|
| 0 | `00-fool` |
| I | `01-magician` |
| II | `02-priestess` |
| III | `03-empress` |
| IV | `04-emperor` |
| V | `05-hierophant` |
| VI | `06-lovers` |
| VII | `07-chariot` |
| VIII | `08-justice` |
| IX | `09-hermit` |
| X | `10-wheel` |
| XI | `11-strength` |
| XII | `12-hanged` |
| XIII | `13-death` |
| XIV | `14-temperance` |
| XV | `15-devil` |
| XVI | `16-tower` |
| XVII | `17-star` |
| XVIII | `18-moon` |
| XIX | `19-sun` |
| XX | `20-judgement` |
| XXI | `21-world` |

> If a deck swaps Justice and Strength (Rider-Waite tradition), use the number as printed on the card.

---

### 1F. Tarot — Minor Arcana

**Suits (full English word):**
`wands` · `cups` · `swords` · `pentacles`

> If the deck uses Latin suits instead of Rider-Waite suits, use `coins` instead of `pentacles` and `batons` instead of `wands`.

**Cards:**

| Card | Code | Example |
|------|------|---------|
| Ace | `1` | `1-wands` |
| 2 through 10 | number | `6-cups` |
| Page | `page` | `page-swords` |
| Knight | `knight` | `knight-pentacles` |
| Queen | `queen` | `queen-wands` |
| King | `king` | `king-cups` |

---

### 1G. Non-standard oracle cards

For oracle decks that don't follow tarot structure, use a short descriptive keyword in English:

`sun` · `moon` · `river` · `fire` · `tree` · `serpent` · `tower` · `star` — or any clear descriptive word.

---

### 1H. Family / Quartet games

Format: `[family-number]-[family-theme]_[card-letter]`

- Family number: `1`, `2`, `3`…
- Family theme: a short English word describing what the family is about (`cars`, `birds`, `countries`, `musicians`…). Use this even if it is not printed on the card — it describes the visual content.
- Card letter: `a`, `b`, `c`, `d` (the position within the family)

| Example | Meaning |
|---------|---------|
| `1-cars_a` | Family 1 (cars), card a |
| `3-birds_c` | Family 3 (birds), card c |
| `2-countries_b` | Family 2 (countries), card b |

If the family also has a printed name, add it after the number:
`1-cars-italy_a` → Family 1, theme cars, specific card about Italy, position a

---

### 1I. UNO-style and colour/symbol games

Format: `[number-or-symbol]_[color]_[category]_[deckname]`

**Order is always:** value → color → category → deckname

**Colors:** `red` · `blue` · `green` · `yellow` · `black` · `white` · `purple` · `orange` · `multicolor`

**Number cards:** just the number: `1`, `5`, `9`…

**Action cards (enumerate all possible types):**

| Type | Code |
|------|------|
| Skip | `skip` |
| Reverse | `reverse` |
| Draw two | `draw-two` |
| Draw four | `draw-four` |
| Wild (color change) | `wild` |
| Wild draw four | `wild-draw-four` |
| Swap hands | `swap` |
| Discard all | `discard-all` |
| Hit (specific game action) | `hit` |
| Block | `block` |
| Plus | `plus` |

**Visual/symbol categories:**

| What's on the card | Code |
|--------------------|------|
| Animal (any) | `animal` |
| Bird (any) | `bird` |
| Fish / sea creature | `fish` |
| Insect | `insect` |
| Plant / flower | `plant` |
| Fruit | `fruit` |
| Food / drink | `food` |
| Human / person | `person` |
| Face / portrait | `portrait` |
| Building | `building` |
| Architecture (detail) | `architecture` |
| Vehicle | `vehicle` |
| Boat / ship | `boat` |
| Aircraft | `aircraft` |
| Landscape | `landscape` |
| Object / tool | `object` |
| Pattern / geometric | `pattern` |
| Number (decorative) | `number` |
| Letter / text | `text` |
| Symbol / icon | `symbol` |
| Star / celestial | `celestial` |
| Abstract | `abstract` |

Example filenames for UNO-style:
- `5_red_deckname.png` — number 5, red
- `skip_blue_deckname.png` — skip card, blue
- `wild_multicolor_deckname.png` — wild card
- `7_green-animal_deckname.png` — 7, green, with an animal illustration
- `draw-two_yellow-fruit_deckname.png` — draw two, yellow, fruit illustration

---

## Part 2 — Game Type

| Code | Meaning |
|------|---------|
| `spanish` | Spanish playing cards (baraja española) |
| `italian` | Italian playing cards |
| `french` | French playing cards |
| `german` | German playing cards |
| `swiss` | Swiss playing cards |
| `tarot` | Tarot deck (standard 78 cards) |
| `oracle` | Oracle deck (non-standard) |
| `family` | Family / quartet game |
| `uno` | UNO-style or colour/symbol game |
| `other` | Other / doesn't fit above |

---

## Part 3 — Deck Name

Short, consistent, no spaces, lowercase. Use the same spelling across every file in the deck.

Current decks:
`jumbo` · `panter` · `vanity` · `waterstones` · `neoclas` · `articho` · `ducale` · `aviator` · `tarotcats` · `anaya` · `animales` · `napoli` · `france` · `sedionbel`

---

## Part 4 — Tags (optional but recommended)

Tags go at the end, separated by underscores. Use them to describe visual content beyond what the card ID already tells you — especially useful for playing cards with rich illustrations.

You can stack multiple tags:

```
king-swords_spanish_neoclas_portrait-architecture.png
```

Use the same visual category words from the UNO section above:
`portrait` · `animal` · `landscape` · `building` · `object` · `pattern` · `plant` · `vehicle` · `celestial` · `abstract` · etc.

You don't need to tag every card — tag when the content is distinctive enough to be worth finding later.

---

## Special cards (any game type)

| What | Code | Example |
|------|------|---------|
| Card back (full) | `back` | `back_french_ducale.png` |
| Card back (cropped detail) | `back-detail` | `back-detail_french_ducale.png` |
| Box / packaging | `box` | `box_french_ducale.png` |
| Box detail / label | `box-detail` | `box-detail_french_ducale.png` |
| Rules card | `rules` | `rules_family_jumbo.png` |
| Cover / title card | `cover` | `cover_tarot_articho.png` |
| Instruction booklet | `booklet` | `booklet_spanish_neoclas.png` |

---

## Multiple scans of the same card

If you have more than one image of the same card (variant, front/back, detail):

Add a suffix at the very end: `_a`, `_b`, `_c`

```
1-swords_spanish_neoclas_a.png   ← first scan
1-swords_spanish_neoclas_b.png   ← second scan / variant
```

---

## Full examples

| Filename | Meaning |
|----------|---------|
| `1-swords_spanish_neoclas.png` | Ace of Swords, Spanish deck, Neoclas |
| `7-coins_spanish_ducale.png` | 7 of Coins, Spanish deck, Ducale |
| `king-coins_italian_napoli.png` | King of Coins, Italian deck, Napoli |
| `horse-cups_spanish_france.png` | Horse of Cups, Spanish deck, France |
| `1-hearts_french_waterstones.png` | Ace of Hearts, French deck, Waterstones |
| `queen-spades_french_aviator.png` | Queen of Spades, French deck, Aviator |
| `joker_french_vanity.png` | Joker, French deck, Vanity |
| `7-bells_german_deckname.png` | 7 of Bells, German deck |
| `ober-acorns_german_deckname.png` | Ober of Acorns, German deck |
| `1-hearts_french_waterstones_portrait.png` | Ace of Hearts with portrait illustration |
| `1-a-cars_family_jumbo.png` | Family 1 (cars), card a, Jumbo quartet |
| `3-c-birds_family_panter.png` | Family 3 (birds), card c, Panter quartet |
| `00-fool_tarot_articho.png` | The Fool, Tarot, Articho deck |
| `18-moon_tarot_tarotcats.png` | The Moon, Tarot, TarotCats |
| `5_red_animales.png` | Number 5, red, Animales game |
| `skip_blue_anaya.png` | Skip card, blue, Anaya game |
| `wild-draw-four_multicolor_anaya.png` | Wild draw four, Anaya game |
| `back_french_ducale.png` | Card back, French, Ducale |
| `back-detail_french_ducale.png` | Card back cropped detail, Ducale |
| `box_spanish_neoclas.png` | Box scan, Spanish, Neoclas |
| `rules_family_jumbo.png` | Rules card, Jumbo quartet |

---

## Quick checklist before renaming

- [ ] Lowercase throughout
- [ ] No spaces anywhere
- [ ] No accents (é, ñ, ü, à…)
- [ ] No special characters or Unicode symbols
- [ ] Underscores `_` between main fields only
- [ ] Hyphens `-` within a field (e.g. `1-swords`, `back-detail`, `wild-draw-four`)
- [ ] Gametype always present
- [ ] Deckname always present and spelled consistently
- [ ] Tags at the end, optional but recommended for distinctive illustrations

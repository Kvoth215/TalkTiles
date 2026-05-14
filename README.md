# 🗣️ TalkTiles — Free Picture Communication Board

**TalkTiles is a free, open-source AAC (Augmentative and Alternative Communication) app that runs on any device — no download, no account, no cost.**

Built by and for educators, TalkTiles gives non-verbal and limited-verbal students a voice in the classroom using picture symbols, color-coded core vocabulary, and natural text-to-speech.

👉 **Live app:** [kvoth215.github.io/TalkTiles](https://kvoth215.github.io/TalkTiles)

---

## What's Inside

| Feature | Details |
|---|---|
| ⭐ Core Words | 42 high-frequency words color-coded by type — always the first tab |
| 🗂️ Categories | Feelings, Food, Activities, School, Social & SEL, Academic, Transitions, and more |
| 🍽️ Menus | Red Robin & McDonald's with full item navigation |
| 🌐 Community Library | 25 ready-to-use vocabulary packs, searchable and installable in one tap |
| ⭐ Focus Mode | Distraction-free view for 1:1 sessions or assessments |
| 📲 QR Sharing | Share any category or full vocabulary instantly — students scan and it loads |
| ✏️ Custom Symbols | Add your own words, upload photos, or use any emoji |
| 📥 Import / Export | Back up or share vocabulary as a JSON file |

---

## Core Vocabulary — Why It Matters

Research shows that roughly **80% of everything we say** comes from a small set of 300–400 words. These are called **core words** — words like *want, more, stop, help, like, go, feel, not, please, what, where.*

TalkTiles includes a built-in **⭐ Core Words** tab, always pinned as the first category, with 42 essential words organized and color-coded by type:

| Color | Word Type | Examples |
|---|---|---|
| 🟡 Yellow | Pronouns | I, you, we, my, it, they |
| 🟢 Green | Verbs | want, need, like, go, stop, help, feel, eat |
| 🔵 Blue | Descriptors | more, all done, good, bad, big, little, again |
| 🔴 Red | Negation | no, not, don't, stop it |
| 🩷 Pink | Social | yes, please, thank you, sorry, hi, bye |
| 🟣 Purple | Questions | what, where, who, why, when, how |

The color coding matches the AAC industry standard used in Proloquo2Go, TouchChat, and Snap Core First — so students who move between systems aren't starting over.

> **Motor memory matters.** Core words always appear in the same grid position, so students build muscle memory and can communicate faster without searching.

---

## For Teachers — Adding Your Own Symbols

You don't need to know how to code. Here's how to build vocabulary for any lesson:

**1. Open the app** at [kvoth215.github.io/TalkTiles](https://kvoth215.github.io/TalkTiles) on any device.

**2. Create a category** for your unit — tap the last tab and choose "New Category." Name it something like *Science — Plants* or *Math — Money.*

**3. Add a symbol** using the **+ Add Symbol** button:
- **Label** — short word shown under the picture (e.g., *photosynthesis*)
- **Speech text** — what the app says out loud (e.g., *"Plants use sunlight to make their own food."*)
- **Image** — paste a URL, pick an emoji, or upload a photo from your device

**4. Share it** — use the QR code button to share your category with the whole class instantly.

### Using AI to Build Symbols Faster

Ask Claude (or any AI assistant) to help write speech text:

> *"Give me simple, student-friendly speech text for these science words: photosynthesis, chlorophyll, evaporation. Write each as one sentence a 6th grader would understand."*

> *"I'm teaching a unit on community helpers. Give me 8 symbol ideas with a short label and a one-sentence speech text for each."*

---

## Speaking Settings

TalkTiles uses your device's built-in text-to-speech engine. Current settings:

| Setting | Value |
|---|---|
| Rate | 0.75 (relaxed, natural pace) |
| Pitch | 1.1 |
| Pause between symbols | Comma-separated — natural breath between each word |

Speech works in any modern browser. On iPad and iPhone, go to **Settings → Accessibility → Spoken Content → Voices** to install higher-quality voices.

---

## Vocabulary Data Format

All vocabulary is stored in a single JavaScript object (`VOCAB`) in `index.html`. Categories and symbols are easy to edit or fork:

```javascript
VOCAB.categories = [
  {
    id: "my_category",
    label: "My Category",
    color: "#6366F1",
    emoji: "🌱",
    symbols: [
      {
        id: "symbol_id",
        label: "Label",         // text shown under the picture
        speech: "Speech text",  // what the app says
        svg: "..."              // inline SVG or generated from emoji
      }
    ]
  }
]
```

To add a new built-in category, add an object to `VOCAB.categories` and follow the pattern above. Use the `coreSymSVG()` helper for text-only symbols, or the emoji SVG pattern for picture symbols.

---

## Contribute

TalkTiles is open source and built for classrooms. Contributions are welcome:

- **New vocabulary packs** — add to `LIBRARY_PACKS` following the existing format
- **New restaurant menus** — follow the Red Robin / McDonald's branching pattern
- **Bug fixes** — open an issue or pull request
- **Translations** — speech text can be set to any language your device supports

Fork this repo, make your changes, and open a Pull Request. Every new symbol helps a student communicate.

---

## License

Free for personal, educational, and classroom use.
No account required. No data collected. No ads.

---

*Built with ❤️ for students who deserve to be heard.*

# 🗣️ TalkTiles — Free AAC Picture Communication

**TalkTiles** is a free, open-source, browser-based AAC (Augmentative and Alternative Communication) tool designed for students with communication and special needs. No app store, no account, no cost — just open the URL on any device and start communicating.

🔗 **Live Site:** https://kvoth215.github.io/TalkTiles/

---

## ✨ What's New (v2.0)

TalkTiles has been upgraded with features that bring it closer to commercial AAC tools like Proloquo2Go and TouchChat — at zero cost to schools and families.

### 🆕 New Features

| Feature | Description |
|---|---|
| **Core Word Strip** | Permanent always-visible bar of high-frequency words (I, want, help, more, stop…) — the backbone of real AAC |
| **ARASAAC Integration** | Search and use 12,000+ professional pictograms from the global ARASAAC symbol library |
| **Kiosk / Lock Mode** | Hides all editing controls during student use — one tap to lock, one tap to unlock |
| **Voice Settings** | Choose from all available voices; adjust speed, pitch, and volume per student |
| **Student Profiles** | Multiple named profiles, each with their own vocabulary, stored on-device |
| **Switch Scanning** | Keyboard-based scanning for students who use switches: `Space` to advance, `Enter` to select, `Esc` to stop |
| **Symbol Size Options** | Small / Medium / Large tile sizes for visual or motor needs |
| **Sentence History** | Scrollable log of the last 50 sentences spoken — great for SLP review |
| **Print Mode** | Browser print generates a clean paper backup of any vocabulary board |
| **Usage Tracking** | See which tiles each student uses most — helps SLPs refine vocabulary |
| **Community Library** | Built-in starter packs: Extended Emotions, Food Requests, Classroom Communication |

---

## 🚀 Getting Started

**For students:** Just open the URL. Tap tiles to build a sentence, then tap **Speak**.

**For teachers/SLPs:**
1. Open TalkTiles on a classroom device
2. Tap **Profiles** to create a profile for each AAC student
3. Tap **Edit** to add or modify symbols (search ARASAAC library or use emojis)
4. Tap **Voice** to choose the best voice/speed for each student
5. Tap **Lock** to enter Kiosk mode before handing the device to the student

---

## ⌨️ Switch Scanning (Keyboard / Single Switch)

TalkTiles supports switch-accessible scanning for students with motor impairments:

- **Space** — Start scanning / advance to next tile
- **Enter** — Select the highlighted tile
- **Escape** — Stop scanning

Connect a USB switch interface (e.g., AbleNet Blue2) and map the buttons to Space and Enter.

---

## 🖼️ ARASAAC Pictograms

TalkTiles integrates with [ARASAAC](https://arasaac.org) (Aragonese Portal of Augmentative and Alternative Communication), a free pictogram library used worldwide by schools and AAC professionals.

To search: Click **Add Symbol → Search ARASAAC**, type any word, and pick from the results. Images are served directly from ARASAAC's CDN — no upload needed.

> ARASAAC pictograms are licensed under [Creative Commons BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/). TalkTiles is non-commercial and open-source.

---

## 👤 Student Profiles

Each profile stores:
- Its own vocabulary (categories + symbols)
- Usage statistics
- All data lives in the browser's localStorage — no server, no login

> **Note:** Profiles are device-specific. To share a vocabulary between devices, use the **Export** button and send the `.json` file.

---

## 📲 Sharing Vocabulary

1. Click **Share** in the top bar
2. Choose "This Category" or "All Categories"
3. Click **Generate QR Code**
4. Project the QR code or share the link — students scan and the vocabulary loads instantly

---

## 📊 Usage Stats

TalkTiles tracks which tiles each student taps most. Open **Stats** to see:
- A ranked bar chart of tile usage
- Useful for SLPs during vocabulary reviews
- Reset anytime with **Reset Stats**

---

## 🖨️ Print Mode

Click **Print** in the sentence bar to generate a paper version of the current board — useful for home backups, field trips, or students transitioning between settings.

---

## 🗂️ Community Library Packs

Built-in vocabulary packs you can install with one click:
- **Extended Emotions** — 12 SEL feeling tiles
- **Food & Snack Requests** — Cafeteria and snack choices
- **Classroom Communication** — Materials, turns, and task management

More packs coming. Community contributions welcome — open a GitHub issue!

---

## 🛠️ Technical Details

- **100% static HTML/CSS/JS** — runs on GitHub Pages, no server required
- **Offline-capable** — once loaded, works without internet (ARASAAC images require connection)
- **Cross-platform** — works on Chromebook, iPad, Android, Windows, Mac
- **Storage:** Browser `localStorage` — no data leaves the device
- **ARASAAC API:** `https://api.arasaac.org/api/pictograms/en/search/{term}`

---

## 🤝 Contributing

Pull requests welcome! Priority areas:
- Additional community vocabulary packs
- Cloud sync option (Google Drive / Firebase)
- Improved motor planning layout (LAMP-style consistent placement)
- Multiple communication modes (scene-based, literacy-based)

---

## 📄 License

**TalkTiles code:** [MIT License](LICENSE)

**ARASAAC pictograms:** [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/) — Government of Aragon / ARASAAC

---

## 🙏 Acknowledgments

- [ARASAAC](https://arasaac.org) — for making world-class pictograms freely available
- [qrserver.com](https://goqr.me/api/) — QR code generation API
- Every SLP, special educator, and parent who believes communication is a right, not a product

---

*Built with ❤️ by Paul Kvoth | Neshaminy School District*

# 🌙 Builders of Light

### An Interactive Educational Journey Through the Islamic Golden Age

**Version 1.0** · Single-file HTML app · 830 KB · 139 sections · 434+ functions · 3 languages · Zero dependencies

---

## ✨ What Is This?

An immersive, self-contained web application that teaches children (ages 7–14) about the extraordinary achievements of the Islamic Golden Age (8th–14th century CE) through 139 interactive sections spanning games, quizzes, stories, art tools, language activities, and explorable content.

Everything runs in a single HTML file. No server, no install, no internet required after first load. Just open the file in any modern browser and start exploring.

**New in v1.0:** Full multilingual support — English, French (Français), and Arabic (العربية) with complete RTL layout.

---

## 🚀 Quick Start

```
1. Open  start_here.html  for the welcome page, or
2. Open  index.html  directly to launch the app
3. That's it. Start scrolling and tapping.
```

For classroom use, see [TEACHERS-GUIDE.md](TEACHERS-GUIDE.md).
For parents, see [PARENTS-GUIDE.md](PARENTS-GUIDE.md).
For common questions, see [FAQ.md](FAQ.md).

---

## 📋 System Requirements

| Requirement | Minimum |
|---|---|
| **Browser** | Chrome 80+, Firefox 78+, Safari 14+, Edge 80+ |
| **Device** | Any — desktop, laptop, tablet, phone |
| **Screen** | Responsive from 320px to 4K |
| **Internet** | Only for first load (PWA caches for offline) |
| **Storage** | ~1 MB localStorage for progress/scores |
| **Audio** | Optional — Web Speech API for TTS narration |

---

## 🌐 Multilingual Support

The app supports three languages with a built-in switcher:

| Language | Code | Direction | Coverage |
|---|---|---|---|
| **English** | EN | LTR | Full (default) |
| **French** | FR | LTR | 360+ translated strings |
| **Arabic** | AR | RTL | 360+ translated strings |

**Features:**
- Language switcher button (EN · FR · عربي) always visible
- 137 section titles translated
- 135 section subtitles translated
- Quiz questions, options, and feedback in all 3 languages
- Full RTL CSS layout for Arabic with 23 override rules
- Scholar bios, city descriptions, timeline events translated
- User preference saved to localStorage

---

## 📦 Package Contents

```
builders-of-light-v1.0/
├── start_here.html       ← Welcome page & launcher
├── index.html             ← The app (830 KB, self-contained)
├── README.md              ← This file
├── QUICKSTART.md          ← 30-second setup guide
├── CHANGELOG.md           ← Full version history (v1–v21)
├── TEACHERS-GUIDE.md      ← Classroom activities & lesson plans
├── PARENTS-GUIDE.md       ← Home learning guide
├── FAQ.md                 ← Common questions & answers
└── LICENSE.md             ← License information
```

---

## 📖 Content Overview

### 11 Categories · 139 Sections

| Category | Sections | Highlights |
|---|---|---|
| 📅 **Start Here** | 3 | Daily challenge, word of the day, streaks |
| 📖 **Stories** | 7 | Time-travel to Baghdad 830 CE, scholar diaries, daily routines |
| 🧑‍🏫 **Scholars** | 8 | 15+ scholar bios, women of knowledge, report cards, connections |
| 🏙️ **Places** | 7 | Interactive city map, trade routes, Silk Road adventure, seafaring |
| 🔬 **Science** | 18 | 8 knowledge fields with interactive demos, inventions gallery |
| 🎨 **Arts** | 12 | Calligraphy, geometric patterns, music, architecture, coloring |
| 🔤 **Language** | 12 | Arabic alphabet, vocabulary, pronunciation, glossary, deep dives |
| 🎮 **Games** | 35 | Crossword, Wordle, memory, Jeopardy, word search, mazes, 25+ more |
| 🕌 **Faith** | 8 | Hadith cards, Quran recitation, duas, pledge wall, values |
| 📊 **Progress** | 15 | Dashboard, badges, trading cards, leaderboard, certificate |
| 🏆 **Completion** | 14 | Final quiz, awards ceremony, reading list, encyclopedia |

### Interactive Features

- 🌟 **Stars System** — Earn stars for completing activities
- 🏅 **30+ Achievement Badges** — Auto-awarded for milestones
- 📊 **Progress Dashboard** — Visual tracking of all sections
- 🎓 **Personalized Certificate** — Generated on completion
- 🔊 **Text-to-Speech** — Narration in English and Arabic
- 🎤 **Voice Input** — Speak answers to quizzes
- 🔥 **Daily Streaks** — Come back each day for new content
- ⌨️ **Keyboard Shortcuts** — Power-user navigation
- 🌙 **Konami Code** — Hidden easter egg!
- 📱 **PWA** — Install as app, works offline

---

## 🏗️ Technical Architecture

### Single-File Design
Everything — HTML, CSS, JavaScript, data, translations — lives in one 830 KB file. No build tools, no bundlers, no frameworks.

### Key Systems
- **i18n Engine**: `t()`, `tl()`, `tsub()`, `tst()` translation functions
- **TR Dictionary**: 360+ string-based content translations
- **UI Dictionary**: 200+ keyed UI translations
- **RTL Engine**: 23 CSS override rules, automatic `dir="rtl"` switching
- **Progress System**: localStorage-based with star tracking
- **PWA**: Service worker for offline capability
- **SFX Engine**: Web Audio API sound effects
- **TTS/STT**: Web Speech API for narration and voice input

### Build History
21 development versions from blank file to complete app:

| Version | Milestone |
|---|---|
| v1–v4 | Foundation, math, medicine, astronomy, optics, geography, chemistry, engineering, books |
| v5–v8 | Games engine, crossword, memory, speed challenges, word games |
| v9–v12 | Art tools, calligraphy, patterns, music, Jeopardy, trump cards |
| v13–v16 | Language section, Arabic alphabet, pronunciation, deep dives |
| v17–v18 | Progress system, badges, dashboard, certificate, leaderboard |
| v19–v20 | Navigation, PWA, keyboard shortcuts, sound effects, polish |
| v21 | Full multilingual system — EN/FR/AR with RTL |

---

## 🎯 Educational Standards Alignment

Covers elements of:
- **History**: Medieval Islamic civilization, comparative timelines
- **Science**: Scientific method, optics, astronomy, chemistry, medicine
- **Mathematics**: Algebra, algorithms, number systems, geometry
- **Geography**: World maps, trade routes, navigation
- **Language Arts**: Arabic loanwords, etymology, vocabulary
- **Art**: Geometric patterns, calligraphy, architecture
- **Technology**: Engineering, inventions, innovation

---

## 📄 License

This project is provided for educational use. See [LICENSE.md](LICENSE.md) for details.

---

<p align="center">
🌙 Made with ❤️ and Bismillah
</p>

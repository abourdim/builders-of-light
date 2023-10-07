# 👩‍🏫 Teacher's Guide

**Version 1.0** · 830 KB · 139 sections · 3 languages

## Overview

*Builders of Light* is designed for use in Islamic schools, supplementary weekend schools, home education, and as enrichment material in mainstream education. It covers Key Stage 2–3 (ages 7–14) and touches on History, Science, Mathematics, Geography, Art, Religious Studies, and English/Literacy.


---

## 🌐 Language Support

The app supports **English, French, and Arabic** with a built-in language switcher.

### In the Classroom
- **Multilingual classrooms**: Students can each use their preferred language independently
- **Arabic schools**: Switch to Arabic for full RTL layout with translated content
- **French immersion**: Use the French mode for francophone students
- **Language comparison**: Use the switcher to show how the same content appears in different languages — great for language arts

### How to Switch
Click the **EN · FR · عربي** button in the top-right corner (bottom-center on mobile). The choice is saved per browser.

---

## Classroom Setup

### Option 1: Individual Devices
Each student opens the HTML file on their own device (laptop, tablet, Chromebook). The app is self-paced and self-contained.

### Option 2: Shared Screen
Project on a whiteboard or TV. Use the **nav drawer** (☰) to jump between sections. Good for whole-class teaching.

### Option 3: Offline / No WiFi
Load the file once on each device while connected. The **Service Worker** caches everything. After that, no internet is needed. Perfect for schools with limited WiFi.

### Option 4: School Network
Place the HTML file on your school's shared drive or intranet server. Students access it via browser. No installation required.

---

## Curriculum Alignment

### Religious Studies / Islamic Studies
- **Foundation** — "Iqra" and the Quranic emphasis on knowledge
- **Hadith Cards** — Authentic sayings about seeking knowledge
- **Duas** — Supplications for learning
- **Scholar Pledge** — Personal commitment to education
- **Recitation** — Quran recitation practice

### History
- **Timeline** (750–1258 CE) — Key dates and events
- **Story Mode** — Narrative journey through Golden Age Baghdad
- **Two Worlds** — Compare Islamic civilisation with medieval Europe
- **True Scale** — Data-driven comparisons (books, hospitals, cities)
- **Time Traveller** — Choose-your-own-adventure in 950 CE

### Science
- **Experiments** — Recreate Golden Age experiments
- **Inventions Gallery** — 12 key inventions with full context
- **Invention Lab** — Build virtual inventions
- **Water Engineering** — Qanat systems
- **Optics, Medicine, Chemistry** — Covered across multiple sections

### Mathematics
- **Math Challenge** — Al-Khwarizmi's algebra
- **Number Bonds** — Practice with Arabic numerals
- **Numbers** — History of the numeral system and zero
- **Number Showdown** — Scale and magnitude comparisons

### Geography
- **Map Quiz** — Locate Golden Age cities
- **Silk Road Adventure** — Travel the ancient trade routes
- **Trade Routes** — How knowledge spread globally
- **Cities** — Baghdad, Córdoba, Cairo, Fez, Damascus, Isfahan

### Art & Design
- **Calligraphy** — Interactive Arabic letter drawing
- **Pattern Builder** — Create geometric Islamic designs
- **Colouring** — Islamic geometric templates
- **Architecture** — Mosque design and geometry
- **Art Gallery** — Islamic art appreciation

### English / Literacy
- **Word Roots** — Arabic origins of English words
- **Glossary / Encyclopedia** — Reference skills
- **Quote Builder** — Sentence reconstruction
- **Fill the Gaps** — Cloze comprehension
- **Word Search / Crossword / Wordle** — Vocabulary building

---

## Suggested Lesson Plans

### Lesson 1: Introduction (45 min)
1. **Foundation** (5 min) — Discuss "Iqra" and why knowledge matters in Islam
2. **Timeline** (10 min) — Overview of the Golden Age period
3. **Story Mode** (15 min) — Walk through a day in Baghdad together
4. **Scholar Profiles** (10 min) — Each student picks a scholar to present
5. **Reflection** (5 min) — Students record what surprised them most

### Lesson 2: Science & Invention (45 min)
1. **Inventions Gallery** (10 min) — Explore all 12 inventions
2. **Experiments** (15 min) — Try 2-3 virtual experiments
3. **True Scale** (5 min) — Compare Muslim world vs Europe
4. **Number Showdown** (5 min) — Quick competitive quiz
5. **Legacy Letter** (10 min) — Write to a scholar thanking them

### Lesson 3: Language & Culture (45 min)
1. **Arabic Alphabet** (10 min) — Practice letters
2. **Calligraphy** (10 min) — Draw "Bismillah"
3. **Word Roots** (10 min) — Discover English words from Arabic
4. **Music & Sound** (5 min) — Learn about Islamic instruments
5. **Poetry** (10 min) — Read and discuss Golden Age poems

### Lesson 4: Assessment & Celebration (45 min)
1. **Final Quiz** (15 min) — Comprehensive assessment
2. **Scavenger Hunt** (10 min) — Find items across the app
3. **Scholar Awards** (5 min) — Vote for favourite scholars
4. **Certificate** (5 min) — Print completion certificates
5. **Share** (10 min) — Students share their favourite discoveries

---

## Differentiation

### Lower Ability / Younger Students
- Focus on visual/interactive sections: Memory Game, Colouring, Sound Board, Lucky Dip
- Use Story Mode and Scholar Diary for accessible narratives
- Enable TTS narration (sound on) for reading support
- Start with Easy difficulty in the Final Quiz

### Higher Ability / Older Students
- Challenge with: Jeopardy, Countdown Quiz, Speed Typing, Crossword
- Direct to: Philosophy, Knowledge Web, Deep Dive for extended learning
- Use Hard difficulty in the Final Quiz
- Encourage the Silk Road Adventure and Time Traveller for critical thinking

### EAL / Bilingual Students
- Sound Board and Pronunciation sections support Arabic learners
- Vocab Flashcards provide bilingual vocabulary
- Translation Race and Translation Match build bridging skills

---

## Assessment Opportunities

| Activity | Assessment Type |
|---|---|
| Final Quiz | Summative (easy/medium/hard) |
| Dashboard | Formative (progress tracking) |
| Reflection | Self-assessment (voice recording) |
| Scholar Awards | Peer assessment / opinion forming |
| Legacy Letter | Extended writing |
| Certificate | Completion evidence |
| Countdown Quiz | Timed recall |
| Sequence Challenge | Ordering / comprehension |

---

## Progress Tracking

Student progress is saved to **localStorage** on each device:
- ⭐ Total stars earned
- 🔥 Daily challenge streak
- 🏆 Personal best scores (quiz, countdown, typing WPM)
- ✅ Completed sections

**Note:** Progress is per-device, not per-student. If students share devices, their scores will merge. For individual tracking, assign one device per student or have students note their star count at the end of each session.

---

## Pastoral Notes

- The app includes **Islamic content** (Quran references, hadith, duas, Prophet Muhammad ﷺ) presented in an educational context
- All historical claims are **researched for accuracy** with appropriate nuance
- The tone is **celebratory but not supremacist** — it acknowledges that Muslim scholars built on Greek, Indian, Persian, and Chinese knowledge
- **Women scholars** are prominently featured (Fatima al-Fihri, Maryam al-Astrulabiyya, Lubna of Córdoba, Sutayda al-Mahamali)
- The content is suitable for **Muslim and non-Muslim students** alike

---

## Technical Notes for IT Departments

- The app is a **single HTML file** with no server-side components
- It makes **no network requests** except for Google Fonts on first load
- It stores data **only in localStorage** (under keys prefixed `ga_`)
- It registers a **Service Worker** for offline caching (can be blocked if needed)
- It uses **Web Speech API** for TTS (requires browser permission on some systems)
- There are **no tracking scripts, analytics, or third-party resources**
- The file can be placed on any **shared drive, intranet, or LMS**

---

*Questions? See [FAQ.md](FAQ.md) for answers to common queries.*

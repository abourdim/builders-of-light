# ❓ Frequently Asked Questions

**Version 1.0** · 830 KB · 139 sections · 3 languages

---

### General

**Q: What age group is this for?**
A: Primarily ages 7–14, but younger children can enjoy the visual/interactive sections (Memory Game, Colouring, Sound Board, Lucky Dip) and older students can benefit from the depth of content (Philosophy, Knowledge Web, Deep Dive, Silk Road Adventure).

**Q: Is this free to use?**
A: Yes, completely free. MIT licensed. Use it in schools, mosques, homes, or anywhere else.

**Q: Does it work on phones and tablets?**
A: Yes. The app is fully responsive from 320px (small phones) to 4K screens. Touch interactions work throughout. You can even install it as an app via "Add to Home Screen."

**Q: Does it need internet?**
A: Only for the very first load (to cache Google Fonts). After that, the built-in Service Worker keeps everything available offline. Perfect for classrooms with unreliable WiFi.


**Q: What languages does it support?**
A: English (default), French, and Arabic. Click the language switcher button (EN · FR · عربي) in the top corner to switch. Arabic uses full right-to-left layout. Your choice is saved automatically.

**Q: How complete are the translations?**
A: The app has 360+ translated content strings, 200+ UI translations, 137 translated section titles, and 135 translated subtitles. All quizzes, scholar bios, timeline events, and interactive sections are translated. Some niche interactive demos remain in English.

**Q: Does the Arabic mode really go right-to-left?**
A: Yes. The entire layout flips — text alignment, navigation, grids, and reading order all switch to RTL with 23 dedicated CSS rules.

**Q: Can I use this in a non-Muslim school?**
A: Absolutely. The content is educational and historically focused. It celebrates the achievements of Islamic civilisation in a way that's accessible and respectful to all backgrounds. Many sections (science, math, geography, art) are purely secular in content.

---

### Content

**Q: Is the historical content accurate?**
A: Yes. All facts, dates, and attributions are based on mainstream historical scholarship. Where there is scholarly debate (e.g., exact dates, attribution of inventions), we've used the most widely accepted positions.

**Q: Why does it say "ﷺ" after Prophet Muhammad's name?**
A: This is the Arabic honorific "ṣallā Allāhu ʿalayhi wa-sallam" (peace and blessings be upon him), a standard Islamic practice when mentioning the Prophet's name.

**Q: Are the Arabic transliterations accurate?**
A: They follow standard academic transliteration conventions. The Text-to-Speech pronunciation depends on the browser's TTS engine and may vary in accuracy for Arabic words.

**Q: How many scholars are covered?**
A: Over 15 named scholars in depth, including Al-Khwarizmi, Ibn Sina, Ibn al-Haytham, Al-Zahrawi, Al-Jazari, Al-Idrisi, Al-Biruni, Abbas ibn Firnas, Jabir ibn Hayyan, Fatima al-Fihri, Al-Kindi, Al-Farabi, Al-Ghazali, Ibn Rushd, and Ibn Khaldun. Many more are mentioned in context.

**Q: I found an error in the content. How can I report it?**
A: The source code is a single HTML file that can be edited with any text editor. If you find a factual error, search for the text in the file and correct it directly.

---

### Technical

**Q: Why is it one giant HTML file?**
A: By design. A single file means zero setup, zero dependencies, zero server requirements. Copy it to a USB stick, email it, put it on a shared drive — it just works. The 830 KB size is smaller than most web pages with their dozens of external resources.

**Q: Can I edit the content?**
A: Yes. Open the HTML file in any text editor (VS Code, Notepad++, Sublime Text). All data is in JavaScript arrays near the top of the `<script>` section. You can change questions, add scholars, modify text, etc.

**Q: How do I clear saved progress?**
A: Open your browser's developer tools (F12), go to Application → localStorage, and delete all keys starting with `ga_`. Or clear all site data in browser settings.

**Q: The Service Worker is caching an old version. How do I update?**
A: Clear the Service Worker cache: Developer Tools → Application → Service Workers → Unregister. Then reload the page. The new version will re-cache automatically.

**Q: Can I embed this in an LMS (Google Classroom, Moodle, etc.)?**
A: Yes. Upload the HTML file as a resource, or host it on your school's web server and link to it. The file is self-contained and will work in any iframe or direct link.

**Q: Does it work on Chromebooks?**
A: Yes. Chrome on ChromeOS supports all the required APIs (Web Speech, Web Audio, Canvas, Service Workers, localStorage).

**Q: Does it collect any data?**
A: No. Zero tracking, zero analytics, zero network requests (after font loading). All data stays in the user's browser localStorage. No information is transmitted anywhere.

---

### Sound & Speech

**Q: How do I turn off all sounds?**
A: Click the 🔊 icon in the top-right star tracker, or press `M` on your keyboard. The preference is saved.

**Q: The Text-to-Speech sounds robotic / has the wrong accent.**
A: TTS quality depends on your browser and operating system. Chrome on desktop generally sounds best. Mobile voices vary. Arabic pronunciation may not be perfect — it's using the browser's built-in speech synthesis.

**Q: Can I use this with screen readers?**
A: The app includes ARIA labels, roles, and live regions for the major interactive elements. However, due to the visual/interactive nature of many games, some sections work better with sighted use. The text content sections (Story Mode, Scholar Profiles, etc.) are fully accessible.

---

### Games

**Q: How do I play Wordle?**
A: Type 5-letter Golden Age words using your keyboard (A–Z, Enter to submit, Backspace to delete). Green = correct letter/position, Yellow = correct letter/wrong position, Grey = not in the word. You get 6 tries. A hint is shown above.

**Q: The maze doesn't respond to my keys.**
A: The maze responds to arrow keys when the maze section is visible on screen. Scroll to the maze section first, then use arrow keys.

**Q: How do stars work?**
A: Almost every interaction earns a star — answering questions, exploring cards, completing games, listening to audio. Stars are tracked in the top-right corner and saved to localStorage. There's no maximum!

**Q: What triggers confetti?**
A: Getting a high score on games (typically 60–80% or higher), completing explorable collections, finishing adventures, and other significant achievements.

---

### Printing

**Q: How do I print the certificate?**
A: Scroll to the Certificate section (or use nav drawer → Completion → Certificate). Enter the student's name, then click "Print Certificate." The print view hides everything except the certificate.

**Q: Can I print other sections?**
A: The current print stylesheet only supports the certificate. To print other content, you could screenshot sections or use your browser's "Save as PDF" with specific pages selected.

---

### Customisation

**Q: Can I add my own quiz questions?**
A: Yes. Open the HTML file in a text editor. Search for the relevant data array (e.g., `cdQuestions` for countdown quiz, `tfData` for true/false). Add new entries following the same format.

**Q: Can I remove sections I don't need?**
A: Yes. Find the `<section id="...">` block in the HTML and delete it. Also remove its corresponding init call from the `DOMContentLoaded` function. The app will work fine with sections removed.

**Q: Can I change the colours / theme?**
A: Yes. Search for `:root` or `--` in the CSS section. The main colours are defined as CSS custom properties: `--navy`, `--gold`, `--emerald`, `--cream`, `--coral`.

**Q: Can I translate this to another language?**
A: The text is all inline in the HTML and JavaScript. You could search and replace the English text with another language. The Arabic content would remain as-is. A full translation would be a significant effort but is technically straightforward.

---

*Still have questions? The source code is open and readable — search for any text you see on screen to find and modify it.*

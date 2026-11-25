KAWAII VOWEL DINO CLUB — STARTER WEBSITE

This project contains a two-page website:
- index.html: choose an age group and play the daily 10-word speaking game.
- collection.html: dinosaur collection, past exercises, recent-score chart and grown-up progress corner.
- style.css: kawaii pastel theme and responsive layout.
- app.js: age-specific word banks, microphone speech recognition, scoring, rewards and local progress.

RUN IT
1. Download and unzip this folder.
2. Open a terminal in the folder.
3. Run: python3 -m http.server 8000
4. Open http://localhost:8000 in Google Chrome.
5. Allow microphone access. The website uses speech recognition and speech synthesis.

AGE GROUPS
4–5: familiar short-vowel words.
6–7: short/long vowels and common vowel teams.
8–9: vowel teams and diphthongs.
10–12: longer words, syllables and more challenging vowel patterns.
Each session randomly chooses 10 words from that age group's word bank.

REWARDS
10 correct = 3 stars; 9 = 2 stars; 8 = 1 star; 0–7 = 0 stars.
Every time the star total crosses another 50-star milestone, a bonus baby dino is awarded.
90–100% = magical dino (10 unique magical dinos, one per excellent exercise until all are collected).
60–89% = cute baby dino.
0–50% = silly dino.
The requested 51–80% range leaves 81–89% unspecified, so this version treats 60–89% as cute baby dinos and 0–50% as silly dinos. If you prefer exact thresholds, change them in finish() in app.js.

IMPORTANT LIMITATIONS
This is a learning-game prototype, not a professional pronunciation assessment. Browser speech recognition checks whether it recognises the target word as text; it cannot reliably assess accent, articulation or whether the vowel sound is produced correctly. Speech recognition varies by browser, device and language and may need an internet connection. Test with an adult before classroom use.
The microphone audio is not recorded or stored by this code. The game stores only age choice, score history, stars and dinosaur collection in localStorage on that device/browser. Clearing browser data removes it. It is not a secure teacher account or cloud sync.
A child should use the microphone with a parent/teacher's permission. Use a secure HTTPS host or localhost for microphone access.
The font is loaded from Google Fonts; if offline, a system font is used instead.

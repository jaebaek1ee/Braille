# Korean Braille Learning App (점자 학습)

A Progressive Web App (PWA) for learning Korean Braille (한글 점자), built as a single HTML file with React.

## Overview

This app was created to help my parents learn Korean Braille for teaching visually impaired students. It covers the complete Korean Braille system based on the **2017 Revised Korean Braille Standard** (한국 점자 규정).

## Features

### Jamo Tab (자모)
- **6 categories**: Chosung (초성, 14), Moeum (모음, 17), Jongsung (종성, 14), Abbreviations (약자, 11), Double consonants (쌍자음, 5), Abbreviated words (약어, 7)
- **Left = Hangul / Right = Braille** layout with interactive 6-dot cell visualization
- **Hide/Reveal toggle**: Hide Hangul or Braille side, tap individual items to reveal
- **Combined Quiz (종합 퀴즈)**: Mix all categories with adjustable question count

### Quiz Modes (3 types)
1. **Braille → Hangul** (4-choice multiple choice)
2. **Hangul → Braille** (4-choice multiple choice)
3. **Direct Dot Input** ✍️ — Tap the 6 dots to build the braille pattern, then submit
- Wrong answers are re-added to the deck and repeated until correct

### Word Tab (단어)
- 70 everyday Korean words with full braille breakdown
- Tap any word to see syllable-by-syllable decomposition (초성+중성+종성 → braille cells)
- Hide/Reveal toggle for self-testing
- Word quiz with adjustable count (10/20/30/50)

### Settings Tab (설정)
- Braille structure guide (6-dot numbering system)
- Recommended learning order
- Key rules summary
- Usage instructions

## Braille Data Accuracy

All braille dot patterns have been verified against:
- [Korean Braille Standard (한국 점자 규정)](https://www.korean.go.kr/front/page/pageView.do?page_id=P000302&mn_id=205)
- [delvier/hanbraille](https://github.com/delvier/hanbraille) — verified open-source Korean Braille converter
- [hi098123 Braille Translator](https://t.hi098123.com/braille)

### Covered patterns
| Category | Count | Description |
|----------|-------|-------------|
| Chosung (초성) | 14 | Initial consonants |
| Moeum (모음) | 17 | Vowels (including compound: ㅘ,ㅚ,ㅝ,ㅢ) |
| Jongsung (종성) | 14 | Final consonants (batchim) |
| Yakja (약자) | 11 | Syllable abbreviations (가,사,나,다,...) |
| Ssang (쌍자음) | 5 | Double consonants (ㄲ,ㄸ,ㅃ,ㅆ,ㅉ) |
| Yakyeo (약어) | 7 | Word abbreviations (그래서,그러나,...) |

## Tech Stack

- **React 18** + Babel (in-browser JSX compilation)
- **Single HTML file** — no build step, no server required
- **PWA-ready** — add to home screen on mobile for app-like experience
- **localStorage-free** — all data is embedded, no external dependencies

## Installation

### Option 1: GitHub Pages (Recommended)
1. Fork or clone this repository
2. Enable GitHub Pages in Settings → Pages → Deploy from `main` branch
3. Access at `https://<username>.github.io/<repo-name>/`

### Option 2: Local
Simply open `index.html` in any modern browser (Chrome recommended).

### Mobile (Add to Home Screen)
1. Open the URL in Chrome (Android) or Safari (iOS)
2. Tap ⋮ → "Add to Home Screen"
3. The app will launch without the browser address bar

## License

MIT

## Acknowledgments

- Korean Braille standard by [National Institute of Korean Language](https://korean.go.kr)
- Original system: 훈맹정음 (1926) by Park Du-seong (박두성)

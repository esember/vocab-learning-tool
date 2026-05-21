# Vocabulary Learning Tool

> Interactive flashcard app for learning the 2,000 most frequently used B2 & C1 level English words — with text-to-speech, auto-timer, and level filtering.

🌐 **Live Demo:** [mekazek.com/english](https://mekazek.com/english)

---

## Features

| Feature | Description |
|---|---|
| 📚 **1,816 Words** | Curated B2 & C1 vocabulary with Turkish meanings |
| 🔊 **Text-to-Speech** | Listen to the word, definition, and example sentences |
| ⏱️ **Auto-Timer** | Auto-advance cards every 5–60 seconds |
| 🔤 **Alphabetical Index** | Jump to any letter instantly |
| 📊 **Level Filter** | Study B2 or C1 words separately |
| 🌍 **Bilingual** | Turkish meaning shown alongside English word |
| 📱 **Responsive** | Works on mobile and desktop |

## Screenshot

![Vocabulary Learning Tool](https://mekazek.com/english)

## Usage

Simply open `index.html` in any modern browser — no build step, no dependencies.

```bash
git clone https://github.com/esember/vocab-learning-tool.git
cd vocab-learning-tool
open index.html   # or double-click
```

Or visit the live version: **[mekazek.com/english](https://mekazek.com/english)**

## Word Data Format

Each entry in `words.js` follows this structure:

```js
{
  word: "abolish",
  level: "C1",          // A1 / A2 / B1 / B2 / C1 / C2
  type: "v.",           // part of speech
  turkish: "Kaldırmak, feshetmek",
  definition: "To formally put an end to a system, practice, or institution.",
  examples: [
    "Many people campaigned to abolish slavery during the 19th century.",
    "The government decided to abolish the unpopular tax."
  ]
}
```

## Read Modes

The **Read** button cycles through 4 modes:

1. **Read: Word + Meaning** — speaks the English word, then Turkish meaning
2. **Read: Definition** — speaks the English definition
3. **Silent Mode** — no auto-speech
4. **Read: Everything** — full sequence: word → meaning → definition → examples

## Tech Stack

- **Vanilla JavaScript** — no frameworks
- **Tailwind CSS** (CDN) — utility-first styling
- **Web Speech API** — native browser TTS

## License

[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) — Free to use, fork, and adapt **with attribution**.

If you use this project or build upon it, please credit the original author:
> Built by [Gursel Olca](https://github.com/esember) — [mekazek.com/english](https://mekazek.com/english)

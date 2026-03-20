# Covenant — Vocabulary-Immersion Reading App

> **Read. Listen. Track your vocabulary. Build fluency.**

Covenant is an all-in-one reader that turns plain text books and EPUB files into active vocabulary-learning sessions. Upload your book, load your vocabulary CSV, and every word in your deck is highlighted as you read — with level tracking, spaced-repetition study, connected-speech analysis, and detailed statistics.

---

## Table of Contents

1. [Getting Started](#getting-started)
2. [Portal — Choosing Your Tool](#portal--choosing-your-tool)
3. [Library — Managing Books](#library--managing-books)
4. [Upload & Vocabulary CSV](#upload--vocabulary-csv)
5. [The Reader](#the-reader)
   - [Vocabulary Highlights](#vocabulary-highlights)
   - [The Tooltip](#the-tooltip)
   - [Word Levels (L1–L5)](#word-levels-l1l5)
   - [Audio Player & Bookmarks](#audio-player--bookmarks)
   - [Difficulty Badge](#difficulty-badge)
   - [Unique Words Sidebar](#unique-words-sidebar)
   - [Highlights Panel](#highlights-panel)
   - [Rules Panel](#rules-panel)
   - [Dictionary Lookup](#dictionary-lookup)
   - [Word Peek](#word-peek)
   - [Keyboard Shortcuts](#keyboard-shortcuts)
6. [VocabForge — Spaced Repetition Study](#vocabforge--spaced-repetition-study)
7. [My Vocabulary](#my-vocabulary)
   - [Weak Words](#weak-words)
   - [Focus Words](#focus-words)
   - [Words Mining](#words-mining)
   - [Mastered Words](#mastered-words)
   - [Connected Speech Rules](#connected-speech-rules)
8. [Core Tab — Settings & Backup](#core-tab--settings--backup)
9. [Reader Settings](#reader-settings)
   - [Themes](#themes)
   - [Fonts](#fonts)
   - [Connected Speech Mode](#connected-speech-mode)
   - [Ignored Words CSV](#ignored-words-csv)
10. [Session Stats](#session-stats)
11. [Data & Privacy](#data--privacy)
12. [Keyboard Shortcuts Reference](#keyboard-shortcuts-reference)

---

## Getting Started

Covenant runs entirely in your browser — no account, no server, no install.

```
1. Open index.html in any modern browser
2. Click "Covenant Reader" on the portal
3. Upload an EPUB or .txt file under the Upload tab
4. (Optional) Upload a vocabulary CSV
5. Open the book from your Library and start reading
```

```svg
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 700 120" font-family="'DM Sans',sans-serif">
  <rect width="700" height="120" rx="12" fill="#161616" stroke="#242424" stroke-width="1"/>
  <!-- Steps -->
  <g fill="none">
    <!-- Step 1 -->
    <circle cx="60" cy="60" r="26" fill="#1c1c1c" stroke="#e8365d" stroke-width="1.5"/>
    <text x="60" y="56" text-anchor="middle" fill="#e8365d" font-size="18" font-weight="700">1</text>
    <text x="60" y="98" text-anchor="middle" fill="#888" font-size="11">Open App</text>
    <!-- Arrow -->
    <line x1="90" y1="60" x2="118" y2="60" stroke="#333" stroke-width="1.5" stroke-dasharray="3,2"/>
    <polygon points="118,55 128,60 118,65" fill="#333"/>
    <!-- Step 2 -->
    <circle cx="158" cy="60" r="26" fill="#1c1c1c" stroke="#555" stroke-width="1.5"/>
    <text x="158" y="56" text-anchor="middle" fill="#e2e2e2" font-size="18" font-weight="700">2</text>
    <text x="158" y="98" text-anchor="middle" fill="#888" font-size="11">Upload Book</text>
    <!-- Arrow -->
    <line x1="188" y1="60" x2="216" y2="60" stroke="#333" stroke-width="1.5" stroke-dasharray="3,2"/>
    <polygon points="216,55 226,60 216,65" fill="#333"/>
    <!-- Step 3 -->
    <circle cx="256" cy="60" r="26" fill="#1c1c1c" stroke="#555" stroke-width="1.5"/>
    <text x="256" y="56" text-anchor="middle" fill="#e2e2e2" font-size="18" font-weight="700">3</text>
    <text x="256" y="98" text-anchor="middle" fill="#888" font-size="11">Upload CSV</text>
    <!-- Arrow -->
    <line x1="286" y1="60" x2="314" y2="60" stroke="#333" stroke-width="1.5" stroke-dasharray="3,2"/>
    <polygon points="314,55 324,60 314,65" fill="#333"/>
    <!-- Step 4 -->
    <circle cx="354" cy="60" r="26" fill="#1c1c1c" stroke="#555" stroke-width="1.5"/>
    <text x="354" y="56" text-anchor="middle" fill="#e2e2e2" font-size="18" font-weight="700">4</text>
    <text x="354" y="98" text-anchor="middle" fill="#888" font-size="11">Open Book</text>
    <!-- Arrow -->
    <line x1="384" y1="60" x2="412" y2="60" stroke="#333" stroke-width="1.5" stroke-dasharray="3,2"/>
    <polygon points="412,55 422,60 412,65" fill="#333"/>
    <!-- Step 5 -->
    <circle cx="452" cy="60" r="26" fill="#1c1c1c" stroke="#555" stroke-width="1.5"/>
    <text x="452" y="56" text-anchor="middle" fill="#e2e2e2" font-size="18" font-weight="700">5</text>
    <text x="452" y="98" text-anchor="middle" fill="#888" font-size="11">Read &amp; Study</text>
    <!-- Arrow -->
    <line x1="482" y1="60" x2="510" y2="60" stroke="#333" stroke-width="1.5" stroke-dasharray="3,2"/>
    <polygon points="510,55 520,60 510,65" fill="#333"/>
    <!-- Step 6 -->
    <circle cx="560" cy="60" r="26" fill="#e8365d" stroke="#e8365d" stroke-width="1.5"/>
    <text x="560" y="56" text-anchor="middle" fill="white" font-size="18" font-weight="700">✓</text>
    <text x="560" y="98" text-anchor="middle" fill="#4ade80" font-size="11">Level Up!</text>
  </g>
</svg>
```

---

## Portal — Choosing Your Tool

When you first open Covenant you land on the **Portal**, a launcher with three tools:

```svg
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 700 200" font-family="'DM Sans',sans-serif">
  <rect width="700" height="200" rx="12" fill="#0e0e0e" stroke="#242424"/>
  <text x="350" y="36" text-anchor="middle" fill="#e2e2e2" font-size="20" font-weight="700" font-style="italic">Cov</text>
  <text x="350" y="36" text-anchor="middle" fill="#e2e2e2" font-size="20" font-weight="700" dx="22">enant</text>
  <text x="350" y="36" text-anchor="middle" fill="#e8365d" font-size="20" font-weight="700" dx="-8">enant</text>
  <!-- Reader Card -->
  <rect x="40" y="60" width="180" height="120" rx="12" fill="#161616" stroke="#e8365d" stroke-width="1.5"/>
  <rect x="56" y="78" width="32" height="32" rx="8" fill="rgba(232,54,93,0.12)" stroke="rgba(232,54,93,0.3)"/>
  <text x="72" y="100" text-anchor="middle" fill="#e8365d" font-size="16">📖</text>
  <text x="130" y="132" text-anchor="middle" fill="#e2e2e2" font-size="13" font-weight="600">Covenant Reader</text>
  <text x="130" y="150" text-anchor="middle" fill="#555" font-size="10">Upload a book &amp; audio,</text>
  <text x="130" y="163" text-anchor="middle" fill="#555" font-size="10">read with vocab tracking</text>
  <!-- Shadow Card -->
  <rect x="260" y="60" width="180" height="120" rx="12" fill="#161616" stroke="#242424" stroke-width="1"/>
  <rect x="276" y="78" width="32" height="32" rx="8" fill="#1c1c1c" stroke="#242424"/>
  <text x="292" y="100" text-anchor="middle" fill="#888" font-size="16">🎙</text>
  <text x="350" y="132" text-anchor="middle" fill="#e2e2e2" font-size="13" font-weight="600">Shadow</text>
  <text x="350" y="150" text-anchor="middle" fill="#555" font-size="10">Shadowing practice —</text>
  <text x="350" y="163" text-anchor="middle" fill="#555" font-size="10">listen, repeat, internalize</text>
  <!-- Roadmap Card -->
  <rect x="480" y="60" width="180" height="120" rx="12" fill="#161616" stroke="#242424" stroke-width="1"/>
  <rect x="496" y="78" width="32" height="32" rx="8" fill="#1c1c1c" stroke="#242424"/>
  <text x="512" y="100" text-anchor="middle" fill="#888" font-size="16">🗺</text>
  <text x="570" y="132" text-anchor="middle" fill="#e2e2e2" font-size="13" font-weight="600">Roadmap</text>
  <text x="570" y="150" text-anchor="middle" fill="#555" font-size="10">Structured learning paths</text>
  <text x="570" y="163" text-anchor="middle" fill="#555" font-size="10">per language</text>
</svg>
```

| Tool | What it does |
|------|-------------|
| **Covenant Reader** | Upload a book (EPUB / TXT) and optional audio. Read with full vocabulary tracking, highlights, tooltips, and SRS study. |
| **Shadow** | Shadowing mode — listen to a recording and repeat to internalize natural speech patterns. |
| **Roadmap** | Structured learning paths by language. English is available; Japanese and Spanish are coming soon. |

---

## Library — Managing Books

The **Library** tab shows all books you've imported. Each card shows the title, cover (auto-extracted from EPUB), chapter count, and audio status.

```svg
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 700 170" font-family="'DM Sans',sans-serif">
  <rect width="700" height="170" rx="10" fill="#161616" stroke="#242424"/>
  <!-- Tab bar -->
  <rect width="700" height="40" rx="10" fill="#161616" stroke="none"/>
  <rect y="30" width="700" height="10" fill="#161616"/>
  <rect y="39" width="700" height="1" fill="#242424"/>
  <text x="24" y="26" fill="#e8365d" font-size="12" font-weight="700">Library</text>
  <rect x="0" y="37" width="52" height="2" fill="#e8365d" rx="1"/>
  <text x="82" y="26" fill="#555" font-size="12">Upload</text>
  <text x="140" y="26" fill="#555" font-size="12">VocabForge</text>
  <text x="222" y="26" fill="#555" font-size="12">My Vocab</text>
  <!-- Book cards -->
  <rect x="20" y="55" width="100" height="100" rx="8" fill="#1c1c1c" stroke="#2e2e2e"/>
  <rect x="22" y="57" width="96" height="70" rx="6" fill="#242424"/>
  <text x="70" y="97" text-anchor="middle" fill="#555" font-size="22">📗</text>
  <text x="70" y="140" text-anchor="middle" fill="#e2e2e2" font-size="9" font-weight="600">My Book</text>
  <text x="70" y="152" text-anchor="middle" fill="#555" font-size="8">24 chapters</text>
  <!-- audio badge -->
  <rect x="100" y="58" width="18" height="14" rx="3" fill="#2a8a4a"/>
  <text x="109" y="69" text-anchor="middle" fill="white" font-size="8">♪</text>

  <rect x="136" y="55" width="100" height="100" rx="8" fill="#1c1c1c" stroke="#2e2e2e"/>
  <rect x="138" y="57" width="96" height="70" rx="6" fill="#242424"/>
  <text x="186" y="97" text-anchor="middle" fill="#555" font-size="22">📘</text>
  <text x="186" y="140" text-anchor="middle" fill="#e2e2e2" font-size="9" font-weight="600">Another Book</text>
  <text x="186" y="152" text-anchor="middle" fill="#555" font-size="8">12 chapters</text>

  <rect x="252" y="55" width="100" height="100" rx="8" fill="#1c1c1c" stroke="#2e2e2e"/>
  <rect x="254" y="57" width="96" height="70" rx="6" fill="#242424"/>
  <text x="302" y="97" text-anchor="middle" fill="#555" font-size="22">📙</text>
  <text x="302" y="140" text-anchor="middle" fill="#e2e2e2" font-size="9" font-weight="600">Third Book</text>
  <text x="302" y="152" text-anchor="middle" fill="#555" font-size="8">8 chapters</text>

  <!-- Actions legend -->
  <rect x="420" y="60" width="260" height="100" rx="8" fill="#1c1c1c" stroke="#2e2e2e"/>
  <text x="435" y="80" fill="#888" font-size="11" font-weight="600">Card actions</text>
  <text x="435" y="100" fill="#555" font-size="10">▶  Open &amp; read</text>
  <text x="435" y="116" fill="#555" font-size="10">♪  Link / replace audio</text>
  <text x="435" y="132" fill="#555" font-size="10">📦  Archive (hide from library)</text>
  <text x="435" y="148" fill="#555" font-size="10">✕  Delete permanently</text>
</svg>
```

**Actions per book:**
- **Click** — open the book in the reader
- **♪ Link Audio** — attach an audio file (MP3, AAC, etc.) that persists across sessions
- **Archive** — hide a book without deleting it (visible in the Archive tab)
- **Delete** — permanently remove the book and its audio

---

## Upload & Vocabulary CSV

The **Upload** tab is where you bring content into Covenant.

### Book Upload (EPUB / TXT)
Drag and drop — or click to browse — an `.epub` or `.txt` file. EPUB covers, chapter structure, and metadata are extracted automatically.

### Vocabulary CSV

A vocabulary CSV is the heart of Covenant's highlight system. Each row is one word entry:

```
word,pronunciation,definition,pos,synonyms,antonyms
ephemeral,/ɪˈfɛmərəl/,lasting for a very short time,adj,fleeting,permanent
```

| Column | Required | Description |
|--------|----------|-------------|
| `word` | ✅ | The target word or phrase |
| `pronunciation` | optional | IPA or phonetic reading |
| `definition` | optional | Shown in the tooltip |
| `pos` | optional | Part of speech |
| `synonyms` | optional | Comma-separated synonyms |
| `antonyms` | optional | Comma-separated antonyms |

You can load **multiple CSV sets** simultaneously — each gets a different colour dot. Sets can be downloaded as CSV or removed at any time.

```svg
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 700 130" font-family="'DM Sans',sans-serif">
  <rect width="700" height="130" rx="10" fill="#161616" stroke="#242424"/>
  <text x="24" y="28" fill="#888" font-size="11" font-weight="700" letter-spacing="1">VOCABULARY SETS LOADED</text>
  <!-- Set chips -->
  <rect x="20" y="44" width="150" height="32" rx="8" fill="#1c1c1c" stroke="#2e2e2e"/>
  <circle cx="38" cy="60" r="5" fill="#e8365d"/>
  <text x="50" y="64" fill="#e2e2e2" font-size="12">vocab-n3.csv</text>
  <text x="140" y="64" fill="#555" font-size="10">842</text>

  <rect x="182" y="44" width="155" height="32" rx="8" fill="#1c1c1c" stroke="#2e2e2e"/>
  <circle cx="200" cy="60" r="5" fill="#7b9ef0"/>
  <text x="212" y="64" fill="#e2e2e2" font-size="12">freq-5000.csv</text>
  <text x="307" y="64" fill="#555" font-size="10">4,998</text>

  <rect x="349" y="44" width="140" height="32" rx="8" fill="#1c1c1c" stroke="#2e2e2e"/>
  <circle cx="367" cy="60" r="5" fill="#4ade80"/>
  <text x="379" y="64" fill="#e2e2e2" font-size="12">custom.csv</text>
  <text x="459" y="64" fill="#555" font-size="10">128</text>

  <!-- Upload drop zone -->
  <rect x="20" y="88" width="660" height="32" rx="8" fill="rgba(232,54,93,0.05)" stroke="rgba(232,54,93,0.2)" stroke-dasharray="4,3"/>
  <text x="350" y="109" text-anchor="middle" fill="#555" font-size="12">⬆  Drop a CSV here or click to browse</text>
</svg>
```

---

## The Reader

The reader is the main workspace. It shows the chapter text with highlighted vocabulary, a chapter list sidebar on the left, and optional panels on the right.

```svg
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 700 380" font-family="'DM Sans',sans-serif">
  <rect width="700" height="380" rx="10" fill="#0e0e0e" stroke="#242424"/>
  <!-- Top bar -->
  <rect width="700" height="42" rx="0" fill="#161616" stroke="none"/>
  <rect y="41" width="700" height="1" fill="#242424"/>
  <text x="16" y="26" fill="#555" font-size="11">← Back</text>
  <text x="280" y="26" fill="#e2e2e2" font-size="12" font-weight="600">Chapter 4 — The Journey</text>
  <text x="520" y="26" fill="#555" font-size="10">Unique</text>
  <text x="565" y="26" fill="#555" font-size="10">Highlights</text>
  <text x="618" y="26" fill="#555" font-size="10">Rules</text>
  <text x="661" y="26" fill="#555" font-size="10">⚙</text>

  <!-- Chapter sidebar -->
  <rect x="0" y="42" width="200" height="338" fill="#161616" stroke="none"/>
  <rect x="199" y="42" width="1" height="338" fill="#242424"/>
  <text x="16" y="68" fill="#555" font-size="10" font-weight="700" letter-spacing="1">CHAPTERS</text>
  <text x="16" y="90" fill="#555" font-size="11">1 — Prologue</text>
  <text x="16" y="108" fill="#555" font-size="11">2 — Awakening</text>
  <text x="16" y="126" fill="#555" font-size="11">3 — The Call</text>
  <rect x="0" y="134" width="200" height="20" fill="rgba(232,54,93,0.06)"/>
  <rect x="0" y="134" width="2" height="20" fill="#e8365d"/>
  <text x="16" y="148" fill="#e2e2e2" font-size="11" font-weight="600">4 — The Journey</text>
  <text x="16" y="166" fill="#555" font-size="11">5 — Arrival</text>

  <!-- Main reading area -->
  <text x="260" y="80" fill="#888" font-size="10" font-weight="700" letter-spacing="1">CHAPTER 4 — THE JOURNEY</text>
  <rect x="220" y="88" width="340" height="1" fill="#2e2e2e"/>

  <!-- Paragraph with highlights -->
  <text x="220" y="116" fill="#c8c8c8" font-size="13">She walked with </text>
  <!-- L1 highlight: ephemeral -->
  <rect x="343" y="103" width="72" height="18" rx="3" fill="rgba(248,113,113,0.3)"/>
  <text x="343" y="116" fill="#f87171" font-size="13">ephemeral</text>
  <text x="418" y="116" fill="#c8c8c8" font-size="13"> grace,</text>
  <text x="220" y="136" fill="#c8c8c8" font-size="13">her steps </text>
  <!-- L3 highlight -->
  <rect x="295" y="123" width="58" height="18" rx="3" fill="rgba(250,204,21,0.2)"/>
  <text x="295" y="136" fill="#facc15" font-size="13">fleeting</text>
  <text x="356" y="136" fill="#c8c8c8" font-size="13"> as dusk.</text>
  <text x="220" y="156" fill="#c8c8c8" font-size="13">The world felt </text>
  <!-- L4 highlight -->
  <rect x="322" y="143" width="64" height="18" rx="3" fill="rgba(74,222,128,0.15)"/>
  <text x="322" y="156" fill="#4ade80" font-size="13">serene</text>
  <text x="389" y="156" fill="#c8c8c8" font-size="13"> yet strange.</text>

  <!-- Difficulty badge -->
  <rect x="614" y="290" width="68" height="30" rx="10" fill="#0f172a" stroke="rgba(255,255,255,0.1)"/>
  <circle cx="626" cy="305" r="5" fill="#facc15"/>
  <text x="635" y="309" fill="#facc15" font-size="11" font-weight="700">78%</text>
  <text x="655" y="309" fill="#64748b" font-size="9">Optimal</text>

  <!-- Legend -->
  <rect x="220" y="340" width="340" height="26" rx="5" fill="#161616" stroke="#2e2e2e"/>
  <circle cx="234" cy="353" r="5" fill="rgba(248,113,113,0.4)"/>
  <text x="244" y="357" fill="#888" font-size="9">L1 New</text>
  <circle cx="288" cy="353" r="5" fill="rgba(250,204,21,0.3)"/>
  <text x="298" y="357" fill="#888" font-size="9">L3 Partial</text>
  <circle cx="348" cy="353" r="5" fill="rgba(74,222,128,0.3)"/>
  <text x="358" y="357" fill="#888" font-size="9">L4 Known</text>
  <circle cx="402" cy="353" r="5" fill="rgba(74,222,128,0.08)"/>
  <text x="412" y="357" fill="#888" font-size="9">L5 Mastered</text>
  <circle cx="467" cy="353" r="5" fill="rgba(255,255,255,0.06)"/>
  <text x="477" y="357" fill="#888" font-size="9">Ignored</text>
</svg>
```

### Vocabulary Highlights

Every word from your CSV that appears in the chapter text is highlighted with a colour that reflects its learning level:

| Level | Colour | Meaning |
|-------|--------|---------|
| L1 | 🔴 Red (full opacity) | New — never studied |
| L2 | 🟠 Orange | Seen once |
| L3 | 🟡 Yellow | Partially known |
| L4 | 🟢 Green (bright) | Almost mastered |
| L5 | 🟢 Green (dim) | Mastered — subtle underline only |
| Ignored | None | Removed from view |

Highlight opacity **fades** as words progress — the reader gets visually cleaner as you learn.

---

### The Tooltip

Clicking (or hovering, depending on settings) any highlighted word opens a **tooltip** with full word information:

```svg
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 700 280" font-family="'DM Sans',sans-serif">
  <rect width="700" height="280" rx="10" fill="#0e0e0e" stroke="#242424"/>
  <!-- Text fragment -->
  <text x="40" y="60" fill="#c8c8c8" font-size="15">Her </text>
  <rect x="72" y="46" width="80" height="22" rx="4" fill="rgba(248,113,113,0.35)"/>
  <text x="72" y="62" fill="#f87171" font-size="15">ephemeral</text>
  <text x="156" y="60" fill="#c8c8c8" font-size="15"> beauty captivated all.</text>

  <!-- Tooltip -->
  <rect x="40" y="82" width="310" height="180" rx="12" fill="#161616" stroke="#2e2e2e"/>
  <!-- Word + close -->
  <text x="58" y="108" fill="#e2e2e2" font-size="18" font-weight="700">ephemeral</text>
  <text x="58" y="124" fill="#888" font-size="11">/ɪˈfɛmərəl/</text>
  <rect x="316" y="88" width="22" height="22" rx="6" fill="#1c1c1c" stroke="#333"/>
  <text x="327" y="103" text-anchor="middle" fill="#555" font-size="12">✕</text>
  <!-- Level pips -->
  <circle cx="60" cy="143" r="5" fill="#f87171"/>
  <circle cx="74" cy="143" r="5" fill="#2e2e2e"/>
  <circle cx="88" cy="143" r="5" fill="#2e2e2e"/>
  <circle cx="102" cy="143" r="5" fill="#2e2e2e"/>
  <circle cx="116" cy="143" r="5" fill="#2e2e2e"/>
  <text x="130" y="147" fill="#555" font-size="10">Level 1</text>
  <!-- Definition -->
  <rect x="50" y="156" width="288" height="1" fill="#242424"/>
  <text x="58" y="174" fill="#888" font-size="10">adj.</text>
  <text x="80" y="174" fill="#aaa" font-size="11">lasting for a very short time</text>
  <!-- Action buttons -->
  <rect x="50" y="184" width="288" height="1" fill="#242424"/>
  <rect x="56" y="194" width="60" height="26" rx="6" fill="rgba(74,222,128,0.1)" stroke="rgba(74,222,128,0.3)"/>
  <text x="86" y="211" text-anchor="middle" fill="#4ade80" font-size="10" font-weight="700">▲ Level Up</text>
  <rect x="124" y="194" width="54" height="26" rx="6" fill="#1c1c1c" stroke="#2e2e2e"/>
  <text x="151" y="211" text-anchor="middle" fill="#888" font-size="10">▼ Drop</text>
  <rect x="186" y="194" width="58" height="26" rx="6" fill="#1c1c1c" stroke="#2e2e2e"/>
  <text x="215" y="211" text-anchor="middle" fill="#888" font-size="10">★ Master</text>
  <rect x="252" y="194" width="70" height="26" rx="6" fill="rgba(248,113,113,0.1)" stroke="rgba(248,113,113,0.2)"/>
  <text x="287" y="211" text-anchor="middle" fill="#f87171" font-size="10">✕ Ignore</text>

  <!-- Context sentence -->
  <text x="350" y="108" fill="#555" font-size="10" font-weight="700" letter-spacing="1">CONTEXT</text>
  <rect x="345" y="116" width="310" height="50" rx="6" fill="#1c1c1c" stroke="#242424"/>
  <text x="358" y="134" fill="#888" font-size="11">Her</text>
  <text x="374" y="134" fill="#4ade80" font-size="11">ephemeral</text>
  <text x="453" y="134" fill="#888" font-size="11">beauty</text>
  <text x="358" y="153" fill="#888" font-size="11">captivated all who saw her.</text>

  <!-- Synonyms -->
  <text x="350" y="188" fill="#555" font-size="10" font-weight="700" letter-spacing="1">SYNONYMS</text>
  <rect x="345" y="196" width="56" height="20" rx="10" fill="#1c1c1c" stroke="#2e2e2e"/>
  <text x="373" y="210" text-anchor="middle" fill="#888" font-size="10">fleeting</text>
  <rect x="407" y="196" width="58" height="20" rx="10" fill="#1c1c1c" stroke="#2e2e2e"/>
  <text x="436" y="210" text-anchor="middle" fill="#888" font-size="10">transient</text>
  <rect x="471" y="196" width="50" height="20" rx="10" fill="#1c1c1c" stroke="#2e2e2e"/>
  <text x="496" y="210" text-anchor="middle" fill="#888" font-size="10">brief</text>

  <!-- Edit mode note -->
  <rect x="345" y="230" width="310" height="28" rx="6" fill="rgba(232,54,93,0.06)" stroke="rgba(232,54,93,0.15)"/>
  <text x="500" y="248" text-anchor="middle" fill="#888" font-size="10">Press  E  to edit word data inline</text>
</svg>
```

**Tooltip actions:**

| Button | Shortcut | Action |
|--------|----------|--------|
| **▲ Level Up** | `2` | Move word to next level |
| **▼ Drop** | `1` | Drop word to previous level |
| **★ Master** | `3` | Jump directly to Level 5 |
| **☆ Focus** | `M` | Mark for focused study |
| **✕ Ignore** | `I` | Remove highlight entirely |
| **📖 Dict** | `Shift` | Look up in external dictionary |
| **✎ Edit** | `E` | Edit word data inline |
| **📌 Pin** | `P` | Keep tooltip open while scrolling |

The tooltip also shows:
- **Pronunciation** (IPA)
- **Part of speech** and **definition**
- **Context sentence** from the chapter
- **Synonyms / Antonyms** (if in CSV)
- **CSV source** name

---

### Word Levels (L1–L5)

Covenant uses a 5-level progression system:

```svg
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 700 90" font-family="'DM Sans',sans-serif">
  <rect width="700" height="90" rx="10" fill="#161616" stroke="#242424"/>
  <!-- L1 -->
  <rect x="20" y="20" width="118" height="50" rx="8" fill="#1c1c1c" stroke="rgba(248,113,113,0.4)"/>
  <text x="79" y="42" text-anchor="middle" fill="#f87171" font-size="14" font-weight="700">L1</text>
  <text x="79" y="58" text-anchor="middle" fill="#888" font-size="10">New</text>
  <rect x="20" y="67" width="118" height="3" rx="2" fill="#f87171" opacity="0.7"/>
  <!-- Arrow -->
  <text x="149" y="48" fill="#333" font-size="18">→</text>
  <!-- L2 -->
  <rect x="162" y="20" width="118" height="50" rx="8" fill="#1c1c1c" stroke="rgba(251,146,60,0.4)"/>
  <text x="221" y="42" text-anchor="middle" fill="#fb923c" font-size="14" font-weight="700">L2</text>
  <text x="221" y="58" text-anchor="middle" fill="#888" font-size="10">Seen once</text>
  <rect x="162" y="67" width="118" height="3" rx="2" fill="#fb923c" opacity="0.7"/>
  <!-- Arrow -->
  <text x="291" y="48" fill="#333" font-size="18">→</text>
  <!-- L3 -->
  <rect x="304" y="20" width="118" height="50" rx="8" fill="#1c1c1c" stroke="rgba(250,204,21,0.4)"/>
  <text x="363" y="42" text-anchor="middle" fill="#facc15" font-size="14" font-weight="700">L3</text>
  <text x="363" y="58" text-anchor="middle" fill="#888" font-size="10">Partial</text>
  <rect x="304" y="67" width="118" height="3" rx="2" fill="#facc15" opacity="0.7"/>
  <!-- Arrow -->
  <text x="433" y="48" fill="#333" font-size="18">→</text>
  <!-- L4 -->
  <rect x="446" y="20" width="118" height="50" rx="8" fill="#1c1c1c" stroke="rgba(74,222,128,0.4)"/>
  <text x="505" y="42" text-anchor="middle" fill="#4ade80" font-size="14" font-weight="700">L4</text>
  <text x="505" y="58" text-anchor="middle" fill="#888" font-size="10">Almost known</text>
  <rect x="446" y="67" width="118" height="3" rx="2" fill="#4ade80" opacity="0.7"/>
  <!-- Arrow -->
  <text x="575" y="48" fill="#333" font-size="18">→</text>
  <!-- L5 -->
  <rect x="588" y="20" width="92" height="50" rx="8" fill="rgba(74,222,128,0.06)" stroke="rgba(74,222,128,0.25)"/>
  <text x="634" y="42" text-anchor="middle" fill="#4ade80" font-size="14" font-weight="700">L5</text>
  <text x="634" y="58" text-anchor="middle" fill="#4ade80" font-size="10">Mastered ★</text>
  <rect x="588" y="67" width="92" height="3" rx="2" fill="#4ade80" opacity="0.3"/>
</svg>
```

- Level 5 words show only a faint underline (not a full highlight) to keep the text readable.
- Progress is stored per-word and persists across sessions.
- Levels earned in VocabForge sync with the reader highlighting instantly.

---

### Audio Player & Bookmarks

When audio is linked to a book, a **mini player bar** appears at the bottom of the reader:

```svg
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 700 70" font-family="'DM Sans',sans-serif">
  <rect width="700" height="70" rx="0" fill="#111" stroke="none"/>
  <rect y="0" width="700" height="1" fill="#242424"/>
  <!-- Play/pause -->
  <circle cx="40" cy="35" r="20" fill="#1c1c1c" stroke="#2e2e2e"/>
  <polygon points="34,26 34,44 52,35" fill="#e2e2e2"/>
  <!-- Time -->
  <text x="70" y="39" fill="#888" font-size="11" font-family="'DM Mono',monospace">12:34</text>
  <!-- Progress bar -->
  <rect x="110" y="32" width="430" height="6" rx="3" fill="#2e2e2e"/>
  <rect x="110" y="32" width="180" height="6" rx="3" fill="#e8365d"/>
  <!-- Bookmark marker -->
  <polygon points="232,26 232,38 240,32" fill="#e8365d" opacity="0.8"/>
  <polygon points="320,26 320,38 328,32" fill="#e8365d" opacity="0.8"/>
  <!-- Duration -->
  <text x="550" y="39" fill="#888" font-size="11" font-family="'DM Mono',monospace">48:12</text>
  <!-- Bookmark btn -->
  <rect x="578" y="20" width="62" height="30" rx="6" fill="#1c1c1c" stroke="#2e2e2e"/>
  <text x="609" y="39" text-anchor="middle" fill="#888" font-size="11">🔖 +BM</text>
  <!-- Speed -->
  <rect x="648" y="20" width="40" height="30" rx="6" fill="#1c1c1c" stroke="#2e2e2e"/>
  <text x="668" y="39" text-anchor="middle" fill="#888" font-size="11">1.0×</text>
</svg>
```

- Click anywhere on the progress bar to seek
- **Bookmark (🔖)** — drop a timestamp at the current position
- Bookmarks appear as **markers on the progress bar** — click to jump back
- Playback speed is adjustable
- Audio persists in IndexedDB across browser restarts

---

### Difficulty Badge

A floating badge in the bottom-right corner shows real-time **comprehension and difficulty estimates** for the current chapter:

```svg
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 700 280" font-family="'DM Sans',sans-serif">
  <rect width="700" height="280" rx="10" fill="#0e0e0e" stroke="#242424"/>
  <!-- Collapsed badge -->
  <rect x="580" y="220" width="80" height="32" rx="10" fill="#0f172a" stroke="rgba(255,255,255,0.1)"/>
  <circle cx="594" cy="236" r="5" fill="#facc15"/>
  <text x="604" y="240" fill="#facc15" font-size="12" font-weight="700">82%</text>
  <text x="633" y="240" fill="#64748b" font-size="9">Optimal</text>

  <!-- Expanded badge panel -->
  <rect x="380" y="30" width="290" height="230" rx="14" fill="#0f172a" stroke="rgba(255,255,255,0.1)"/>
  <!-- Header -->
  <circle cx="400" cy="58" r="7" fill="#facc15"/>
  <text x="414" y="62" fill="#facc15" font-size="14" font-weight="700">82%</text>
  <text x="445" y="62" fill="#94a3b8" font-size="11">Optimal</text>

  <rect x="388" y="72" width="274" height="1" fill="rgba(255,255,255,0.07)"/>

  <!-- Stats rows -->
  <text x="392" y="92" fill="#64748b" font-size="9" font-weight="700" letter-spacing="1">COMPREHENSION</text>
  <text x="650" y="92" text-anchor="end" fill="#facc15" font-size="11" font-weight="700">82%</text>
  <text x="392" y="110" fill="#64748b" font-size="9" font-weight="700" letter-spacing="1">DIFFICULTY</text>
  <text x="650" y="110" text-anchor="end" fill="#e2e8f0" font-size="11" font-weight="700">31% unknown</text>

  <rect x="388" y="118" width="274" height="1" fill="rgba(255,255,255,0.07)"/>

  <!-- Chapter / Book cards -->
  <rect x="390" y="126" width="126" height="64" rx="7" fill="rgba(255,255,255,0.04)"/>
  <text x="400" y="144" fill="#64748b" font-size="9" font-weight="700" letter-spacing="1">CHAPTER</text>
  <rect x="480" y="132" width="28" height="18" rx="4" fill="rgba(201,134,30,0.10)" stroke="rgba(201,134,30,0.35)"/>
  <text x="494" y="145" text-anchor="middle" fill="#c9861e" font-size="8" font-weight="700">VF</text>
  <text x="400" y="162" fill="#e2e8f0" font-size="13" font-weight="700">64 vocab</text>
  <text x="400" y="178" fill="#475569" font-size="9">4,211 words</text>

  <rect x="524" y="126" width="126" height="64" rx="7" fill="rgba(255,255,255,0.04)"/>
  <text x="534" y="144" fill="#64748b" font-size="9" font-weight="700" letter-spacing="1">BOOK</text>
  <rect x="614" y="132" width="28" height="18" rx="4" fill="rgba(74,222,128,0.10)" stroke="rgba(74,222,128,0.35)"/>
  <text x="628" y="145" text-anchor="middle" fill="#4ade80" font-size="8" font-weight="700">CSV</text>
  <text x="534" y="162" fill="#e2e8f0" font-size="13" font-weight="700">318 vocab</text>
  <text x="534" y="178" fill="#475569" font-size="9">48,500 words</text>

  <!-- Level bar -->
  <rect x="390" y="200" width="274" height="5" rx="3" fill="rgba(255,255,255,0.08)"/>
  <rect x="390" y="200" width="110" height="5" rx="3" fill="#f87171"/>
  <rect x="500" y="200" width="60" height="5" rx="3" fill="#fb923c"/>
  <rect x="560" y="200" width="104" height="5" rx="3" fill="#4ade80"/>

  <!-- Sparkline chips -->
  <rect x="390" y="218" width="38" height="32" rx="5" fill="rgba(248,113,113,0.1)" stroke="rgba(248,113,113,0.3)"/>
  <text x="409" y="232" text-anchor="middle" fill="#f87171" font-size="9" font-weight="700">L1</text>
  <text x="409" y="244" text-anchor="middle" fill="#f87171" font-size="10" font-weight="700">28</text>
  <rect x="434" y="218" width="38" height="32" rx="5" fill="rgba(251,146,60,0.1)" stroke="rgba(251,146,60,0.3)"/>
  <text x="453" y="232" text-anchor="middle" fill="#fb923c" font-size="9" font-weight="700">L2</text>
  <text x="453" y="244" text-anchor="middle" fill="#fb923c" font-size="10" font-weight="700">12</text>
  <rect x="478" y="218" width="38" height="32" rx="5" fill="rgba(250,204,21,0.07)" stroke="rgba(250,204,21,0.2)"/>
  <text x="497" y="232" text-anchor="middle" fill="#facc15" font-size="9" font-weight="700">L3</text>
  <text x="497" y="244" text-anchor="middle" fill="#facc15" font-size="10" font-weight="700">8</text>
  <rect x="522" y="218" width="38" height="32" rx="5" fill="rgba(74,222,128,0.07)" stroke="rgba(74,222,128,0.2)"/>
  <text x="541" y="232" text-anchor="middle" fill="#4ade80" font-size="9" font-weight="700">L4</text>
  <text x="541" y="244" text-anchor="middle" fill="#4ade80" font-size="10" font-weight="700">9</text>
  <rect x="566" y="218" width="38" height="32" rx="5" fill="rgba(74,222,128,0.05)" stroke="rgba(74,222,128,0.15)"/>
  <text x="585" y="232" text-anchor="middle" fill="#4ade80" font-size="9" font-weight="700">L5</text>
  <text x="585" y="244" text-anchor="middle" fill="#4ade80" font-size="10" font-weight="700">7</text>
  <rect x="616" y="224" width="56" height="22" rx="5" fill="rgba(255,255,255,0.06)" stroke="rgba(255,255,255,0.08)"/>
  <text x="644" y="238" text-anchor="middle" fill="#64748b" font-size="9">✕ Close</text>
</svg>
```

**Badge features:**
- **Comprehension %** — estimated percentage of the chapter text you currently know
- **Difficulty %** — percentage of highlighted words below Level 4
- **Chapter panel** — vocab word count + VF button (opens chapter in VocabForge)
- **Book panel** — total book vocabulary + **⬇ CSV** download button
- **Level chips (L1–L5)** — click any chip to **filter highlights** in the chapter to only that level
- **Ignored words are excluded** from all counts

---

### Unique Words Sidebar

Toggle with the **Unique** button in the topbar. Shows every unique vocabulary word appearing in the current chapter (or whole book), sorted by frequency, alphabetically, or by length.

**Features:**
- **Chapter / Book** tab — switch scope
- **Frequency filter** — hide words appearing more than N times (removes common words)
- **Coverage stat** — what % of the chapter's running words are in your CSV
- **Coverage trend chart** — sparkline of coverage across recent chapters
- **⚡ Mine All Visible** — send all listed words to Words Mining in one click
- **⬇ Download CSV** — export the word list
- **⊞ Grid View** — open an interactive grid card view in a new tab

---

### Highlights Panel

Toggle with the **Highlights** button in the topbar. Shows all highlighted words in the current chapter with level badges and bulk-action controls.

```svg
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 280 320" font-family="'DM Sans',sans-serif">
  <rect width="280" height="320" rx="10" fill="#161616" stroke="#242424"/>
  <!-- Header -->
  <text x="16" y="24" fill="#888" font-size="10" font-weight="700" letter-spacing="1.5">✏ HIGHLIGHTS</text>
  <rect x="232" y="12" width="32" height="18" rx="9" fill="rgba(232,54,93,0.1)"/>
  <text x="248" y="24" text-anchor="middle" fill="#e8365d" font-size="10" font-weight="700">42</text>
  <!-- Filter strip -->
  <rect x="8" y="38" width="264" height="28" rx="0" fill="none" stroke="none"/>
  <rect x="10" y="42" width="36" height="18" rx="5" fill="rgba(232,54,93,0.1)" stroke="rgba(232,54,93,0.28)"/>
  <text x="28" y="54" text-anchor="middle" fill="#e8365d" font-size="10" font-weight="700">All</text>
  <rect x="52" y="42" width="32" height="18" rx="5" fill="none"/>
  <text x="68" y="54" text-anchor="middle" fill="#555" font-size="10">L1</text>
  <rect x="90" y="42" width="32" height="18" rx="5" fill="none"/>
  <text x="106" y="54" text-anchor="middle" fill="#555" font-size="10">L2</text>
  <rect x="128" y="42" width="32" height="18" rx="5" fill="none"/>
  <text x="144" y="54" text-anchor="middle" fill="#555" font-size="10">L3</text>
  <rect x="166" y="42" width="32" height="18" rx="5" fill="none"/>
  <text x="182" y="54" text-anchor="middle" fill="#555" font-size="10">L4</text>
  <rect x="204" y="42" width="32" height="18" rx="5" fill="none"/>
  <text x="220" y="54" text-anchor="middle" fill="#555" font-size="10">L5</text>
  <!-- Word rows -->
  <rect x="0" y="68" width="280" height="24" fill="rgba(232,54,93,0.05)" stroke="none"/>
  <rect x="0" y="68" width="2" height="24" fill="rgba(232,54,93,0.5)"/>
  <rect x="10" y="74" width="3" height="12" rx="2" fill="#f87171"/>
  <text x="20" y="84" fill="#f87171" font-size="12">ephemeral</text>
  <text x="192" y="84" fill="#555" font-size="9" font-family="'DM Mono',monospace">×3</text>
  <rect x="215" y="71" width="28" height="16" rx="3" fill="rgba(248,113,113,0.1)" stroke="rgba(248,113,113,0.25)"/>
  <text x="229" y="82" text-anchor="middle" fill="#f87171" font-size="8" font-weight="700">L1</text>
  <text x="256" y="84" fill="#555" font-size="12">👁</text>

  <rect x="0" y="92" width="280" height="24" fill="none"/>
  <rect x="10" y="98" width="3" height="12" rx="2" fill="#facc15"/>
  <text x="20" y="108" fill="#e2e2e2" font-size="12">fleeting</text>
  <text x="192" y="108" fill="#555" font-size="9" font-family="'DM Mono',monospace">×1</text>
  <rect x="215" y="95" width="28" height="16" rx="3" fill="rgba(250,204,21,0.1)" stroke="rgba(250,204,21,0.25)"/>
  <text x="229" y="106" text-anchor="middle" fill="#facc15" font-size="8" font-weight="700">L3</text>

  <rect x="0" y="116" width="280" height="24" fill="none"/>
  <rect x="10" y="122" width="3" height="12" rx="2" fill="#4ade80"/>
  <text x="20" y="132" fill="#e2e2e2" font-size="12">serene</text>
  <text x="192" y="132" fill="#555" font-size="9" font-family="'DM Mono',monospace">×2</text>
  <rect x="215" y="119" width="28" height="16" rx="3" fill="rgba(74,222,128,0.1)" stroke="rgba(74,222,128,0.25)"/>
  <text x="229" y="130" text-anchor="middle" fill="#4ade80" font-size="8" font-weight="700">L4</text>

  <!-- Bulk actions -->
  <rect x="0" y="270" width="280" height="50" rx="0" fill="#0e0e0e" stroke="none"/>
  <rect x="0" y="270" width="280" height="1" fill="#242424"/>
  <text x="140" y="284" text-anchor="middle" fill="#555" font-size="9" font-weight="700" letter-spacing="1">SELECT WORDS TO ACT ON</text>
  <rect x="8" y="290" width="58" height="22" rx="6" fill="#1c1c1c" stroke="#2e2e2e"/>
  <text x="37" y="304" text-anchor="middle" fill="#fb923c" font-size="9">▼ Level Down</text>
  <rect x="72" y="290" width="52" height="22" rx="6" fill="#1c1c1c" stroke="#2e2e2e"/>
  <text x="98" y="304" text-anchor="middle" fill="#4ade80" font-size="9">▲ Level Up</text>
  <rect x="130" y="290" width="50" height="22" rx="6" fill="#1c1c1c" stroke="#2e2e2e"/>
  <text x="155" y="304" text-anchor="middle" fill="#facc15" font-size="9">★ Mastery</text>
  <rect x="186" y="290" width="40" height="22" rx="6" fill="#1c1c1c" stroke="#2e2e2e"/>
  <text x="206" y="304" text-anchor="middle" fill="#f87171" font-size="9">👁 Hide</text>
</svg>
```

- **Level filter strip** — show only L1, L2, L3, L4, or L5 words
- **Search** — filter words by name
- **Select-all checkbox** for bulk operations
- **Bulk actions** — Level Down, Level Up, Mastery, Hide/Unhide
- **Per-row hide button** — hide a specific word's highlight without ignoring it
- **⊞ Grid View** — open highlights as interactive flashcard grid

---

### Rules Panel

Toggle with the **Rules** button in the topbar. Shows all **Connected Speech rules** that match the current chapter's text.

- Scans raw chapter text (immune to CS DOM mutations)
- Shows **hit count** — how many times each rule fired in this chapter
- **Category badge** — colour-coded by rule type
- **Inline Edit** — modify original phrase, connected form, category, and note without leaving the reader
- **Delete** — remove a rule with confirmation
- **Manage All Rules** button — navigate to My Vocab → Rules

---

### Dictionary Lookup

When **Dictionary Lookup** is enabled (`Alt D` or Settings toggle), a **📖 Dict** button appears in the tooltip. Pressing it (or pressing `Shift` with a tooltip open) fetches the word definition from your configured external dictionary URL and shows it in the **Dictionary sidebar**.

You can also configure a **Hover Dictionary** (`Alt H`) to auto-fetch definitions on hover.

---

### Word Peek

**Word Peek** (`Alt W` to toggle) shows a floating definition peek as you hover over highlighted words — without opening the full tooltip. Useful for quick lookups while reading at speed.

---

### Keyboard Shortcuts

Full reference in the [Keyboard Shortcuts Reference](#keyboard-shortcuts-reference) section below.

---

## VocabForge — Spaced Repetition Study

VocabForge is the built-in SRS (spaced repetition) study system. Load words from any source and study them in four modes:

```svg
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 700 160" font-family="'DM Sans',sans-serif">
  <rect width="700" height="160" rx="10" fill="#161616" stroke="#242424"/>
  <text x="350" y="28" text-anchor="middle" fill="#888" font-size="11" font-weight="700" letter-spacing="1">STUDY MODES</text>

  <!-- Cards -->
  <rect x="20" y="42" width="148" height="100" rx="10" fill="#1c1c1c" stroke="#2e2e2e"/>
  <text x="94" y="72" text-anchor="middle" fill="#e2e2e2" font-size="20">📋</text>
  <text x="94" y="94" text-anchor="middle" fill="#e2e2e2" font-size="13" font-weight="600">Cards</text>
  <text x="94" y="112" text-anchor="middle" fill="#555" font-size="10">Browse &amp; level words</text>
  <text x="94" y="128" text-anchor="middle" fill="#555" font-size="10">from your loaded set</text>

  <!-- Flashcard -->
  <rect x="184" y="42" width="148" height="100" rx="10" fill="#1c1c1c" stroke="#2e2e2e"/>
  <text x="258" y="72" text-anchor="middle" fill="#e2e2e2" font-size="20">🔄</text>
  <text x="258" y="94" text-anchor="middle" fill="#e2e2e2" font-size="13" font-weight="600">Flashcard</text>
  <text x="258" y="112" text-anchor="middle" fill="#555" font-size="10">Flip to reveal</text>
  <text x="258" y="128" text-anchor="middle" fill="#555" font-size="10">pronunciation &amp; definition</text>

  <!-- Quiz -->
  <rect x="348" y="42" width="148" height="100" rx="10" fill="#1c1c1c" stroke="#2e2e2e"/>
  <text x="422" y="72" text-anchor="middle" fill="#e2e2e2" font-size="20">✏️</text>
  <text x="422" y="94" text-anchor="middle" fill="#e2e2e2" font-size="13" font-weight="600">Quiz</text>
  <text x="422" y="112" text-anchor="middle" fill="#555" font-size="10">Type the definition</text>
  <text x="422" y="128" text-anchor="middle" fill="#555" font-size="10">— scored immediately</text>

  <!-- Multiple Choice -->
  <rect x="512" y="42" width="168" height="100" rx="10" fill="#1c1c1c" stroke="#2e2e2e"/>
  <text x="596" y="72" text-anchor="middle" fill="#e2e2e2" font-size="20">🎯</text>
  <text x="596" y="94" text-anchor="middle" fill="#e2e2e2" font-size="13" font-weight="600">Multiple Choice</text>
  <text x="596" y="112" text-anchor="middle" fill="#555" font-size="10">Pick from 4 options</text>
  <text x="596" y="128" text-anchor="middle" fill="#555" font-size="10">with distractors</text>
</svg>
```

**Word sources for VocabForge:**

| Source | How to load |
|--------|-------------|
| Chapter highlights | Difficulty Badge → **VF** button (chapter column) |
| All book highlights | Difficulty Badge → Book column stats |
| CSV deck | Core tab → deck card → **▶ VF** |
| Specific level | Click level segment in chapter/book stats |

**Filters:**
- **All / New / Studying / Mastered** — filter by status
- **Hide Common** — suppress words appearing more than 8× in the chapter
- **Search** — filter the card list by word

**Context sentences** — cards show a real context sentence harvested from the chapter text to reinforce natural usage.

**Stats bar** — shows word counts per status (New / Studying / Mastered) and overall progress.

---

## My Vocabulary

The **My Vocab** tab is a five-section hub for managing your learning data.

### Weak Words

Words you have failed **multiple times** in Quiz, Flashcard, or Multiple Choice sessions. Useful for targeted review.

- **Fail Threshold** slider — set how many failures qualify as "weak" (default: 3)
- Each card shows: word, accuracy %, last studied date, fail count
- **↻ Refresh** — recompute the list

### Focus Words

Words you've manually starred with the **☆ Focus** button in the reader tooltip. Acts as a personal "look at this later" list.

- **✕ Clear all** — remove all focus words at once
- Individual delete per word

### Words Mining

A **scratchpad** for capturing words as you read — outside the CSV system.

```svg
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 700 120" font-family="'DM Sans',sans-serif">
  <rect width="700" height="120" rx="10" fill="#161616" stroke="#242424"/>
  <text x="24" y="28" fill="#e2e2e2" font-size="14" font-weight="700">⚡ Words Mining</text>
  <text x="24" y="46" fill="#555" font-size="11">Capture words as you read. Download as CSV to import into your vocabulary decks.</text>
  <!-- Quick capture form -->
  <rect x="20" y="60" width="180" height="44" rx="8" fill="#1c1c1c" stroke="#2e2e2e"/>
  <text x="36" y="76" fill="#555" font-size="9">Word *</text>
  <text x="36" y="92" fill="#e2e2e2" font-size="12">ephemeral</text>
  <rect x="212" y="60" width="160" height="44" rx="8" fill="#1c1c1c" stroke="#2e2e2e"/>
  <text x="228" y="76" fill="#555" font-size="9">Pronunciation</text>
  <text x="228" y="92" fill="#888" font-size="12">/ɪˈfɛmərəl/</text>
  <rect x="384" y="60" width="220" height="44" rx="8" fill="#1c1c1c" stroke="#2e2e2e"/>
  <text x="400" y="76" fill="#555" font-size="9">Definition</text>
  <text x="400" y="92" fill="#888" font-size="12">lasting a very short time</text>
  <rect x="618" y="66" width="64" height="32" rx="8" fill="#e8365d"/>
  <text x="650" y="86" text-anchor="middle" fill="white" font-size="13" font-weight="700">+ Mine</text>
</svg>
```

- Cap: **500 words**, auto-purge after 7 days
- **⬇ Download CSV** — export as `word, pronunciation, definition` CSV
- **ⓘ How it works** — inline tutorial panel
- Mined words are highlighted in the reader (just like CSV words) so you notice them while reading

### Mastered Words

All words at Level 5 across all your CSV sets and VocabForge sessions.

- **⬆ Import Mastery Words** — bulk-import a CSV or TXT file and set all words to Level 5 instantly
- **⬇ Export CSV** — download your full mastery list
- **Search** and **pagination** (20 / 50 / 100 per page)
- **By Source** breakdown — shows which CSV contributed the most mastered words

### Connected Speech Rules

Manage rules that show how spoken English (or other languages) differs from its written form.

```svg
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 700 180" font-family="'DM Sans',sans-serif">
  <rect width="700" height="180" rx="10" fill="#161616" stroke="#242424"/>
  <text x="24" y="28" fill="#e2e2e2" font-size="14" font-weight="700">🔗 Connected Speech Rules</text>
  <!-- Rule rows -->
  <rect x="20" y="44" width="660" height="40" rx="7" fill="#1c1c1c" stroke="#2e2e2e"/>
  <text x="36" y="60" fill="#e2e2e2" font-size="13" font-weight="600">want to</text>
  <text x="106" y="60" fill="#555" font-size="12">→</text>
  <text x="120" y="60" fill="#f59e0b" font-size="13" font-style="italic">wanna</text>
  <rect x="196" y="50" width="62" height="18" rx="9" fill="rgba(74,222,128,0.12)" stroke="rgba(74,222,128,0.3)"/>
  <text x="227" y="62" text-anchor="middle" fill="#4ade80" font-size="9" font-weight="700">Reduction</text>
  <text x="278" y="62" fill="#555" font-size="10">reduction in fast speech</text>
  <text x="590" y="62" fill="#555" font-size="10">14 hits</text>
  <text x="638" y="62" fill="#555" font-size="12">✎</text>
  <text x="661" y="62" fill="#555" font-size="12">✕</text>

  <rect x="20" y="92" width="660" height="40" rx="7" fill="#1c1c1c" stroke="#2e2e2e"/>
  <text x="36" y="108" fill="#e2e2e2" font-size="13" font-weight="600">going to</text>
  <text x="112" y="108" fill="#555" font-size="12">→</text>
  <text x="126" y="108" fill="#f59e0b" font-size="13" font-style="italic">gonna</text>
  <rect x="196" y="98" width="62" height="18" rx="9" fill="rgba(74,222,128,0.12)" stroke="rgba(74,222,128,0.3)"/>
  <text x="227" y="110" text-anchor="middle" fill="#4ade80" font-size="9" font-weight="700">Reduction</text>
  <text x="638" y="110" fill="#555" font-size="12">✎</text>
  <text x="661" y="110" fill="#555" font-size="12">✕</text>

  <rect x="20" y="140" width="660" height="40" rx="7" fill="#1c1c1c" stroke="#2e2e2e"/>
  <text x="36" y="156" fill="#e2e2e2" font-size="13" font-weight="600">did you</text>
  <text x="100" y="156" fill="#555" font-size="12">→</text>
  <text x="114" y="156" fill="#f59e0b" font-size="13" font-style="italic">didja</text>
  <rect x="196" y="148" width="80" height="18" rx="9" fill="rgba(123,158,240,0.12)" stroke="rgba(123,158,240,0.3)"/>
  <text x="236" y="160" text-anchor="middle" fill="#7b9ef0" font-size="9" font-weight="700">Assimilation</text>
  <text x="638" y="156" fill="#555" font-size="12">✎</text>
  <text x="661" y="156" fill="#555" font-size="12">✕</text>
</svg>
```

**Rule anatomy:** `original phrase → connected form` + category + optional note

**Categories** (each with its own colour):
- Reduction, Assimilation, Linking, Elision, Contraction, Intrusion, Custom

**Adding rules:**
1. **From the reader** — select text, press the Connected Speech popup → fill in connected form
2. **Manual form** — + Add Rule button
3. **CSV upload** — bulk import (`original,connected form,note`)

**Category colours** are fully customisable in this panel.

---

## Core Tab — Settings & Backup

The **Core** tab contains global settings and data management.

### Vocabulary Deck Manager
Lists all loaded CSV sets with word counts. Each deck has:
- **▶ VF** — open in VocabForge
- **↓ CSV** — download the original CSV
- **✕** — remove the deck

### Audio Upload
Attach audio to the currently open book from the home screen.

### Backup & Restore
```
What's saved in a backup:
• All CSV vocabulary sets
• VocabForge study progress (per-word levels)
• Words Mining list
• Ignored words
• Focus words
• Coverage trend data
• Connected Speech rules
• Reader settings
```

- **⬇ Download Backup** — save a JSON file locally
- **↩ Restore Backup** — load a previously saved JSON to replace current data

---

## Reader Settings

Open with the **⚙ Settings** button in the reader topbar.

### Themes

10 built-in themes — 4 light, 6 dark:

```svg
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 700 120" font-family="'DM Sans',sans-serif">
  <!-- Dark -->
  <rect x="10" y="10" width="60" height="80" rx="8" fill="#0e0e0e" stroke="#333"/>
  <rect x="14" y="18" width="52" height="8" rx="3" fill="#e8365d" opacity="0.6"/>
  <rect x="14" y="30" width="38" height="5" rx="2" fill="#555"/>
  <rect x="14" y="39" width="46" height="5" rx="2" fill="#444"/>
  <rect x="14" y="48" width="30" height="5" rx="2" fill="#444"/>
  <text x="40" y="104" text-anchor="middle" fill="#888" font-size="9">Dark</text>

  <!-- Warm Paper -->
  <rect x="80" y="10" width="60" height="80" rx="8" fill="#f5f0e8" stroke="#d4c9b0"/>
  <rect x="84" y="18" width="52" height="8" rx="3" fill="#c0392b" opacity="0.7"/>
  <rect x="84" y="30" width="38" height="5" rx="2" fill="#8a7555"/>
  <rect x="84" y="39" width="46" height="5" rx="2" fill="#999"/>
  <rect x="84" y="48" width="30" height="5" rx="2" fill="#999"/>
  <text x="110" y="104" text-anchor="middle" fill="#888" font-size="9">Warm Paper</text>

  <!-- Nord -->
  <rect x="150" y="10" width="60" height="80" rx="8" fill="#1e2330" stroke="#333d52"/>
  <rect x="154" y="18" width="52" height="8" rx="3" fill="#88c0d0" opacity="0.7"/>
  <rect x="154" y="30" width="38" height="5" rx="2" fill="#546378"/>
  <rect x="154" y="39" width="46" height="5" rx="2" fill="#445"/>
  <rect x="154" y="48" width="30" height="5" rx="2" fill="#445"/>
  <text x="180" y="104" text-anchor="middle" fill="#888" font-size="9">Nord</text>

  <!-- Solarized -->
  <rect x="220" y="10" width="60" height="80" rx="8" fill="#002b36" stroke="#144f5e"/>
  <rect x="224" y="18" width="52" height="8" rx="3" fill="#268bd2" opacity="0.7"/>
  <rect x="224" y="30" width="38" height="5" rx="2" fill="#3a6470"/>
  <rect x="224" y="39" width="46" height="5" rx="2" fill="#2a5560"/>
  <rect x="224" y="48" width="30" height="5" rx="2" fill="#2a5560"/>
  <text x="250" y="104" text-anchor="middle" fill="#888" font-size="9">Solarized</text>

  <!-- Forest -->
  <rect x="290" y="10" width="60" height="80" rx="8" fill="#0d1a12" stroke="#223826"/>
  <rect x="294" y="18" width="52" height="8" rx="3" fill="#5bbf72" opacity="0.7"/>
  <rect x="294" y="30" width="38" height="5" rx="2" fill="#4a6b48"/>
  <rect x="294" y="39" width="46" height="5" rx="2" fill="#3a5538"/>
  <rect x="294" y="48" width="30" height="5" rx="2" fill="#3a5538"/>
  <text x="320" y="104" text-anchor="middle" fill="#888" font-size="9">Forest</text>

  <!-- Midnight -->
  <rect x="360" y="10" width="60" height="80" rx="8" fill="#0a0e1a" stroke="#1e2a44"/>
  <rect x="364" y="18" width="52" height="8" rx="3" fill="#7b9ef0" opacity="0.7"/>
  <rect x="364" y="30" width="38" height="5" rx="2" fill="#3a4f7a"/>
  <rect x="364" y="39" width="46" height="5" rx="2" fill="#2a3a60"/>
  <rect x="364" y="48" width="30" height="5" rx="2" fill="#2a3a60"/>
  <text x="390" y="104" text-anchor="middle" fill="#888" font-size="9">Midnight</text>

  <!-- Ivory -->
  <rect x="430" y="10" width="60" height="80" rx="8" fill="#f9f6f0" stroke="#ddd5c5"/>
  <rect x="434" y="18" width="52" height="8" rx="3" fill="#b05a2f" opacity="0.7"/>
  <rect x="434" y="30" width="38" height="5" rx="2" fill="#9a8770"/>
  <rect x="434" y="39" width="46" height="5" rx="2" fill="#aaa"/>
  <rect x="434" y="48" width="30" height="5" rx="2" fill="#aaa"/>
  <text x="460" y="104" text-anchor="middle" fill="#888" font-size="9">Ivory</text>

  <!-- Sage -->
  <rect x="500" y="10" width="60" height="80" rx="8" fill="#f4f6f2" stroke="#cdd4c6"/>
  <rect x="504" y="18" width="52" height="8" rx="3" fill="#3d7a4a" opacity="0.7"/>
  <rect x="504" y="30" width="38" height="5" rx="2" fill="#7a8f76"/>
  <rect x="504" y="39" width="46" height="5" rx="2" fill="#999"/>
  <rect x="504" y="48" width="30" height="5" rx="2" fill="#999"/>
  <text x="530" y="104" text-anchor="middle" fill="#888" font-size="9">Sage</text>

  <!-- Obsidian -->
  <rect x="570" y="10" width="60" height="80" rx="8" fill="#13141a" stroke="#2c3040"/>
  <rect x="574" y="18" width="52" height="8" rx="3" fill="#c97beb" opacity="0.7"/>
  <rect x="574" y="30" width="38" height="5" rx="2" fill="#505870"/>
  <rect x="574" y="39" width="46" height="5" rx="2" fill="#404060"/>
  <rect x="574" y="48" width="30" height="5" rx="2" fill="#404060"/>
  <text x="600" y="104" text-anchor="middle" fill="#888" font-size="9">Obsidian</text>

  <!-- Amber label -->
  <text x="640" y="60" text-anchor="middle" fill="#555" font-size="9">+Amber</text>
</svg>
```

### Fonts

10 reader fonts, all with CJK fallbacks (Japanese, Chinese, Korean):

| Font | Style |
|------|-------|
| **Source Sans** | Default — clean sans-serif |
| **Serif** | Lora — elegant book serif |
| **Garamond** | EB Garamond — classic humanist |
| **Playfair** | Playfair Display — dramatic editorial |
| **IBM Plex** | IBM Plex Serif — modern technical |
| **Literata** | Google eBook serif |
| **Crimson** | Crimson Pro — scholarly |
| **Baskerville** | Libre Baskerville — timeless |
| **Spectral** | Spectral — contemporary serif |
| **Serif JP** | Noto Serif JP-first (for Japanese) |

Font size and line height are also adjustable via sliders.

---

### Connected Speech Mode

When enabled (`Alt K` to toggle), Covenant overlays your Connected Speech rules onto the chapter text — **replacing the written form with the spoken form** so you read what you'd actually hear.

```
Written:  "I want to go to the store."
CS Mode:  "I wanna go to the store."
```

- **Gloss mode** — instead of replacing text, shows the connected form as a **superscript tooltip** above the original word
- **Alt F** — activate a Connected Form popup from selected text to add a rule instantly

---

### Ignored Words CSV

Upload a list of words to **permanently suppress** their highlights across all books. Useful for very common words you don't want cluttering the display.

---

## Session Stats

At the end of each chapter, a **✓ Chapter Completed** button appears. Clicking it shows a summary of your study session:

```svg
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 700 180" font-family="'DM Sans',sans-serif">
  <rect width="700" height="180" rx="10" fill="#0e0e0e" stroke="#242424"/>
  <rect x="190" y="20" width="320" height="140" rx="14" fill="#161622" stroke="rgba(255,255,255,0.08)"/>
  <text x="350" y="50" text-anchor="middle" fill="#e2e2e2" font-size="16" font-weight="700">Chapter Complete</text>
  <text x="350" y="68" text-anchor="middle" fill="#555" font-size="11">Chapter 4 — The Journey</text>
  <!-- Stat pills -->
  <rect x="210" y="82" width="80" height="50" rx="8" fill="rgba(255,255,255,0.04)" stroke="rgba(255,255,255,0.08)"/>
  <text x="250" y="105" text-anchor="middle" fill="#7dd3fc" font-size="22" font-weight="700">▲ 8</text>
  <text x="250" y="122" text-anchor="middle" fill="#555" font-size="10">Level Ups</text>

  <rect x="305" y="82" width="80" height="50" rx="8" fill="rgba(255,255,255,0.04)" stroke="rgba(255,255,255,0.08)"/>
  <text x="345" y="105" text-anchor="middle" fill="#fbbf24" font-size="22" font-weight="700">★ 3</text>
  <text x="345" y="122" text-anchor="middle" fill="#555" font-size="10">Mastered</text>

  <rect x="400" y="82" width="90" height="50" rx="8" fill="rgba(255,255,255,0.04)" stroke="rgba(255,255,255,0.08)"/>
  <text x="445" y="105" text-anchor="middle" fill="#a78bfa" font-size="22" font-weight="700">11</text>
  <text x="445" y="122" text-anchor="middle" fill="#555" font-size="10">Words studied</text>

  <rect x="250" y="144" width="200" height="8" rx="4" fill="#2e2e2e"/>
  <rect x="250" y="144" width="140" height="8" rx="4" fill="#4ade80"/>
  <text x="350" y="165" text-anchor="middle" fill="#555" font-size="10">70% chapter words known</text>
</svg>
```

---

## Data & Privacy

Covenant stores everything **locally in your browser** — nothing is ever sent to a server.

| Storage | What's stored |
|---------|--------------|
| **IndexedDB** | Book files (HTML), cover images, audio blobs |
| **localStorage** | All other data: vocab progress, settings, rules, mining list, ignored words, focus words, bookmarks, coverage trends |

> ⚠️ Clearing your browser data will erase everything. Use **Download Backup** regularly.

---

## Keyboard Shortcuts Reference

### Reader Toggles

| Action | Shortcut |
|--------|----------|
| Sidebar Tooltip mode | `Alt + S` |
| Click-to-Show Tooltip | `Alt + C` |
| Dictionary Lookup | `Alt + D` |
| Word Peek | `Alt + W` |
| Hover Dictionary | `Alt + H` |
| Connected Speech mode | `Alt + K` |
| Activate Connected Form popup | `Alt + F` |

### Tooltip — Word Actions

| Action | Shortcut |
|--------|----------|
| Drop word to previous level | `1` |
| Level up word | `2` |
| Master word (jump to Level 5) | `3` |
| Focus / unfocus word | `M` |
| Ignore / unignore word | `I` |

### Tooltip — Controls

| Action | Shortcut |
|--------|----------|
| Open inline edit mode | `E` |
| Pin / unpin tooltip | `P` |
| Dictionary lookup | `Shift` |
| Dismiss / unpin tooltip | `Esc` |

### Inline Edit Mode

| Action | Shortcut |
|--------|----------|
| Save changes | `Enter` |
| Cancel edits | `Esc` |
| Move between fields | `Tab` |

---

*Covenant is a self-contained HTML application. All data is local. No internet connection is required to use the reader after fonts are loaded.*

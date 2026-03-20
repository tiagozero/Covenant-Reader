================================================================================
  COVENANT — Vocabulary-Immersion Reading App
  Read. Listen. Track your vocabulary. Build fluency.
================================================================================

Covenant is an all-in-one reader that turns EPUB and plain text books into
active vocabulary-learning sessions. Load your vocabulary CSV, open a book,
and every word in your deck is highlighted as you read — with level tracking,
spaced-repetition study, connected-speech analysis, and detailed statistics.
Everything runs in a single HTML file, entirely in your browser. No account,
no server, no install required.


--------------------------------------------------------------------------------
  TABLE OF CONTENTS
--------------------------------------------------------------------------------

  1.  Getting Started
  2.  Portal — Choosing Your Tool
  3.  Library — Managing Books
  4.  Upload & Vocabulary CSV
  5.  The Reader
        5.1  Vocabulary Highlights
        5.2  The Tooltip
        5.3  Word Levels (L1–L5)
        5.4  Audio Player & Bookmarks
        5.5  Difficulty Badge
        5.6  Unique Words Sidebar
        5.7  Highlights Panel
        5.8  Rules Panel
        5.9  Dictionary Lookup & Word Peek
        5.10 Keyboard Shortcuts
  6.  VocabForge — Spaced Repetition Study
  7.  My Vocabulary
        7.1  Weak Words
        7.2  Focus Words
        7.3  Words Mining
        7.4  Mastered Words
        7.5  Connected Speech Rules
  8.  Core Tab — Settings & Backup
  9.  Reader Settings
        9.1  Themes
        9.2  Fonts
        9.3  Connected Speech Mode
        9.4  Ignored Words CSV
  10. Session Stats
  11. Data & Privacy
  12. Keyboard Shortcuts Reference


================================================================================
  1. GETTING STARTED
================================================================================

  1. Open index.html in any modern browser (Chrome, Firefox, Edge, Safari).
  2. Click "Covenant Reader" on the portal screen.
  3. Go to the Upload tab and drop in an EPUB or .txt file.
  4. (Optional) Upload a vocabulary CSV to enable word highlighting.
  5. Open the book from your Library and start reading.

All data is stored locally in your browser. Nothing is sent to any server.


================================================================================
  2. PORTAL — CHOOSING YOUR TOOL
================================================================================

The portal is the launcher screen you see when first opening the app.
It offers three tools:

  Covenant Reader
    Upload a book (EPUB / TXT) and optional audio file. Read with full
    vocabulary tracking, word highlights, tooltips, and SRS study.

  Shadow
    Shadowing practice mode — listen to a recording and repeat along to
    internalize natural speech patterns and pronunciation.

  Roadmap
    Structured learning paths by language. English is available now.
    Japanese and Spanish are coming soon.


================================================================================
  3. LIBRARY — MANAGING BOOKS
================================================================================

The Library tab shows all books you have imported as cards. Each card
displays the book title, cover image (auto-extracted from EPUB files),
chapter count, and an audio badge when audio has been linked.

  Actions available per book:

    Click card     Open the book in the reader
    Link Audio     Attach an MP3 or other audio file (persists across sessions)
    Archive        Hide a book from the Library without deleting it
                   (archived books are visible in the Archive tab)
    Delete         Permanently remove the book and its associated audio

Books remain available between sessions because they are stored in the
browser's IndexedDB database.


================================================================================
  4. UPLOAD & VOCABULARY CSV
================================================================================

The Upload tab is where you bring content into Covenant.

  Book Upload
  -----------
  Drag and drop an .epub or .txt file onto the drop zone, or click to browse.
  EPUB chapter structure, cover images, and metadata are extracted automatically.

  Vocabulary CSV
  --------------
  A vocabulary CSV drives the highlight system. Each row defines one word:

    word, pronunciation, definition, pos, synonyms, antonyms

  Column reference:

    word           REQUIRED  The target word or phrase to highlight
    pronunciation  optional  IPA or phonetic reading (e.g. /ɪˈfɛmərəl/)
    definition     optional  Shown in the tooltip while reading
    pos            optional  Part of speech (adj, n, v, etc.)
    synonyms       optional  Comma-separated synonyms
    antonyms       optional  Comma-separated antonyms

  Example row:
    ephemeral,/ɪˈfɛmərəl/,lasting for a very short time,adj,fleeting,permanent

  You can load MULTIPLE CSV sets simultaneously. Each set gets a different
  colour dot so you can tell them apart at a glance. Sets can be downloaded
  as CSV or removed at any time from the Core tab.


================================================================================
  5. THE READER
================================================================================

The reader is the main workspace. It is divided into three zones:

  Left sidebar    Chapter list — click any chapter to jump to it
  Centre          The chapter text with vocabulary highlights
  Right panels    Optional: Unique Words, Highlights, Rules, Dictionary


  5.1  Vocabulary Highlights
  --------------------------
  Every word in your CSV that appears in the chapter text gets highlighted.
  The highlight colour reflects the word's current learning level:

    L1  Red (full opacity)   New — never studied
    L2  Orange               Seen once
    L3  Yellow               Partially known
    L4  Green (bright)       Almost mastered
    L5  Green (very faint)   Mastered — subtle underline only
    --  No highlight         Ignored words

  Highlight intensity fades as words progress, so the reading experience
  becomes cleaner as your vocabulary grows.


  5.2  The Tooltip
  ----------------
  Click (or hover, depending on settings) any highlighted word to open its
  tooltip. The tooltip shows:

    - Word + pronunciation
    - Part of speech + definition
    - Level progress (five pip indicators)
    - A context sentence from the current chapter
    - Synonyms and antonyms (if present in the CSV)
    - The name of the CSV set the word belongs to

  Action buttons in the tooltip:

    Level Up  (shortcut: 2)   Move word to the next level
    Drop      (shortcut: 1)   Drop word to the previous level
    Master    (shortcut: 3)   Jump directly to Level 5
    Focus     (shortcut: M)   Star the word for focused study
    Ignore    (shortcut: I)   Remove the word's highlight entirely
    Dict      (shortcut: Shift) Look up in your configured dictionary
    Edit      (shortcut: E)   Edit the word's data inline
    Pin       (shortcut: P)   Keep tooltip open while you scroll


  5.3  Word Levels (L1–L5)
  -------------------------
  Covenant uses a five-level progression for each word:

    L1  New             Full bright highlight, never studied
    L2  Seen once       Slightly dimmer highlight
    L3  Partial         Medium opacity highlight
    L4  Almost known    Light highlight
    L5  Mastered        Faint underline only; excluded from SRS sessions

  Progress is stored per word and survives browser restarts. Levels earned
  in VocabForge are reflected in the reader immediately.


  5.4  Audio Player & Bookmarks
  ------------------------------
  When audio is linked to a book, a player bar appears at the bottom of the
  reader with:

    Play / Pause button
    Seek bar with clickable timestamps
    Current time and total duration
    Bookmark button — drops a marker at the current playback position
    Playback speed control (e.g. 0.75x for shadowing practice)

  Bookmarks appear as small markers on the seek bar. Click any marker to
  jump back to that timestamp. Audio is persisted in IndexedDB across
  browser restarts.


  5.5  Difficulty Badge
  ----------------------
  A small floating badge sits in the bottom-right corner of the reader.
  It shows the estimated comprehension percentage for the current chapter
  and changes colour based on difficulty:

    Green   Easy        < 20% unknown words
    Yellow  Optimal     20–45% unknown
    Orange  Challenging 45–65% unknown
    Red     Hard        > 65% unknown

  Click the badge to expand it. The expanded panel shows:

    Comprehension %   Estimated % of chapter text you know
    Difficulty %      % of highlights below Level 4
    Chapter column    Vocab word count in this chapter
                      + VF button to open chapter words in VocabForge
    Book column       Total vocabulary across the whole book
                      + CSV button to download all book highlights
    Level bar         Visual breakdown of L1/L2/L3/L4/L5 counts
    Level chips       Click any chip (L1–L5) to filter the reader so only
                      words at that level are highlighted

  Ignored words are excluded from all counts.


  5.6  Unique Words Sidebar
  --------------------------
  Toggle with the "Unique" button in the reader topbar.

  Shows every vocabulary word appearing in the current chapter (or the whole
  book), with frequency counts. Controls:

    Chapter / Book tab    Switch between chapter-level and book-level scope
    Frequency slider      Hide words that appear more than N times
                          (removes common, low-value words from view)
    Coverage stat         What % of the chapter's running words are in
                          your CSV (95%+ is comfortable reading level)
    Coverage trend chart  Sparkline of coverage across recent chapters
    Mine All Visible      Send all listed words to Words Mining in one click
    Download CSV          Export the word list as a CSV file
    Grid View             Open an interactive visual grid in a new tab


  5.7  Highlights Panel
  ----------------------
  Toggle with the "Highlights" button in the reader topbar.

  Shows all highlighted words in the current chapter with level badges,
  frequency counts, and checkboxes for bulk selection.

  Controls:

    Level filter strip    Show only words at L1, L2, L3, L4, or L5
    Search box            Filter the list by word text
    Select-all checkbox   Select all visible words for bulk actions
    Bulk actions:
      Level Down          Drop all selected words one level
      Level Up            Advance all selected words one level
      Mastery             Set all selected words to Level 5
      Hide / Unhide       Toggle highlight visibility (without ignoring)
    Per-row hide button   Hide one word's highlight on hover
    Grid View             Open the highlights as a flashcard grid


  5.8  Rules Panel
  -----------------
  Toggle with the "Rules" button in the reader topbar.

  Shows all Connected Speech rules that match text in the current chapter.
  Rules are detected by scanning the raw chapter source, so the panel works
  correctly even when Connected Speech mode is active (which replaces text
  in the DOM).

  Each rule row shows:

    Original phrase → Connected form
    Category badge (colour-coded)
    Hit count — how many times the rule triggered in this chapter
    Edit button (pencil) — opens an inline editor for that rule
    Delete button (X) — removes the rule after confirmation

  Inline edit fields:

    Original phrase    The written form to match
    Connected form     The spoken form to display
    Category           Reduction / Assimilation / Linking / Elision /
                       Contraction / Intrusion / Custom
    Note               Optional explanation or phonetic note

  "Manage All Rules" button at the bottom navigates to My Vocab → Rules.


  5.9  Dictionary Lookup & Word Peek
  ------------------------------------
  Dictionary Lookup (toggle: Alt D)
    When enabled, a "Dict" button appears in each word tooltip. Press it
    (or press Shift while the tooltip is open) to fetch the definition from
    your configured external dictionary URL. The result appears in the
    Dictionary sidebar on the right. A "Hover Dictionary" mode (Alt H)
    can auto-fetch definitions as you hover over words.

  Word Peek (toggle: Alt W)
    Shows a floating mini-definition when hovering over highlighted words,
    without opening the full tooltip. Good for quick glances while reading
    at normal speed.


  5.10 Keyboard Shortcuts (summary)
  -----------------------------------
  Full reference is in Section 12. Quick overview:

    Alt + S    Toggle Sidebar Tooltip mode
    Alt + C    Toggle Click-to-Show Tooltip
    Alt + D    Toggle Dictionary Lookup
    Alt + W    Toggle Word Peek
    Alt + H    Toggle Hover Dictionary
    Alt + K    Toggle Connected Speech mode
    Alt + F    Open Connected Form popup (select text first)

    (With tooltip open)
    1          Drop word one level
    2          Level up word
    3          Master word (Level 5)
    M          Toggle Focus
    I          Toggle Ignore
    E          Open inline edit
    P          Pin / unpin tooltip
    Shift      Dictionary lookup
    Esc        Dismiss tooltip


================================================================================
  6. VOCABFORGE — SPACED REPETITION STUDY
================================================================================

VocabForge is the built-in SRS (spaced repetition system) study module.
Load words from any source and study them in one of four modes:

  Cards           Browse your word set, read definitions, and manually
                  level words up or down.

  Flashcard       Flip cards to reveal pronunciation and definition.
                  Self-grade after each reveal.

  Quiz            Type the definition (or pronunciation) from memory.
                  Graded immediately; wrong answers lower the word's level.

  Multiple Choice Pick from four options. Distractors are drawn from other
                  words in your active set for realistic challenge.

Loading words into VocabForge:

  Source                        How to load
  ---------------------------   ----------------------------------------
  Chapter highlights            Difficulty Badge > VF button (Chapter)
  All book highlights           Difficulty Badge > Book column
  CSV deck                      Core tab > deck card > VF button
  Specific level                Click a level chip on the Difficulty Badge

Filters available during study:

  All / New / Studying / Mastered   Show only words with that status
  Hide Common                       Suppress words appearing > 8× in chapter
  Search                            Filter the card list by word text

Every study card shows a real context sentence harvested from the chapter
text, so you always see words in their natural habitat.

The stats bar at the top of VocabForge shows word counts per status (New /
Studying / Mastered) and overall progress at a glance.


================================================================================
  7. MY VOCABULARY
================================================================================

The My Vocab tab has five sub-sections for managing your learning data.


  7.1  Weak Words
  ----------------
  Words you have failed multiple times in Quiz, Flashcard, or Multiple
  Choice sessions. Useful for targeted re-study.

  Controls:
    Fail Threshold slider   Set how many failures make a word "weak"
                            (default: 3 failures)
    Refresh button          Recompute the list from current session data

  Each word card shows: word text, accuracy %, fail count, last studied.


  7.2  Focus Words
  -----------------
  Words you have manually starred using the Focus button (shortcut: M) in
  the reader tooltip. Acts as a personal "pay attention to this" list.

  Controls:
    Clear all    Remove all focus words at once
    X per row    Remove individual words from the list


  7.3  Words Mining
  ------------------
  A temporary scratchpad for capturing interesting words as you read,
  separate from your permanent CSV decks.

  Quick Capture form fields:
    Word *         Required — the word or phrase
    Pronunciation  Optional IPA or phonetic form
    Definition     Optional definition

  Press "+ Mine" or hit Enter to save. Mined words are highlighted in the
  reader just like CSV words, so you notice them as you keep reading.

  Limits:
    500 words maximum
    Entries older than 7 days are automatically purged on load
    Duplicate words are rejected

  Buttons:
    Download CSV   Export as word,pronunciation,definition CSV — ready
                   to re-import as a permanent vocabulary deck
    How it works   Toggle an inline tutorial panel
    Clear all      Wipe the entire mining list

  Note: mined words are a scratchpad, NOT permanent storage. Export to
  CSV if you want to keep them long-term.


  7.4  Mastered Words
  --------------------
  All words that have reached Level 5 across all your CSV sets and
  VocabForge sessions — your personal hall of fame.

  Controls:
    Import Mastery Words   Upload a CSV or TXT file; all words in the
                           file are immediately set to Level 5
    Export CSV             Download your full mastery list with
                           pronunciation and definition columns
    Search box             Filter the list by word or definition text
    Per page               Show 20, 50, or 100 words per page

  The stats panel at the top shows the total mastered count and a
  breakdown by source CSV deck.


  7.5  Connected Speech Rules
  ----------------------------
  Manage rules that describe how spoken language differs from writing.
  These rules power the Connected Speech overlay in the reader.

  Each rule has:
    Original phrase   The written form that appears in text
    Connected form    The spoken form (how it actually sounds)
    Category          Reduction / Assimilation / Linking / Elision /
                      Contraction / Intrusion / Custom
    Note              Optional explanation

  Examples:
    "want to"   →  "wanna"   (Reduction)
    "going to"  →  "gonna"   (Reduction)
    "did you"   →  "didja"   (Assimilation)
    "at all"    →  "atal"    (Linking)

  Adding rules:

    From the reader:
      1. Select text in the chapter
      2. Press Alt + F to open the Connected Form popup
      3. Enter the connected form and press Save

    Manual form (this tab):
      Click "+ Add Rule" and fill in the fields

    CSV upload:
      Click "Upload CSV" — format is: original,connected form,note
      All rows are assigned the category you choose in the import dialog

  Controls per rule:
    Toggle switch   Enable or disable the rule without deleting it
    Edit (pencil)   Open inline editor for that rule
    Delete (X)      Remove the rule permanently

  Sort options:  Date added / A–Z / Hit count
  Filter by category using the category pills

  Category colours are fully customisable — click any colour swatch
  in the category colour section at the bottom of this tab.


================================================================================
  8. CORE TAB — SETTINGS & BACKUP
================================================================================

The Core tab handles global settings and data management.

  Vocabulary Deck Manager
  -----------------------
  Lists all currently loaded CSV sets with word counts. Per deck:
    VF button     Open this deck in VocabForge
    CSV button    Download the original CSV file
    X button      Remove the deck from the session

  Backup & Restore
  ----------------
  All your data can be exported as a single JSON file at any time.

  What a backup includes:
    All CSV vocabulary sets
    VocabForge study progress (per-word levels and status)
    Words Mining list
    Ignored words (manual + CSV)
    Focus words
    Coverage trend data across chapters
    Connected Speech rules and category colour overrides
    Reader settings (theme, font, all toggles)

  Download Backup    Saves a .json file to your downloads folder
  Restore Backup     Select a previously saved .json to replace all
                     current data with the backup contents

  IMPORTANT: Restoring a backup overwrites your current data completely.
  Always download a fresh backup before restoring an old one.


================================================================================
  9. READER SETTINGS
================================================================================

Open the Settings panel with the gear icon (⚙) in the reader topbar.

  9.1  Themes
  ------------
  Ten built-in colour themes — four light, six dark:

    Dark           Classic dark background, red accent
    Warm Paper     Warm cream light theme (default light)
    Nord           Muted blue-grey dark theme
    Solarized      Deep teal dark theme, blue accent
    Forest         Dark green theme
    Midnight       Deep navy dark theme, blue accent
    Ivory          Warm off-white light theme, terracotta accent
    Sage           Soft green light theme
    Obsidian       Near-black with purple accent
    Amber          Very dark warm theme with amber accent


  9.2  Fonts
  -----------
  Ten reader fonts, all with CJK fallbacks (Japanese, Chinese, Korean):

    Source Sans    Clean humanist sans-serif (default)
    Serif          Lora — elegant book serif
    Garamond       EB Garamond — classic humanist serif
    Playfair       Playfair Display — high-contrast editorial serif
    IBM Plex       IBM Plex Serif — modern technical serif
    Literata       eBook-optimised serif
    Crimson        Crimson Pro — scholarly Renaissance-style serif
    Baskerville    Libre Baskerville — timeless transitional serif
    Spectral       Contemporary digital serif
    Serif JP       Noto Serif JP-first (best for Japanese text)

  Font size and line height are adjustable with sliders in the same panel.


  9.3  Connected Speech Mode
  ---------------------------
  Toggle with the "Connected Speech" switch (Alt K) in the Settings panel.

  When active, Covenant overlays your Connected Speech rules on the chapter
  text, replacing the written form with the spoken form inline:

    Written:   "I want to go to the store."
    CS Mode:   "I wanna go to the store."

  Gloss mode (separate toggle):
    Instead of replacing the text, shows the connected form as a small
    superscript above the original word, so both forms are visible.

  Alt + F (with text selected) opens the Connected Form popup to quickly
  add a new rule from text you have highlighted while reading.


  9.4  Ignored Words CSV
  -----------------------
  Upload a plain-text or CSV file containing words that should NEVER be
  highlighted, regardless of which vocabulary CSV is loaded.

  Useful for very high-frequency words (e.g. "the", "is", "have") that
  you already know perfectly and don't want cluttering the highlight view.

  The ignored-words list is separate from the "Ignore" action on individual
  words in the tooltip. Both are respected.


================================================================================
  10. SESSION STATS
================================================================================

At the end of each chapter, a "Chapter Completed" button appears at the
bottom of the text. Clicking it shows a summary of your reading session:

  Level Ups     How many words you advanced at least one level during
                this reading session
  Mastered      How many words you moved to Level 5 this session
  Words studied Total number of distinct words you interacted with

A progress bar shows the estimated percentage of chapter words currently
at Level 4 or above (i.e. words you effectively know).

Session counts reset each time you load a new chapter.


================================================================================
  11. DATA & PRIVACY
================================================================================

Covenant stores ALL data locally in your browser. Nothing is ever sent to
a server, and no internet connection is required once the app is open
(fonts may load from Google Fonts on first visit).

  Storage used:

    IndexedDB     Book files (parsed HTML chapters), cover images, audio
    localStorage  Vocabulary progress, settings, rules, mining list,
                  ignored words, focus words, bookmarks, coverage trends

  Important warnings:

    - Clearing your browser's site data WILL erase all Covenant data.
    - Private / Incognito mode may not persist data between sessions.
    - Use "Download Backup" regularly to protect your progress.
    - To move data between computers, use Download Backup on the old
      machine and Restore Backup on the new one.


================================================================================
  12. KEYBOARD SHORTCUTS REFERENCE
================================================================================

  Reader Toggles
  --------------
  Alt + S    Sidebar Tooltip mode (tooltip shows in a side panel, not float)
  Alt + C    Click-to-Show Tooltip (require click, not hover)
  Alt + D    Dictionary Lookup (enable Dict button in tooltip)
  Alt + W    Word Peek (mini hover definition)
  Alt + H    Hover Dictionary (auto-fetch on hover)
  Alt + K    Connected Speech mode on / off
  Alt + F    Open Connected Form popup (select text in reader first)

  Tooltip — Word Actions
  ----------------------
  1          Drop word to previous level
  2          Level up word
  3          Master word (jump to Level 5)
  M          Toggle Focus (star for study list)
  I          Toggle Ignore (remove highlight)

  Tooltip — Controls
  ------------------
  E          Open inline edit mode
  P          Pin / unpin tooltip (keeps it open while you read)
  Shift      Dictionary lookup (requires Dictionary Lookup to be enabled)
  Esc        Dismiss / unpin tooltip

  Inline Edit Mode
  ----------------
  Enter      Save changes (in single-line fields)
  Esc        Cancel edits without saving
  Tab        Move between fields


================================================================================
  END OF README
================================================================================

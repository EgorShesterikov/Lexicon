<p align="center">
  <a href="https://htmlpreview.github.io/?https://github.com/EgorShesterikov/Lexicon/blob/main/Lexicon.html">
    <img src="Icons/lexicon-banner.svg" alt="Lexicon — English vocabulary" width="100%">
  </a>
</p>

[![release](https://img.shields.io/github/v/release/EgorShesterikov/Lexicon)](../../releases)
[![release date](https://img.shields.io/github/release-date/EgorShesterikov/Lexicon)](../../releases)
[![last commit](https://img.shields.io/github/last-commit/EgorShesterikov/Lexicon)](../../commits)
[![license](https://img.shields.io/github/license/EgorShesterikov/Lexicon)](LICENSE.md)

<p>
  <a href="https://htmlpreview.github.io/?https://github.com/EgorShesterikov/Lexicon/blob/main/Lexicon.html">
    <img src="https://img.shields.io/badge/%E2%96%B6%20Launch%20the%20app-Open%20in%20browser-7a2321?style=for-the-badge" alt="Launch the app in the browser">
  </a>
</p>

<p><b>English</b> | <a href="README.ru.md">Русский</a></p>

An app to record, group and memorize English words. It is a single HTML file — it opens right in the browser, with no installation, server or internet (except for the automatic word look-up).

## Quick launch

You don't have to download anything — click the banner above or the **▶ Launch the app** button to open it straight in your browser.

- **Instant, no setup** — the launch link opens the file through [htmlpreview](https://htmlpreview.github.io). Great for a quick look.
- **Offline** — download `Lexicon.html` and open it with a double click; everything works without internet except the automatic look-up.

## Features

- **Dictionary.** Words are sorted automatically by part of speech. Each word has a translation, transcription (IPA) and pronunciation.
- **Adding words.** One at a time (with auto-filled translation, transcription and audio) or in bulk — as a list, with a review-and-edit window before saving.
- **Multiple meanings.** All translation variants are pulled in, grouped by part of speech; you pick the one you need.
- **Groups.** Your own sets of words to review (for example, by lesson).
- **“Cards” game — three modes.** *Repetition* (flip the card as much as you like, single “Next word”, no statistics), *Test* (type the answer; flipping the card counts as a mistake; optional per-group timer with unique time stats), and *Random* (fresh random English words from an online database with a “knew / didn’t know” rating, added to your dictionary automatically). English↔Russian, flip, audio, per-word accuracy and a list of mistakes at the end.
- **Statistics.** Accuracy and repetition count per word; separate “hard words” and “not studied yet” modes.
- **Two languages.** English or Russian interface, switchable from the header (⚙️ area); English by default, and your choice is remembered.
- **Accessibility.** Full keyboard control, screen-reader support and a reduced-motion mode.
- **Backup.** Export and import the dictionary as CSV, and reset all data — in the settings menu (⚙️).

## Run locally

Open `Lexicon.html` with a double click in any modern browser (Chrome, Edge, Firefox). For convenience you can make a shortcut with the icon from the `Icons` folder.

## Language

The interface language is switched with the **EN / RU** toggle in the header. English is the default; the choice is saved in the browser. The learning direction stays English → Russian regardless of the interface language.

## Data storage

The dictionary and groups are saved in the browser's `localStorage` (key `vocab_app_v1`) and survive a restart. Data is tied to the browser on a specific computer — use CSV export/import to move it.

## Technology

Plain HTML, CSS and JavaScript with no build step and no external libraries. The automatic look-up uses free, key-less services:

- [Free Dictionary API](https://dictionaryapi.dev) — transcription, pronunciation, part of speech;
- [MyMemory](https://mymemory.translated.net) and the public Google Translate endpoint — translation and meaning variants by part of speech.

## Limitations

- The automatic look-up needs the internet; when the services are unavailable, the fields are filled in by hand.
- When ready-made audio is missing, pronunciation is synthesized by the browser voice (Web Speech API).

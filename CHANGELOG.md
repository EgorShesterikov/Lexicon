# Lexicon

## 1.0.6 - 12.08.2026

The dictionary and the groups list are now split into pages when there are a lot of items — 50 words per page and 10 groups per page. The « ‹ › » controls with an "X–Y of Z" counter appear both above and below the list, so you can page through without scrolling to the end. Search, filter and sort jump back to the first page, and reordering a group or creating a new one follows it to whichever page it lands on — so a long collection stays quick to render and easy to page through.

## 1.0.5 - 12.08.2026

Dictionary search now puts an exact match first. If your query exactly matches a word or one of its translations, that entry is shown at the top, with the remaining partial matches below it.

Large dictionaries and groups scroll smoothly now. Off-screen rows are skipped by the browser until you reach them, row actions share a single handler instead of one per row, and search is debounced — so long lists no longer stutter while scrolling or typing.

## 1.0.4 - 12.08.2026

Groups can be reordered: each group has up and down arrows to move it in the list, and the new order is saved. The name search now shows up as soon as you have more than a couple of groups, so it's easier to find the one you want.

## 1.0.3 - 12.08.2026

A word that works as more than one part of speech is now kept as a separate entry for each one. Re-adding a word under a different part of speech creates its own card instead of piling the new meanings onto the entry you already had, so "run" the verb and "run" the noun sit in their own sections with their own translations. Adding the same word under a part of speech it already has still merges the translation as before.

Fixed the page backdrop shifting shade between tabs: the dark background is now pinned to the window, so it looks identical on the long Dictionary list and the shorter Add, Groups and Cards tabs instead of the Dictionary standing out.

## 1.0.2 - 12.08.2026

Adding a batch of words is safer now: the review window no longer closes if you misclick the dimmed area behind it or press Escape. Instead it asks whether to discard the words you've prepared, so a stray click can't wipe out a long list you were about to add.

## 1.0.1 - 11.08.2026

The "Cards" game is now three modes. Repetition lets you flip through cards freely with no pressure and no stats. Test asks you to type the answer — flipping the card counts as a mistake — and an optional per-group timer saves your best time only for a flawless run. Random pulls fresh words from an online database, rates them "knew / didn't know", and adds each one to your dictionary automatically. Every card shows the part of speech, plays audio, and auto-shrinks long words or translations so nothing ever spills over the edge.

Groups are much easier to manage: lists stay collapsed until you open them, there's a name search once you have many, and a quick "Add words" dialog builds a group with checkboxes, live search and a part-of-speech filter. The "Learn" button drops you straight into the Cards setup with the group already selected.

The dictionary got smarter too — search by first letter or by substring, sort by newest, and re-adding a word you already have now merges the translation instead of duplicating it. Rounding it out: tidier button tabs and native-feeling in-app dialogs throughout.

## 1.0.0 - 11.08.2026

First public release!

An app to record, group and memorize English words. It is a single HTML file — it opens right in the browser, with no installation, server or internet (except for the automatic word look-up).

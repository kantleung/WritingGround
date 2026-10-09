---
name: long-form-prose
description: Write and archive a multi-chapter prose work with continuity of argument, chronology, tone, and terminology. Use when the user wants a book, a chapter sequence, or the next chapter of an existing project in an Obsidian vault or project folder. Do not use for a single essay, letter, or note.
---

# Long-form prose

Use this skill only for a work of more than one chapter, or when the user points at an existing project folder. The system prompt still governs accuracy, British English, and style. The soul still governs voice.

## Start

If there is no outline on disk, write one and stop.

`00_Project/Outline_v0.1.md`:

- the single argument of the book, in one sentence
- chapter list with a one-line job for each chapter
- names, terms, and dates that must stay stable
- what is contested in the record

Ask the user to accept or revise the outline. Do not write Chapter 1 in that same turn.

## Once the outline is accepted

Proceed. Do not ask for permission before each chapter. Do not ask for feedback at the end of a chapter. Write the next missing chapter, save it, and stop so the user can read it.

A chapter is done when it has:

- carried the book’s argument one step
- kept chronology, names, and terms consistent with the outline and earlier chapters
- marked any thin or contested point in the prose, not in a footnote apology
- ended on a sentence that makes the next chapter necessary

## Files

Root: the vault or folder the user names. If none is named, create `Prose_<TitleSlug>/` in the working directory and say so.

```
00_Project/     outline, style sheet, decisions
01_Chapters/    Chapter_01_v0.1.md, ...
02_Notes/       sources, discarded openings, continuity log
```

Version. Do not overwrite. After each save, give the path.

Keep `00_Project/Continuity_v0.1.md` current: terms, ages, dates, and any decision that a later chapter must not contradict. Read it before writing the next chapter.

## Revision

If the user marks a chapter, revise that chapter only, as `_v0.2`, with a short note of what moved. Do not silently rewrite earlier chapters to match a new whim. If a revision breaks continuity, say which earlier file must change and wait.

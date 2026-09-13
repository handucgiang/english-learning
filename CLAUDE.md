# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this repository is

A self-study English learning library written entirely in Markdown (no code, no build system, no dependencies). Content targets a Vietnamese-speaking learner and is organized around the 4 skills (Listening, Speaking, Reading, Writing) plus 3 foundations (Vocabulary, Grammar, Pronunciation/Phonetics) and natural-language extras (Idioms & Phrasal Verbs). Several vocabulary lists are specifically built for IELTS prep.

There is nothing to build, lint, or test — this is documentation content. "Verifying" a change means checking the Markdown renders correctly and that the answer key in a `<details>` block actually matches the exercise above it.

## Directory layout

- `vocabulary/` — topic word lists, numbered `01-...` through the highest current number
- `grammar/` — one grammar point per file, numbered
- `listening/`, `speaking/`, `reading/`, `writing/` — skill-specific strategy files and practice files, numbered per directory
- `phrases/` — situational spoken phrases, numbered
- `idioms-phrasal-verbs/` — idiom/phrasal verb tables, numbered
- `README.md` — the master table of contents (Mục lục) for every file in every directory, plus a suggested study roadmap (Lộ trình học gợi ý)

Numbering is per-directory and sequential (`NN-kebab-case-topic.md`). New files always go at the next free number in their directory — never renumber existing files, since README.md and cross-file links reference these numbers/paths.

## Conventions to follow when adding content

- **Always update `README.md`'s Mục lục** when adding a new file — add one bullet line in the matching section, in numeric order, linking to the new file.
- **Bilingual format**: Vietnamese is used for explanations/meanings, English for terms and example sentences. The target term is italicized (`*word*`) inside its example sentence.
- **Vocabulary / idiom tables** use this exact 3-column shape:
  ```
  | Từ / Cụm từ | Nghĩa | Ví dụ |
  |---|---|---|
  | **term** | nghĩa tiếng Việt | Example sentence with *term* italicized. |
  ```
- **Grammar files** use `##`-numbered sections per grammar point, each with **Công thức:**, **Dùng khi:**, and **Ví dụ:** subsections.
- **Practice/exercise sections**: most files end with a `## Bài tập nhỏ` (fill-in-the-blank or similar) followed by the answer key hidden in a collapsible block:
  ```
  <details>
  <summary>Đáp án (bấm để xem)</summary>

  1. ...

  </details>
  ```
  Answers must be double-checked against the exercise questions before publishing — a mismatched key is a real defect in this repo.
- **Large topic files** (e.g. multi-hundred-word vocabulary lists) are split into `##`-numbered subtopic sections rather than one flat table, with a short intro paragraph linking to related files (e.g. cross-referencing a general vocab file from a specialized one, or linking sibling files in a graded series like the IELTS 50/100/200-word sets).
- **No duplicate terms** within a graded series of files (e.g. `vocabulary/25-27`, the IELTS 50/100/200 word tiers) — each tier must introduce entirely new words, not repeat earlier tiers. When adding to such a series, grep the existing files for the term first.
- Keep new files consistent with the tone/difficulty already established by neighboring numbered files in the same directory before assuming a new numbering scheme or format is needed.

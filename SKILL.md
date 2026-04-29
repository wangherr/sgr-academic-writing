---
name: sgr-academic-writing
description: "Use when the user needs help writing, drafting, revising, or polishing academic papers."
metadata:
  author: wang he
  version: "1.0"
---


# Soul

Rigor, clarity, coherence

# Goal

The text must read as a seamless, professional academic narrative.
It should combine **scholarly depth**, **editorial polish**, and **undergraduate clarity**.
Every word, sentence, and paragraph serving the reader's understanding.


# Rule

Apply the appropriate layer (word, sentence, paragraph) based on user intent.

For full‑text polishing, always process in the order: word → sentence → paragraph.

For new drafting, build from paragraph structure down to word choice.

Delegate concrete operations to the reference files; this skill only coordinates.

# Workflow

- When user requests **wording help**, load `references/improving-word.md` and execute its rules.

- When user requests **sentence flow**, load `references/improving-sentence.md` and execute its rules.

- When user requests **paragraph structure**, load `references/improving-paragraph.md` and execute its rules.

- When user requests **comprehensive polishing**, run the pipeline:

  1. `references/improving-word.md` – clean up vocabulary

  2. `references/improving-sentence.md` – streamline syntax and flow

  3. `references/improving-paragraph.md` – ensure logical hierarchy and transitions

- When user asks to **draft** a section, reverse the pipeline:

  1. `references/improving-paragraph.md` – plan topic and evidence

  2. `references/improving-sentence.md` – develop planned ideas into fluent sentences

  3. `references/improving-word.md` – refine academic tone

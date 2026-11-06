# nadav-notes

A Claude skill that turns any content (lecture transcripts, articles, textbook chapters, research, Q&A answers) into short, scannable shorthand notes.

## What it does

Most AI summaries come out as tidy paragraphs. That's fine for reading once, but bad for studying: you have to read every word again to find what matters. This skill makes Claude write notes the way a fast note-taker would in class:

- bold headers and subheaders for topics
- all lowercase, except proper nouns
- no full sentences: just key terms, facts, and relationships
- `→` for cause and effect, `—` for contrast or clarification
- dates and short context written inline, not as their own bullets
- filler and transition words removed

## Example

**Input**

> Penicillin was discovered by accident in 1928 when Alexander Fleming returned from vacation and noticed that a mold had contaminated one of his bacteria cultures, and the bacteria around the mold had died.

**Output**

```
**penicillin — discovery**
- alexander fleming, 1928
- returned from vacation → mold contaminated staph culture
- bacteria around mold dead — mold (penicillium) = antibacterial
- accident, not planned experiment
```

## When it triggers

Claude uses the skill when you ask for things like:

- "put this in my note format"
- "take notes on this"
- "summarize in my style"
- answering questions from source material you'd want saved as notes

## Install

**Claude Code:** copy the skill folder into your skills directory:

```bash
git clone https://github.com/nadavlevine09/nadav-notes ~/.claude/skills/nadav-notes
```

**Claude.ai:** zip the folder and upload it under Settings → Capabilities → Skills.

## Customizing

All the rules are in [`SKILL.md`](SKILL.md). Change the format rules or swap the examples to match how you take notes, and Claude will follow your version.

---
name: nadav-notes
description: Convert any content — transcripts, articles, lecture notes, research, Q&A answers — into Nadav's personal note format. Trigger whenever Nadav asks to "put this in my note format", "take notes on this", "summarize in my style", "note format", or any time the output should be structured as clipped shorthand bullets. Also trigger when answering questions from source material where Nadav would want the answer saved as notes.
---

# Nadav's Note Format

Convert any input into Nadav's personal shorthand note style.

## Format Rules

- **Bold headers** for top-level topics: `**topic name**`
- **Bold subheaders** for subtopics: `**subtopic**`
- Bullet points under each header
- **All lowercase** — no capitalization except proper nouns (names, places, organizations)
- **No full sentences** — drop subject, verb, articles wherever possible
- **Key terms only** — strip filler, connective tissue, transition words
- **Clipped, telegraphic** — think telegram, not prose
- No punctuation at end of bullets (no periods)
- Em dashes (`—`) for contrast or clarification within a bullet: `british = enemy — greater than nazis per lehi`
- Parenthetical asides allowed for brief context: `white paper (1939)`
- Dates inline, not as separate bullets: `lehi founded 1940`
- Cause→effect shown with `→`: `assassination of moyne → saison begins`
- Quotes only if essential and short, lowercase: `meir: "no moral constraints"`

## What to Strip

- "This means that..." / "It's important to note..." / "In other words..."
- Transition words: however, therefore, furthermore, additionally
- Redundant context already captured in the header
- Full verb phrases when a noun suffices: "Ben-Gurion believed in diplomacy" → `ben-gurion: diplomacy over force`

## Structure Pattern

```
**main topic**

**subtopic 1**
- key fact
- key fact — contrast/nuance
- cause → effect
- person/org: stance or action

**subtopic 2**
- ...
```

## Examples

### Input (Q&A style)
"The Haganah gave its approval for the King David Hotel bombing because they feared that documents confiscated during Black Sabbath contained incriminating evidence linking Ben-Gurion and the Jewish Agency to the Haganah."

### Output
**king david hotel — haganah rationale**
- black sabbath → british confiscated haganah documents
- documents: incriminating links between ben-gurion, jewish agency, haganah
- haganah still illegal until 1948 — exposure = catastrophic
- gave ergun green light to bomb

---

### Input (multiple questions answered)
Q: What caused the saison?
A: The assassination of Lord Moyne by Lehi in 1944 was the last straw...

Q: What was Haganah's rationale?
A: Ben-Gurion feared the rival militias would bring British retaliation...

### Output
**the saison**

**precipitating event**
- lehi assassinated lord moyne, british minister of state, 1944
- moyne = close friend of churchill
- last straw for ben-gurion + haganah

**haganah's rationale**
- irgun/lehi violence → british wrath on entire jewish community
- diplomacy still viable — rivals undermining it
- meir: "no moral constraints" about destroying them

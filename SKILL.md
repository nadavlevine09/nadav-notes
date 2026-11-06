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
- Em dashes (`—`) for contrast or clarification within a bullet: `mitochondria = energy — not the only organelle with own dna`
- Parenthetical asides allowed for brief context: `calvin cycle (light-independent)`
- Dates inline, not as separate bullets: `penicillin discovered 1928`
- Cause→effect shown with `→`: `stomata close → co2 intake drops`
- Quotes only if essential and short, lowercase: `fleming: "one sometimes finds what one is not looking for"`

## What to Strip

- "This means that..." / "It's important to note..." / "In other words..."
- Transition words: however, therefore, furthermore, additionally
- Redundant context already captured in the header
- Full verb phrases when a noun suffices: "Fleming noticed that mold killed the bacteria" → `fleming: mold killed bacteria`

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
"Penicillin was discovered by accident in 1928 when Alexander Fleming returned from vacation and noticed that a mold had contaminated one of his bacteria cultures, and the bacteria around the mold had died."

### Output
**penicillin — discovery**
- alexander fleming, 1928
- returned from vacation → mold contaminated staph culture
- bacteria around mold dead — mold (penicillium) = antibacterial
- accident, not planned experiment

---

### Input (multiple questions answered)
Q: What happens in the light-dependent reactions?
A: In the thylakoid membranes, chlorophyll absorbs light, which splits water and produces ATP and NADPH...

Q: What does the Calvin cycle do?
A: Using the ATP and NADPH from the light reactions, the Calvin cycle in the stroma fixes CO2 into sugar...

### Output
**photosynthesis**

**light-dependent reactions**
- location: thylakoid membranes
- chlorophyll absorbs light → water split
- byproduct: o2 released
- outputs: atp + nadph → feed calvin cycle

**calvin cycle**
- location: stroma (light-independent)
- uses atp + nadph from light reactions
- co2 fixed → glucose
- rubisco = key enzyme — most abundant protein on earth

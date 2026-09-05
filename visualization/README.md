# Villa visualisation package

Produced from five CAD sheets (`Facade.pdf`, `ground_floor.pdf`, `first_floor.pdf`,
`roof_and_second_floor.pdf`, `landscape.pdf`). Three documents, read in order:

| File | What it is |
|---|---|
| [`SPEC.md`](SPEC.md) | **Phase 1.** The factual sheet. Every room, opening, setback, the pool, the parking, the yard depths, the derived heights. Each value is flagged ✅ dimensioned / ⚠️ measured / ❓ uncertain. Nothing is invented. |
| [`IDENTITY.md`](IDENTITY.md) | **Phase 2.** A 328-word locked description of the building as a photographer sees it. |
| [`PROMPTS.md`](PROMPTS.md) | **Phase 3.** Twelve standalone, production-ready text-to-image prompts for ChatGPT / GPT Image, plus a global negative list, a ten-point consistency crib, and a record of every deliberate departure from the drawings. |

## How the drawings were read

Each PDF was rasterised at 200 DPI (300–600 DPI for details) and inspected visually. In
parallel, the vector geometry was pulled straight out of the PDF content streams, so most
values in `SPEC.md` are exact drawing geometry rather than pixel estimates.

A scale was derived per sheet and then verified against *every* printed dimension on that
sheet — 56 dimensions in total, all reproducing exactly. The four plan sheets were
registered to one another on the 0.40 m structural columns, which coincide exactly.

`Facade.pdf` carries no dimension lines at all. Its scale was derived and then confirmed
against five independent horizontal features that match the plans exactly (bay width, stone
reveal, glazed panel width, entrance portal width, door leaf width). Every height in this
package descends from that derivation and is flagged as measured, never dimensioned.

## Quick start

1. Run `PROMPTS.md` → **P01**. That is the anchor image.
2. Attach the accepted P01 frame to every later prompt.
3. Check each result against the ten-point crib in `PROMPTS.md` §3 before accepting it.

## Open questions for the author

`SPEC.md` §6 lists eight ambiguities in the drawing set — the most consequential being the
front glazing width conflict between plan and elevation, the stair strip drawn outside the
ground-floor wall line, and the complete absence of any height dimension, section, north
point or material schedule.

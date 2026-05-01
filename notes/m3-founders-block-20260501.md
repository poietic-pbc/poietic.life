# M3 fix: founders block on poietic.life landing page

Date: 2026-05-01
Task: m3-fix-founders
Commit: 5b21176 (poietic-pbc/poietic.life main)

## Where the founders section was placed

Inserted as a new top-level section between the mission section
(`#mission`) and the "what we've built" section (`#built`). The mission
section carries the public-benefit operating purpose paragraph, so this
position satisfies the spec ("between the public benefit statement and
the 'What we've built' cards").

Section numbering was updated from `01/03 ... 03/03` to
`01/04 ... 04/04`:

- `01/04` mission
- `02/04` founders   <-- new
- `03/04` what we've built
- `04/04` get involved

A `founders` link was added to the top nav between `mission` and
`what we've built`. The dark monospace aesthetic is preserved: founder
cards reuse the existing card border / surface / hover treatment,
the section header uses the same `## section-title` pattern, and the
serif italic accent is used for inline tool names (`vg`,
`CRISPResso2`, `The Uncertainty Mindset`).

## Exact text used for each founder

### Erik Garrison

> University of Tennessee Health Science Center
>
> Created *vg*, the foundational pangenomics toolkit (~72,000 Google
> Scholar citations across the toolkit), and built PGGB, the pangenome
> graph builder used by the Human Pangenome Reference Consortium.
> Author on Nat Biotechnol 2018 and Nat Methods 2024. WorkGraph
> architect and lead developer.

### Luca Pinello

> Massachusetts General Hospital / Harvard Medical School / Broad Institute
>
> Built *CRISPResso2*, the standard for CRISPR editing analysis
> (18,700+ citations). His group's CRISPRme independently identified an
> off-target in the BCL11A guide that became Casgevy, informing the FDA
> review. Built Chorus to orchestrate genomic AI models.

### Vaughn Tan

> Honorary Professor, UCL School of Management
>
> Author of *The Uncertainty Mindset* (Columbia University Press,
> 2020). PhD in Organizational Behavior from Harvard. Researches how
> hybrid teams operate under uncertainty, the organizational question
> WorkGraph is built to answer.

## Constraints honored

- No em-dashes anywhere in the new content.
- No "PI" / "lead PI" / "principal investigator" language.
- C.Origami / Chromnitron not mentioned anywhere (would have been a
  misattribution to Luca).
- CRISPRme / Casgevy framing uses "independently identified" with no
  language implying direct collaboration with the company that
  commercialized Casgevy.
- Single HTML file, no build step. Pure CSS additions slotted into the
  existing `<style>` block; new section uses existing utility classes.

## Render confirmation

- HTML tag balance verified (no unclosed elements at end of parse;
  apparent SVG self-closing-tag warnings are spurious).
- Local diff shows only additions inside `index.html`: 149 insertions /
  7 deletions, all confined to nav, the new section, and the section
  index numbers.
- Rebased cleanly onto the 3 newer remote commits (mobile responsive
  fixes) without conflicts. The new founder cards inherit `.section`
  padding, so the mobile padding fix from `15ce9fa` applies for free.
- Pushed to `origin/main` at commit `5b21176`. GitHub Pages will
  rebuild and serve the updated `https://poietic.life/` shortly.

## Git commit hash

`5b21176` on `poietic-pbc/poietic.life`, branch `main`.

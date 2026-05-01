---
fix_id: H1
target_section: 29
target_word_cap: 200
status: ready-for-assembly
source_task: fix-h1-29-add
source_review: notes/v3-review-synthesis-20260501.md
---

# fix-h1: §29 add adoption metric numbers

## Criticism

Verbatim from `notes/v3-review-synthesis-20260501.md` §3 high-value table:

> | H1 | §29 | Adoption metric named without a number; §46 says 50+ but §29 does not | Replace "Lab adoption is the falsifiable external metric." with "Lab adoption is the falsifiable external metric (target: 10+ adopter labs by month 18, 50+ by month 36)." |

Restated in this task's brief:

> §29 names 'lab adoption is the falsifiable external metric' without numbers. §46 says 50+ but §29 doesn't carry the specifics. Sympathetic reviewer wants explicit numbers.

## Target section + word cap

- **Section:** 29 (Theory of change)
- **Word cap:** 200 words (per CLAUDE.md, "Section 29: 200 words")
- **Current count:** 199 (one-word headroom)

## Current text (verbatim from v3 at 70c8e7f)

> 29. Theory of change (200 words)
>
> The chain by which this grant produces public benefit has links we control upstream and links we do not control downstream. We are honest about both.
>
> Upstream: WorkGraph is at minimum-viable maturity today, used daily by the founders. The grant funds hardening it for outside labs and a longitudinal deployment across the founders' active genomics programs (Garrison's pangenomics and HPRC work, Pinello's clinical genomics), producing real research outputs (preprints, software releases, datasets) coordinated through auditable computation graphs. Lab adoption is the falsifiable external metric.
>
> Middle: when labs adopt and stay, hybrid human-AI genomics work becomes more reliable. Errors are caught earlier, provenance is traceable, results reproduce across operators and machines. This matters most in reference-resource construction, where errors and biases propagate to thousands of downstream studies, and in clinical genomics, where misinterpretation has direct patient consequences.
>
> Downstream: better science contributes to clinical and translational benefit. We do not promise specific clinical outcomes inside 36 months. The chain is real but indirect, and the PBC mission ("make human and machine collaboration legible and responsive to its participants") is what we operationalize directly. Downstream public benefit follows from credible reference resources and reproducible clinical analyses, not from this grant's outputs alone.

## Proposed text

> 29. Theory of change (200 words)
>
> The chain has upstream links we control and downstream links we do not. We are honest about both.
>
> Upstream: WorkGraph is at minimum-viable maturity today, used daily by the founders. The grant funds hardening it for outside labs and a longitudinal deployment across the founders' active genomics programs (Garrison's pangenomics and HPRC work, Pinello's clinical genomics), producing real research outputs (preprints, software releases, datasets) coordinated through auditable computation graphs. Lab adoption is the falsifiable external metric (target: 10+ adopter labs by month 18, 50+ by month 36).
>
> Middle: when labs adopt and stay, hybrid human-AI genomics work becomes more reliable. Errors are caught earlier, provenance is traceable, results reproduce across operators and machines. This matters most in reference-resource construction, where errors and biases propagate to thousands of downstream studies, and in clinical genomics, where misinterpretation has direct patient consequences.
>
> Downstream: better science contributes to clinical and translational benefit. We do not promise specific clinical outcomes inside 36 months. The chain is real but indirect, and the PBC mission ("make human and machine collaboration legible and responsive to its participants") is what we operationalize directly. Public benefit follows from credible reference resources and reproducible clinical analyses, not this grant alone.

## Diff

Three localized edits, all inside §29:

1. **Para 1 (intro):**
   ```
   - The chain by which this grant produces public benefit has links we control upstream and links we do not control downstream. We are honest about both.
   + The chain has upstream links we control and downstream links we do not. We are honest about both.
   ```
   Removes "by which this grant produces public benefit" (redundant with the section heading "Theory of change" and with §29's downstream framing) and reorders so "upstream links we control" / "downstream links we do not" sit adjacent to the Upstream/Middle/Downstream paragraph cues that follow. Net: 26 → 18 words (-8).

2. **Para 2 (Upstream), final sentence — the criticism's specified action:**
   ```
   - Lab adoption is the falsifiable external metric.
   + Lab adoption is the falsifiable external metric (target: 10+ adopter labs by month 18, 50+ by month 36).
   ```
   Net: 7 → 18 words (+11).

3. **Para 4 (Downstream), final sentence:**
   ```
   - Downstream public benefit follows from credible reference resources and reproducible clinical analyses, not from this grant's outputs alone.
   + Public benefit follows from credible reference resources and reproducible clinical analyses, not this grant alone.
   ```
   Drops the leading "Downstream" (already redundant with the paragraph's "Downstream:" cue) and tightens "from this grant's outputs alone" to "not this grant alone". Net: 18 → 15 words (-3).

Net change across §29: -8 + 11 - 3 = 0 words. Final count 199, unchanged.

## Word count check

| Version | Words | Cap | Margin |
|---|---|---|---|
| Current (v3) | 199 | 200 | +1 |
| Proposed | 199 | 200 | +1 |

Counts produced by `wc -w` on the full §29 paragraph block (heading line excluded). The "(target: 10+ adopter labs by month 18, 50+ by month 36)" insertion adds 11 words; the para 1 trim recovers 8 and the para 4 trim recovers 3, for net zero.

A version that *only* applies the minimal substitution from the criticism's action (without the para 1 / para 4 trims) lands at 210 words and breaches the cap by 10. That version is rejected.

## Constraint compliance check

- Word cap respected (199 ≤ 200). ✓
- No em-dashes introduced. The proposed text uses commas, periods, parentheses, and one semicolon-free comma split. ✓
- No PI / lead-PI language. Founders referenced as "the founders" and by surname (Garrison, Pinello). ✓
- No v1 terms (KRAS, MRTX1133, Boltz, RFdiffusion, DiffDock, pancreatic cancer, drug discovery). ✓
- No recursion claim ("drafted using WorkGraph", "incorporated using WorkGraph", "we wrote this proposal with WorkGraph"). The §29 phrase "used daily by the founders" is the defensible CLAUDE.md item #10 framing and is preserved unchanged. ✓
- CRISPRme / Casgevy framing precise: not present in §29 (lives in §17a, §35, §36); unaffected. ✓
- DNA-Diffusion not in funded scope: not present in §29; unaffected. ✓
- Founder order Erik / Luca / Vaughn: §29 mentions Garrison's pangenomics work first, then Pinello's clinical genomics, in the same Erik-then-Luca order; unchanged. Vaughn is not name-checked in §29 in either version. ✓
- Internal consistency with §46 (§46 cites "50+ adopter labs by month 36"): §29 now matches that figure verbatim and adds the month-18 milestone, which is consistent with the timeline language in §22. ✓
- Internal consistency with §30: §30's mitigation sentence "lab adoption is the falsifiable external metric" stays accurate; the figures are introduced in §29 and need not be repeated in §30's 100-word block. ✓

## Rationale

The criticism is a sympathetic-reviewer ask: §29 names lab adoption as the falsifiable external metric but leaves "falsifiable" hanging without a number a panel can compare future state against. §46 carries the "50+ adopter labs by month 36" figure, but a reviewer reading §29 in isolation (which a Google.org panel does, section by section) sees an unfalsifiable claim and a credibility hit follows. Adding the month-18 milestone alongside the month-36 figure also addresses the synthesis's secondary observation O2 ("§22: tie computation-graph dataset milestone to a date and adopter count"), since §29's adoption ramp now mirrors the §22 timeline structure without duplicating §22's content.

The change is non-trivial because §29 is already at 199 of 200 words. A literal application of the action's substitution overshoots by 10 words, so the spec must propose a trim that lands the criticism without breaching the cap or pulling in scope creep. The two trims chosen (para 1 intro and para 4 closing sentence) are inside the same section as the substitution, target only redundant phrasing relative to the section heading and paragraph cues, and preserve every load-bearing element of §29's argument: upstream/middle/downstream structure, the honest framing, the lab-adoption as falsifiable metric, the "we do not promise specific clinical outcomes inside 36 months" hostage-of-fortune disclaimer, the PBC mission quotation, and the indirect-chain framing in the closing line. No other v3 sections are touched. The deterministic assembler can apply the diff as a triple in-section edit confined to §29.

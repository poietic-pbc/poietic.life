---
fix_id: H6
target_section: "§19c (changes from baseline)"
target_word_cap: 75
status: ready
---

# Fix H6: §19c BioBench claim soften

## Criticism (verbatim from synthesis)

> H6 | §19c | "BioBench established as the open standard" is implausible in 36 months | Soften to "BioBench actively used as a public benchmark by ≥3 external groups"

Source: `~/poietic.life/notes/v3-review-synthesis-20260501.md` row H6.

## Target section + word cap

§19c (changes from baseline expected). Cap: 75 words (per CLAUDE.md word-limit table for §19a/§19b/§19c).

## Current text (verbatim from v3, commit 70c8e7f)

> 19c. The changes from baseline we expect to see are... (75 words)
>
> Today, AI-assisted research produces outputs without auditable processes; reference-resource construction lacks systematic provenance; clinical genomics analyses cannot easily be reconstructed by independent reviewers. By project end: computation graph publication as routine practice for at least some genomics venues; a community of independent labs using WorkGraph for sustained hybrid research; ethnographic case studies grounding the organizational design framework; and BioBench established as the open standard for evaluating agentic biology systems.

## Proposed text

> 19c. The changes from baseline we expect to see are... (75 words)
>
> Today, AI-assisted research produces outputs without auditable processes; reference-resource construction lacks systematic provenance; clinical genomics analyses cannot easily be reconstructed by independent reviewers. By project end: computation graph publication as routine practice for at least some genomics venues; a community of independent labs using WorkGraph for sustained hybrid research; ethnographic case studies grounding the organizational design framework; and BioBench actively used as a public benchmark by ≥3 external groups.

Single-clause change: replace "BioBench established as the open standard for evaluating agentic biology systems" with "BioBench actively used as a public benchmark by ≥3 external groups".

## Word count check

Sentence-by-sentence (hyphenated compounds counted as one token; "≥3" counted as one token):

- Sentence 1 (unchanged): "Today, AI-assisted research produces outputs without auditable processes; reference-resource construction lacks systematic provenance; clinical genomics analyses cannot easily be reconstructed by independent reviewers." → 23 words.
- Sentence 2 lead-in (unchanged): "By project end: computation graph publication as routine practice for at least some genomics venues; a community of independent labs using WorkGraph for sustained hybrid research; ethnographic case studies grounding the organizational design framework;" → 34 words.
- Sentence 2 final clause:
  - Before: "and BioBench established as the open standard for evaluating agentic biology systems." → 12 words.
  - After: "and BioBench actively used as a public benchmark by ≥3 external groups." → 12 words.

Total:
- Before: 23 + 34 + 12 = 69 words.
- After: 23 + 34 + 12 = 69 words.
- Cap: 75 words.
- Margin: 6 words under cap. ✓

Constraint pass:
- No em-dashes. ✓
- No PI language. ✓
- No v1 terms (KRAS, MRTX1133, Boltz, RFdiffusion, DiffDock, pancreatic cancer). ✓
- No recursion claim ("drafted using WorkGraph"). ✓
- CRISPRme/Casgevy framing: not invoked here. ✓
- DNA-Diffusion: not invoked here. ✓
- Founder order: not invoked here. ✓

## Rationale

The criticism is that "BioBench established as the open standard for evaluating agentic biology systems" is implausible as a 36-month outcome: SWE-bench took years and a sustained community organising effort to become the de-facto coding-agent benchmark, and there are already several attempts (LAB-Bench, BioCoder, BiomedBench) competing for the agentic-biology slot. Promising "the" open standard in three years invites the skeptical reviewer to score the entire outcomes block as overpromising, which contaminates the credibility of the other (more defensible) claims in §19c. The synthesis's suggested replacement, "actively used as a public benchmark by ≥3 external groups," lands the criticism cleanly: it preserves the BioBench deliverable as a real outcome of the grant, replaces a category-defining claim with a measurable adoption claim that can be verified by counting external research groups submitting evaluations, and matches the calibration of the other three end-state claims in the same sentence (each of which is already specified as "at least some," "a community of," and "ethnographic case studies" — i.e., bounded adoption rather than category dominance). The ≥3-external-groups bar is also internally consistent with §43–§46 milestone language ("at least 10 pilot labs," "10+ adopter labs"), so a panel reviewer reading §19c against the milestone plan will see one coherent adoption story rather than a milestone plan that promises pilot-lab counts and an outcomes block that promises category capture. Word count is preserved exactly (12-word clause replaced by a 12-word clause), so no other text in §19c needs to shift.

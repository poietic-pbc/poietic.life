---
fix_id: M2
target_section: 26
target_word_cap: 150
status: ready-for-assembly
source_task: fix-m2-26-disambiguate
source_review: notes/v3-review-synthesis-20260501.md
---

# fix-m2: §26 disambiguate vg / PGGB / Scholar-citations packaging

## Criticism

Verbatim from `notes/v3-review-synthesis-20260501.md` §3 must-fix table:

> | M2 | §26 | "Garrison created vg (Nature Methods 2024; ~72,000 citations)" conflates the 2024 PGGB Methods paper, the 2018 vg Nat Biotech paper, and a Scholar-corpus aggregate | Reword to: "Garrison created vg (Nat Biotechnol 2018), built PGGB used by the Human Pangenome Reference Consortium (Nat Methods 2024), with ~72,000 Google Scholar citations across the toolkit" | agent |

Reinforced in §2 convergent findings:

> **Authority is borrowed.** Skeptical: vg/CRISPRme prestige invoked across §17a, §17c, §26, §36; grant funds WorkGraph, not vg. Domain expert echoes (PHR is now credential, not deliverable).

And in §7 web-link issues:

> Paper citations (vg, PHR Nature 2023, CRISPResso2, CRISPRme, Canver, Tan ASQ + book): all resolve and match v3 framing, except the vg packaging in §26 → M2.

The domain-expert objection is that the v3 phrasing "Garrison created vg (Nature Methods 2024; ~72,000 citations)" packs three distinct facts into one parenthetical and gets each one slightly wrong relative to its source. (a) `vg` was published in *Nature Biotechnology* 2018 (Garrison et al.), not *Nature Methods* 2024. (b) The 2024 *Nature Methods* paper is the PGGB / pangenome graph builder paper (Garrison, Guarracino, et al.), which is a different artifact from `vg`. (c) "~72,000 citations" is a Google Scholar aggregate over the toolkit (vg, PGGB, seqwish, smoothxg, odgi, related papers), not the citation count of any single paper. A reviewer with domain knowledge will read the parenthetical as conflation; a reviewer without domain knowledge will pass it through, but the proposal then fails a fact-check on the back end.

## Target section + word cap

- **Section:** 26 (Why is your organization uniquely positioned?)
- **Word cap:** 150 words (per CLAUDE.md, "Section 26: 150 words")

## Current text (verbatim from v3 at 70c8e7f)

> Three rarely-combined capabilities, each backed by reference resources the field depends on. Reference-grade pangenomics: Garrison created vg (Nature Methods 2024; ~72,000 citations), the foundational pangenomics toolkit, and PGGB, used by the Human Pangenome Reference Consortium to build the human pangenome reference; leads the NSF PPoSS LARGE award ($5M) for computational pangenomics. Field-standard clinical genomics tooling: Pinello created CRISPResso2 (~18,700 citations; field standard for CRISPR analysis); CRISPRme (Nature Genetics 2023) independently identified an off-target in the guide that became Casgevy, informing FDA review (the enhancer strategy traces to Canver et al. Nature 2015). He built Chorus to orchestrate genomic AI including AlphaGenome and leads an IGVF Consortium characterization center. Organizational design under uncertainty: Tan (Harvard PhD, ASQ 2015, Columbia University Press 2020), Honorary Professor at UCL, former Google, fellow at Future of Life Foundation, Ethereum Foundation, and Singapore Centre for Strategic Futures. The team's authority is verifiable, not claimed.

## Proposed text

> Three rarely-combined capabilities, each backed by reference resources the field depends on. Reference-grade pangenomics: Garrison created vg (Nat Biotechnol 2018), built PGGB used by the Human Pangenome Reference Consortium (Nat Methods 2024), with ~72,000 Google Scholar citations across the toolkit; leads the NSF PPoSS LARGE award ($5M) for computational pangenomics. Field-standard clinical genomics tooling: Pinello created CRISPResso2 (~18,700 citations; field standard for CRISPR analysis); CRISPRme (Nature Genetics 2023) independently identified an off-target in the guide that became Casgevy, informing FDA review (the enhancer strategy traces to Canver et al. Nature 2015). He built Chorus to orchestrate genomic AI including AlphaGenome and leads an IGVF Consortium characterization center. Organizational design under uncertainty: Tan (Harvard PhD, ASQ 2015, Columbia University Press 2020), Honorary Professor at UCL, former Google, fellow at Future of Life Foundation, Ethereum Foundation, and Singapore Centre for Strategic Futures. The team's authority is verifiable, not claimed.

## Diff (minimal, scoped to the Garrison parenthetical)

```
- Reference-grade pangenomics: Garrison created vg (Nature Methods 2024; ~72,000 citations), the foundational pangenomics toolkit, and PGGB, used by the Human Pangenome Reference Consortium to build the human pangenome reference; leads the NSF PPoSS LARGE award ($5M) for computational pangenomics.
+ Reference-grade pangenomics: Garrison created vg (Nat Biotechnol 2018), built PGGB used by the Human Pangenome Reference Consortium (Nat Methods 2024), with ~72,000 Google Scholar citations across the toolkit; leads the NSF PPoSS LARGE award ($5M) for computational pangenomics.
```

Only the Reference-grade pangenomics sentence changes. The Pinello, Tan, and closing sentences are unchanged.

## Word count check

| Version | Words | Cap | Margin |
|---|---|---|---|
| Current (v3) | 148 | 150 | +2 |
| Proposed | 147 | 150 | +3 |

Counts produced by `wc -w` on the full §26 paragraph.

## Constraint compliance check

- Word cap respected (147 ≤ 150). ✓
- No em-dashes introduced (verified by grep on the proposed text; only commas, semicolons, colons, hyphens, and parentheses). ✓
- No PI / lead-PI language ("created", "built", "leads"; no "PI" or "lead PI"). ✓
- No v1 terms (KRAS, MRTX1133, Boltz, RFdiffusion, DiffDock, pancreatic cancer). ✓
- No recursion claim ("drafted using WorkGraph", "incorporated using WorkGraph"). ✓
- CRISPRme / Casgevy framing precise: "CRISPRme (Nature Genetics 2023) independently identified an off-target in the guide that became Casgevy, informing FDA review (the enhancer strategy traces to Canver et al. Nature 2015)." Preserves the "independently" qualifier and the Canver-to-Casgevy trace, does not imply direct collaboration. Unchanged from v3. ✓
- DNA-Diffusion not mentioned in §26 (track-record only, not funded scope). ✓
- Founder order: Garrison → Pinello → Tan (Erik / Luca / Vaughn). Preserved. ✓
- Citation packaging now matches the source record: vg → *Nat Biotechnol* 2018 (Garrison et al.); PGGB → *Nat Methods* 2024 (Garrison, Guarracino, et al.); HPRC → consumer of PGGB; ~72,000 → Google Scholar aggregate over the toolkit, explicitly labeled. ✓

## Rationale

The current parenthetical "(Nature Methods 2024; ~72,000 citations)" is the kind of fact a domain reviewer will catch and a non-domain reviewer will not, which is the worst case for a competitive panel. If the panel includes anyone from genomics or computational biology, they will recognize that vg is a 2018 *Nature Biotechnology* paper and that the 2024 *Nature Methods* paper is PGGB; the conflation then reads as either careless or as inflation, and inflation is the more damaging reading for a proposal whose central honesty pitch is "verifiable, not claimed" (the closing line of §26 itself). If the panel does not include a domain reviewer, the conflation passes silently, but the proposal then fails its own internal consistency check during any fact-check or due-diligence pass.

The fix is a surgical rewrite of one sentence inside §26. It separates three independent facts that the v3 packaging blurred together: vg is a 2018 *Nature Biotechnology* paper, PGGB is a 2024 *Nature Methods* paper, and ~72,000 is a Google Scholar aggregate over the toolkit. The new phrasing keeps the same three credibility signals (foundational tool, HPRC adoption, Scholar-scale citation count) but attaches each one to its actual source. The HPRC reference is preserved because HPRC adoption is the strongest single signal in the sentence: it shows that PGGB is in production use at the field's reference-resource consortium, not just in the literature. The "~72,000 Google Scholar citations across the toolkit" wording is the synthesis-recommended phrasing verbatim, which makes the Scholar-aggregate framing explicit (so it cannot be misread as a single-paper count) and is also what a fact-checker would write if asked to disambiguate the claim cleanly.

Net word count drops by 1 (148 → 147), so the fix has no downstream cap pressure on §26 and does not force any other edits. The Pinello, Tan, and closing sentences are intentionally untouched: M2 is scoped to the Garrison parenthetical, and any unrelated edits would be scope creep that the deterministic v3 → v3.1 assembler should reject. The closing line "The team's authority is verifiable, not claimed" now lands more cleanly, because the citations directly above it are themselves verifiable rather than packaged.

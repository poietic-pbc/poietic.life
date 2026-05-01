---
fix_id: M1
target_section: 36
target_word_cap: 100
status: ready-for-assembly
source_task: fix-m1-36-commit
source_review: notes/v3-review-synthesis-20260501.md
---

# fix-m1: §36 commit count "93+" → "2,000+"

## Criticism

Verbatim from `notes/v3-review-synthesis-20260501.md`:

> **§36 "93+ commits"** is wrong (live: 2,094). Trivial fix, real credibility hit if caught.

Reinforced in the §3 must-fix table:

> | M1 | §36 | "MIT, 93+ commits" (live count is 2,094, ~22x off) | Replace with "MIT, 2,000+ commits" or drop the count entirely; license + URL is enough | agent |

And in §7 web-link issues:

> `github.com/graphwork/workgraph`: 200 OK, content matches; commit count drift ("93+" vs 2,094) → M1.

## Target section + word cap

- **Section:** 36 (Public presence)
- **Word cap:** 100 words (per CLAUDE.md, "Sections 20, 21, 23, 25, 28, 30, 35, 36: 100 words each")

## Current text (verbatim from v3 at 70c8e7f)

> WorkGraph is publicly available at github.com/graphwork/workgraph (MIT, 93+ commits). Co-founders have extensive public profiles. Garrison: vg ecosystem (~72,000 citations, Nature Methods 2024), pseudo-homologous regions (Nature 2023), HPRC contributions. Pinello: CRISPResso2 (~18,700 citations, Nature Biotechnology), CRISPRme (Nature Genetics 2023, off-target identified independently in the BCL11A guide before Casgevy FDA approval), Chorus framework, IGVF Consortium center. Tan: *The Uncertainty Mindset* (Columbia University Press 2020), Administrative Science Quarterly 2015, recent Future of Life Foundation fellowship on AI for Human Reasoning. Longitudinal case-study outputs and computation-graph archives will be published openly with interactive reports.

## Proposed text

> WorkGraph is publicly available at github.com/graphwork/workgraph (MIT, 2,000+ commits). Co-founders have extensive public profiles. Garrison: vg ecosystem (~72,000 citations, Nature Methods 2024), pseudo-homologous regions (Nature 2023), HPRC contributions. Pinello: CRISPResso2 (~18,700 citations, Nature Biotechnology), CRISPRme (Nature Genetics 2023, off-target identified independently in the BCL11A guide before Casgevy FDA approval), Chorus framework, IGVF Consortium center. Tan: *The Uncertainty Mindset* (Columbia University Press 2020), Administrative Science Quarterly 2015, recent Future of Life Foundation fellowship on AI for Human Reasoning. Longitudinal case-study outputs and computation-graph archives will be published openly with interactive reports.

## Diff (minimal)

```
- (MIT, 93+ commits)
+ (MIT, 2,000+ commits)
```

Single token-level change. No other text in §36 is touched.

## Word count check

| Version | Words | Cap | Margin |
|---|---|---|---|
| Current (v3) | 90 | 100 | +10 |
| Proposed | 90 | 100 | +10 |

Counts produced by `wc -w` on the full paragraph. The two strings "93+" and "2,000+" are each tokenized as a single word, so the count is unchanged.

## Constraint compliance check

- Word cap respected (90 ≤ 100). ✓
- No em-dashes introduced. ✓
- No PI / lead-PI language. ✓
- No v1 terms (KRAS, MRTX1133, Boltz, RFdiffusion, DiffDock, pancreatic cancer). ✓
- No recursion claim ("drafted using WorkGraph", "incorporated using WorkGraph"). The phrase "in daily use coordinating Garrison's ongoing pangenomics research" is in §29, not §36, and is the defensible version per CLAUDE.md item #10. ✓
- CRISPRme / Casgevy framing precise: "CRISPRme (Nature Genetics 2023, off-target identified independently in the BCL11A guide before Casgevy FDA approval)" — preserves the "independently" qualifier and does not imply direct collaboration with the Casgevy developer. Unchanged from v3. ✓
- DNA-Diffusion not mentioned in §36. ✓
- Founder order: Garrison → Pinello → Tan (Erik / Luca / Vaughn). Unchanged. ✓
- Repository URL `github.com/graphwork/workgraph` and MIT license are retained, so the credibility chain (license + URL) holds even if the count drifts again before submission. ✓

## Rationale

The criticism is binary and verifiable: a panel reviewer who clicks the cited URL sees the GitHub commit count, finds 2,094, and the proposal's "93+" reads as either careless or stale. M1 is graded as a "trivial fix, real credibility hit if caught" in the synthesis, and is the cheapest item on the must-fix list because it is a single-token substitution inside an existing §36 sentence with ten words of cap headroom.

The fix replaces "93+" with "2,000+" rather than dropping the number for two reasons. First, the count is load-bearing in §36's purpose — §36 is the "Public presence" answer, and a commit count is concrete evidence that the repository is active rather than a dormant placeholder. The license and URL alone show existence; the commit count shows activity. Second, "2,000+" is conservative against the live count (~2,094) and stays correct through several months of further commits, so it does not re-incur the same drift risk before the May 1 submission or during any post-submission review window.

The "+" suffix is preserved (matching the original "93+" formulation) so the claim is a lower bound rather than a snapshot, which is the form a reviewer should expect for an active repository. No other §36 content is touched: founder credentials, citation counts, CRISPRme/Casgevy framing, and the closing line on computation-graph archives are all intentionally left as-is, since they are not part of the M1 criticism and any unrelated edits would create scope creep that the deterministic assembler should reject.

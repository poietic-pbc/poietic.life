# v3.1 fanout assembly summary (2026-05-01)

Assembled `workgraph_google_application_FINAL_v3_1.md` at project root from v3 (commit 70c8e7f, worktree `wg/agent-77/v3-assemble-stitch`) plus all 12 fix specs.

## Criticism → edit map

| Criticism | Section(s) | Result |
|---|---|---|
| M1 | §36 | "93+" → "2,000+" commits |
| M2 | §26 | vg/PGGB/Scholar disambiguated |
| H1 | §29 | Adoption numbers folded into divergent-29 Version A |
| H2 | §17a | Superseded by W1 |
| H3 | §28 | Liverpool architectural-divergence sentence appended |
| H4 | §31 | Boilerplate sentence dropped (Option A) |
| H5 | §43 | impg 1.0 — superseded by W1 (preserved verbatim inside W1's rewrite) |
| H6 | §19c | BioBench softened — superseded by W1 |
| H7 | (no v3 text change) | Erik-only repo action — see TODOs |
| W1 | §17a/b/c/d, §19a/b/c, §43-46 | Substrate framing + named deliverables |
| divergent-29 | §29 | Version A (keep-honest, sharpened); supersedes H1 |
| O1 | §17c | Tan-research scope sentence layered on W1 |
| O2 | §22 | Tightening + m18/m36 milestone |
| O3 | §17d | BioBench definition layered on W1 |
| O4 | §11 | v2 title residue removed |
| O5 | §28 | Unlinked Tan reasoning-scaffold sentence dropped |

## Final word counts

75-cap: 16a 69, 16b 73, 16c 69, 17a 71, 17b 75, 17c 73, 17d 73, 18a 66, 18b 64, 18c 68, 19a 70, 19b 71, 19c 73.
100-cap: 20 89, 21 86, 23 97, 25 91, 28 91, 30 93, 35 86, 36 90.
150-cap: 26 147, 33 127.
200-cap: 29 198.
50-cap: 34a 47, 34b 45.
Milestones (~100): §43 83, §44 84, §45 100, §46 94.

All caps respected. §17b at 75/75 and §45 at 100/100 sit at exact cap.

## Conflicts resolved

1. **§17c (W1 + O1).** Naive composition 76/75. Dropped "Garrison et al., " from W1's HPRC citation in S2 (Garrison authorship is established in §26 and §36). Final 73/75.
2. **§17d (W1 + O3).** Compressed O3's BioBench definition to one sentence; dropped O3's second sentence (implicit in §18b); preserved W1's full high-risk-arc list. Final 73/75.
3. **§28 (H3 + O5; H7 = no change).** H3 (+19, -15) and O5 (-8) commute. Final 91/100.
4. **§29.** divergent-29 Version A folds H1 numbers in. Final 198/200.
5. **§43, §19c.** W1 supersedes H5 and H6.

## Style sweep — all clean

- 0 em-dashes; 0 PI/lead PI; 0 v1 terms (KRAS, MRTX1133, pancreatic, Boltz, RFdiffusion, DiffDock); 0 recursion claims
- DNA-Diffusion appears once, §30 disclosure, "outside funded scope"
- CRISPRme/Casgevy framing precise (3 mentions, all use "independently identified")
- Founder order Erik / Luca / Vaughn preserved
- Budget sums to $1,500,000 ($900k + $300k + $150k + $150k)
- Liverpool ack in §28 with H3 architectural-divergence sentence
- §30 "reviewers may want a specific scientific deliverable" risk preserved
- v2 (project root) and v3 (worktree, commit 70c8e7f) untouched

## TODOs for Erik

1. **H7 repo.** Recommended: GitHub-archive `phr-methodology-comparison` (same pattern as M4). Alt: stub README pointer.
2. **M4 (parallel).** Archive or repurpose `deep-research-competition` (v2 KRAS scaffold; STATE.md §3 "Pending").
3. **§42 / §47 form verification.** v3.1 skips both. Verify form schema before submission; supply content if required.
4. **Effort allocations.** §38 keeps allocations at "to be finalized at award" per CLAUDE.md. If form forces percentages, decide jointly with Luca and Vaughn.
5. **§28 Tan demo.** O5 dropped the unlinked October-2025 reasoning-scaffold sentence. Reinstate with citation only if a public link can be produced.
6. **Extended outline §17d high-risk-arc paragraph.** W1 specifies a 272-word paragraph for `workgraph_extended_outline_v2.md` documenting Pinello's research arc. Add to extended outline before public dissemination.

## How to choose v2 vs v3 vs v3.1

**v2** carried the PHR-discovery demonstration and a concrete 36-month deliverable (PHR atlas on undiagnosed rare-disease cohort). Reviewable as science-led but exposed Casgevy-precision and clinical-overclaim risks. **v3** dropped the PHR atlas in favor of "longitudinal deployment as substrate" — honest about what the grant buys, but reviewers (skeptical, domain-expert) flagged it as having no specific scientific output. **v3.1** keeps v3's substrate framing but restores named, co-authored 36-month deliverables (HPRC R3 build, impg 1.0, COSIGT and graph-augmentation papers, adaptive tracepoints integration, vg-CNV, PGGB v1.0, three MemPanG cohorts) drawn from Garrison's in-flight work, plus a high-risk-arc framing for Pinello's methodological breadth that respects the DNA-Diffusion COI. **Recommendation: submit v3.1.** It carries v3's honest theory of change (§29 sharpened to remove the five "hedge-read" phrases), satisfies the science-deliverable criticism with verifiable named artifacts, fixes M1/M2 fact errors, addresses every H- and O-row finding, and respects every word cap. v2 and v3 preserved untouched for diff and history.

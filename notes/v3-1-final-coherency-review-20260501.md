---
review_id: v3-1-final-coherency-review
date: 2026-05-01
target: workgraph_google_application_FINAL_v3_1.md
source_branch: wg/agent-201/v3-1-fanout-assemble (commit adc06f0)
verdict: submit-v3.1
---

# v3.1 final coherency review (2026-05-01)

## 1. Headline verdict

**Submit v3.1.** Every criticism in `v3-review-synthesis-20260501.md` is fixed in the document, supplied by the live landing page, or routed to a clear Erik-only repo action that does not gate submission. The dogfooding framing landed: the application reads as people who built and use this tool inside their own active research programs, not as people pitching infrastructure to hypothetical adopters. Word caps respected, budget sums correctly, style clean, founder order preserved, no v1 residue. Two repos still need archival (M4, H7) and §42 / §47 / certifications need Erik's eyes, but neither is a textual fix.

## 2. Criticism coverage table

| Item | Section(s) | v3.1 location | Verdict | Notes |
|---|---|---|---|---|
| M1 | §36 | line 268 | Fixed | "MIT, 2,000+ commits" |
| M2 | §26 | line 194 | Fixed | vg → Nat Biotechnol 2018; PGGB → Nat Methods 2024; ~72,000 → "Google Scholar citations across the toolkit" |
| M3 | poietic.life | landing page | Fixed elsewhere | `index.html` names Erik / Luca / Vaughn (commit `ce369c2`, agent-32). No application-text change required. |
| M4 | repo archival | external | Erik-only | `github.com/poietic-pbc/deep-research-competition` not yet GitHub-archived. Application text does not gate on this. |
| H1 | §29 | line 213 | Fixed | Adoption numbers folded into divergent-29 Version A. |
| H2 | §17a | line 95 | Fixed | "in daily use across the founders' labs" replaces "in production today" (subsumed by W1). |
| H3 | §28 | line 205 | Fixed | "Liverpool optimizes for lab-robotics scheduling and physical-experiment coordination; WorkGraph optimizes for git-native provenance across distributed human and computational actors." |
| H4 | §31 | line 229 | Fixed | "Initial conversations are underway" boilerplate dropped (Option A). |
| H5 | §43 | line 314 | Fixed | Named co-authored impg 1.0 deliverable (subsumed by W1). |
| H6 | §19c | line 149 | Fixed | "BioBench actively used as a public benchmark by 3+ external groups" replaces "open standard" overreach. |
| H7 | external repo | none in §28 | Erik-only | `phr-methodology-comparison` not archived. Application text lacks any "demonstration in motion" claim already. |
| W1 | §17a–d, §19a–c, §43–46 | multiple | Fixed | Substrate framing + named deliverables (HPRC R3, impg 1.0, COSIGT, graph-aug, MemPanG ×3, adaptive tracepoints, variant-calling, vg-CNV, PGGB v1.0). |
| divergent-29 (A) | §29 | line 209 | Fixed | Five hedge phrases removed; control-band structure preserved with we-deliver / we-enable / we-contribute parentheticals. |
| O1 | §17c | line 107 | Fixed | "Tan's research on hybrid teams under uncertainty (ASQ; Columbia University Press) provides the methodological frame." |
| O2 | §22 | line 169 | Fixed | "First public release by month 18, with contributions from at least 10 adopter labs by month 36." |
| O3 | §17d | line 113 | Fixed | "BioBench: an open benchmark of verifiable biology research challenges, distinct from prior SWE-bench-for-bio attempts." (compressed to fit cap; D4 high-risk-arc retained). |
| O4 | §11 | line 59 | Fixed | "WorkGraph: Open Coordination Infrastructure for Auditable, Hybrid Human-AI Work in Functional Genomics" |
| O5 | §28 | line 205 | Fixed | Unlinked Tan reasoning-scaffold demo sentence dropped. |

No uncovered criticisms. No cosmetic-only fixes.

## 3. Dogfooding framing audit

**The framing landed.** Erik asked for "we built this tool because we need it, we will use it constantly across our active research, our track records prove we know what useful infrastructure looks like." Five passages carry that load:

- §17a: "in daily use across the founders' labs ... matures the substrate that coordinates Garrison's ongoing pangenome work (PGGB, impg, HPRC Release 3) and Pinello's clinical genomics programs (CRISPRme, IGVF)." Active use, named deliverables.
- §17c: WorkGraph "in daily use coordinating Garrison's pangenome research, including the pseudo-homologous-region program."
- §18b: "the founders' own active research programs (Erik's reference-resource construction, Luca's clinical genomics analysis) drive WorkGraph's evolution: the tool serves real workflows, not invented ones." Cleanest dogfooding sentence in the document.
- §19a + §19b: named deliverables flow through founders' own audited workflows; failure mode is "founders themselves quietly reverting to ad-hoc tools." Failure-as-dogfooding-negation is the strongest possible signal.
- §43–§46: every milestone is a co-authored, in-flight Garrison-lab deliverable shipped through WorkGraph traces. Continued-use, not aspirational adoption.

§26 carries track record: vg + PGGB + HPRC + NSF PPoSS LARGE; CRISPResso2 + CRISPRme + Chorus + IGVF; Harvard PhD + ASQ + Columbia + UCL + Google + FLF + Ethereum + Singapore CSF. Closing "verifiable, not claimed" is earned.

**No edits proposed.** Framing is at appropriate strength for a panel reading at speed.

## 4. Internal consistency

Cross-checked §17 ↔ §26 ↔ §29 ↔ §43–§46. Chains hold.

- Garrison: §17a names PGGB / impg / HPRC R3 → §26 backs with vg / PGGB / HPRC / NSF PPoSS LARGE → §43 ships HPRC R3 + impg 1.0 → §44 ships COSIGT + graph-augmentation → §45 ships adaptive tracepoints + variant-calling best-practice → §46 ships vg-CNV + PGGB v1.0.
- Pinello: §17c cites CRISPRme → §26 backs with CRISPResso2 + CRISPRme + Chorus + IGVF → §43–§46 deliberately name no Pinello-led 36-month ship (DNA-Diffusion COI keeps Pinello inside substrate scope without a named software promise). Consistent with §30.
- Tan: §17d names case studies + framework → §44 "First Tan working paper" → §45 framework accepted at ASQ or Research Policy.
- Adoption: §29 / §19a / §46 all cite 10+ at m18, 50+ at m36. §22 dataset milestone uses the same cadence.
- §30 Risk #1 is now mitigated by §43–§46 named deliverables. Risk #4 contains DNA-Diffusion to disclosure-only.

No contradictions or drift found.

## 5. Hard checks

| Check | Result |
|---|---|
| §16a–c, §17a–d, §18a–c, §19a–c at ≤75 | Pass (max §17b at 75/75, §17c at 73, §17d at 73) |
| §20, §21, §23, §25, §28, §30, §35, §36 at ≤100 | Pass (max §23 at 97) |
| §26 at ≤150 | Pass (147) |
| §29 at ≤200 | Pass (198) |
| §33 at ≤150 | Pass (127) |
| §34a, §34b at ≤50 | Pass (47, 45) |
| §43–§46 at soft ~100 | Pass (86, 87, 98, 92 by manual recount) |
| Budget sums to $1,500,000 | Pass ($900k + $300k + $150k + $150k) |
| §37 funding request $1,500,000 | Pass |
| Em-dashes (— or `--`) | 0 found |
| PI / lead PI / Principal Investigator | 0 found |
| Founder order Erik / Luca / Vaughn | Preserved across §8/§9, §17a, §17c, §26, §28, §36, §38 |
| v1 terms (KRAS, MRTX1133, pancreatic, Boltz, RFdiffusion, DiffDock) | 0 found |
| Recursion claim ("drafted using WorkGraph", etc.) | 0 found |
| CRISPRme/Casgevy framing precise | Pass (3 mentions, all use "independently identified", no implication of direct collaboration) |
| DNA-Diffusion only in §30, outside funded scope | Pass (1 mention total, in §30 disclosure) |
| Liverpool ack present + architectural divergence | Pass (§28, two-sentence pair) |
| §30 "reviewers may want a specific scientific deliverable" risk | Preserved as Risk #1 |
| M3 founders on poietic.life | Live (Erik Garrison, Luca Pinello, Vaughn Tan named in `index.html`) |

## 6. Erik-only TODOs for submission

1. **M4 repo archival.** GitHub-archive `poietic-pbc/deep-research-competition` (Settings → Archive). Removes v1 KRAS framing from the org page.
2. **H7 repo archival.** Same action for `poietic-pbc/phr-methodology-comparison`. Application text already lacks any "demonstration in motion" claim.
3. **§42 / §47 form verification.** Skipped in v3.1 (form schema not visible to assembler). Confirm what the form asks; supply content during submission.
4. **§38 effort allocations.** Kept at "to be finalized at award" per CLAUDE.md item #6. If the form forces percentages, decide with Luca and Vaughn before submit.
5. **Section VII certifications (§48–§53).** Confirm each Yes/No matches the legal record before certifying.
6. **Attachments.** Budget worksheet, org documents, letters of support if the form expects them; none are in the markdown.
7. **Extended-outline §17d high-risk-arc paragraph.** W1 specifies a 272-word Pinello-arc paragraph for `workgraph_extended_outline_v2.md`. Add before public dissemination. Not a submission gate.
8. **§28 Tan reasoning-scaffold demo.** Dropped per O5. Reinstate only if a public link can be produced; otherwise leave dropped (CLAUDE.md item #10).

None block submission of the application markdown. Items 1, 2 are repo hygiene.

## 7. If hold-for-fixes

Not applicable. **Submission-ready.**

---

## Method note

Verified v3.1 (commit adc06f0, md5 f695874a6c5c4f8b76633023bb551ec9) against the synthesis and all twelve fix specs. Word counts checked programmatically and manually for borderline sections. Style sweep, budget sum, founder order, DNA-Diffusion containment, CRISPRme/Casgevy phrasing, Liverpool ack, and §30 risk preservation all confirmed. Read end-to-end against Erik's dogfooding instruction; no edits proposed.

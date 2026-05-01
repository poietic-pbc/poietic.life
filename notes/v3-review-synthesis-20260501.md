# v3 Review Synthesis (2026-05-01)

Synthesis of four reviews of `workgraph_google_application_FINAL_v3.md` (commit `70c8e7f`): link verification, sympathetic, skeptical, domain expert.

## 1. Headline verdict

**Submit v3 with must-fixes.** v3's spine (open infrastructure + longitudinal genomics deployment + falsifiable adoption metric) reads as honest to the sympathetic reviewer, viable to the domain expert, and is not disqualified by the skeptical reviewer (who attacks tone and specificity, not category). Blockers are small: one wrong number in §36, one ambiguous citation in §26, two public-web destinations (landing page, old org repo) that contradict authority claims. Fix those and submit v3. v2's PHR-atlas is a more vivid set piece, but its 36-month clinical promise is a hostage to fortune the team has decided to drop.

## 2. Convergent findings

### Strengths (reviewers agree or none object)
- **§16a problem framing.** "Session-scoped CLIs vs data-pipeline workflow managers" carves a defensible category in two sentences. Sympathetic flags it as strongest; skeptical does not attack; domain expert nods.
- **Team authority verifies.** vg/PGGB, CRISPResso2, CRISPRme, Tan's ASQ + book resolve to real artifacts. Domain expert: "unimpeachable."
- **CRISPRme/Casgevy framing is precise.** "Independently identified an off-target in the BCL11A guide that became Casgevy" is consistent with CLAUDE.md and matches Cancellieri et al. 2023. Keep as-is.
- **§19a failure signals are genuine.** "Founders themselves quietly reverting to ad-hoc tools" is the kind of metric most science grants do not write down. Skeptical concedes the structure.
- **No v1 residue.** KRAS/MRTX1133/Boltz are gone; cited papers match v3 framing.

### Weaknesses (most or all reviewers agree)
- **No specific science deliverable.** Skeptical: v2 named a PHR atlas, v3 dropped it without replacement. Domain expert: "what specific reference resource gets built better in 36 months? v3 has no answer." Sympathetic concedes a non-program-officer panelist may ask "what is the science we are buying?" Source of most other objections.
- **§36 "93+ commits"** is wrong (live: 2,094). Trivial fix, real credibility hit if caught.
- **§43–§46 milestones are vague.** Skeptical: "four vague claims, zero specifics." Domain expert wants a named co-authored deliverable by month 18.
- **BioBench is underspecified.** Sympathetic: "orphaned." Skeptical: "open standard in 36 months is implausible." §19c is the overreach.
- **Liverpool framing is asserted, not argued.** Both sympathetic ("underplayed") and skeptical ("closer to 'didn't we just fund this'") want one sentence on architectural divergence.
- **Authority is borrowed.** Skeptical: vg/CRISPRme prestige invoked across §17a, §17c, §26, §36; grant funds WorkGraph, not vg. Domain expert echoes (PHR is now credential, not deliverable).

## 3. Divergent findings (Erik decides)

- **v3 vs v2 overall.** Sympathetic prefers v3 (falsifiable, no clinical hostages). Skeptical thinks v3 lost the science deliverable v2 had. Domain expert: honest but less vivid. Question is which kind of panel reads this.
- **§29 theory of change.** Sympathetic: "unusually honest." Skeptical: "three paragraphs of hedge, reads as expecting to underdeliver." Same words, opposite read.
- **§30 risks ordering.** Skeptical wants "reviewers may want science deliverable" cut as defensive. Sympathetic does not object. The placement was deliberate, to pre-empt the predictable objection.
- **Infrastructure-as-deliverable.** Sympathetic thinks this is the right trade for a Google.org panel; skeptical and domain expert think it requires reviewer faith.

## 4. MUST FIX before submit (blockers)

| # | Section | Problem | Fix | Owner |
|---|---|---|---|---|
| M1 | §36 | "MIT, 93+ commits" (live count is 2,094, ~22x off) | Replace with "MIT, 2,000+ commits" or drop the count entirely; license + URL is enough | agent |
| M2 | §26 | "Garrison created vg (Nature Methods 2024; ~72,000 citations)" conflates the 2024 PGGB Methods paper, the 2018 vg Nat Biotech paper, and a Scholar-corpus aggregate | Reword to: "Garrison created vg (Nat Biotechnol 2018), built PGGB used by the Human Pangenome Reference Consortium (Nat Methods 2024), with ~72,000 Google Scholar citations across the toolkit" | agent |
| M3 | poietic.life (`index.html`) | Site cited as §5a "Website URL" does not list founders by name. v3 leans on founder credibility in §17c, §26, §36 | Add a founders section with three names + affiliations + one-line credibility (vg/PGGB; CRISPResso2/CRISPRme; *The Uncertainty Mindset*) | Erik (separate repo) or agent if delegated |
| M4 | `github.com/poietic-pbc/deep-research-competition` | Repo is still public with KRAS framing as first impression on the org page; `ARCHIVED.md` exists but the repo is not GitHub-archived | GitHub-archive the repo (adds the visible "Public archive" badge) or stub the README to a one-line pointer at `phr-methodology-comparison` | Erik (GitHub admin) |

## 5. HIGH VALUE if time permits

| # | Section | Problem | Fix |
|---|---|---|---|
| H1 | §29 | Adoption metric named without a number; §46 says 50+ but §29 does not | Replace "Lab adoption is the falsifiable external metric." with "Lab adoption is the falsifiable external metric (target: 10+ adopter labs by month 18, 50+ by month 36)." |
| H2 | §17a | "in production today" reads as overclaim against §28's "daily use across founder labs" | Replace "in production today" with "in daily use across the founders' labs" |
| H3 | §28 | Liverpool complementarity asserted, not argued | Append one sentence: "Liverpool optimizes for lab-robotics scheduling and physical-experiment coordination; WorkGraph optimizes for git-native provenance across distributed human and computational actors." |
| H4 | §31 | "Initial conversations are underway with clinical genomics programs" reads as boilerplate | Either name 1–2 programs or drop the sentence |
| H5 | §43 | "Methodology paper drafted as preprint" by month 6 is weak; domain expert wants a named co-authored deliverable | Commit to one named software release or one specific HPRC / pangenome curation paper as a month-18 deliverable |
| H6 | §19c | "BioBench established as the open standard" is implausible in 36 months | Soften to "BioBench actively used as a public benchmark by ≥3 external groups" |
| H7 | `phr-methodology-comparison` repo | 1 commit, region not selected as of submission day | Push at least one commit naming the region and species set OR remove "demonstration in motion" implications from §28 |

## 6. OPTIONAL polish

| # | Section | Suggestion |
|---|---|---|
| O1 | §17c | Acknowledge scope of Tan's research: "Tan's research on hybrid teams under uncertainty (ASQ; Columbia University Press) provides the methodological frame" |
| O2 | §22 | Tie computation-graph dataset milestone to a date and adopter count (sympathetic suggestion) |
| O3 | §17d / §29 | Two sentences on what BioBench is and how it differs from SWE-bench-for-bio attempts |
| O4 | §11 title | Assembler flagged this as v2 verbatim. Replace with: "WorkGraph: Open Coordination Infrastructure for Auditable, Hybrid Human-AI Work in Functional Genomics" |
| O5 | §28 | "Tan's reasoning-scaffold prototype demoed in October 2025" has no public link. Link or drop |

## 7. Web-link issues consolidated

- `poietic.life`: 200 OK, no founder names → M3.
- `github.com/graphwork/workgraph`: 200 OK, content matches; commit count drift ("93+" vs 2,094) → M1.
- `github.com/orgs/poietic-pbc`: 200 OK; `deep-research-competition` (KRAS) still leads the org page → M4.
- `graphwork.github.io`: 200 OK, matches v3 framing. No action.
- `github.com/poietic-pbc/poietic.life`: same content gap as poietic.life; fix via M3.
- `github.com/poietic-pbc/phr-methodology-comparison`: 200 OK; 1 commit, region pending → H7.
- Paper citations (vg, PHR Nature 2023, CRISPResso2, CRISPRme, Canver, Tan ASQ + book): all resolve and match v3 framing, except the vg packaging in §26 → M2.

## 8. v2 vs v3 final

| Dimension | v2 | v3 | Verdict |
|---|---|---|---|
| Scientific concreteness (named deliverable) | PHR atlas + named candidates in rare disease cohort | Longitudinal deployment + computation graph corpus | **v2** (but commits to outcomes outside team control) |
| Falsifiability of success | Atlas exists or it does not | Adoption count, computation graphs, BioBench participation | **v3** (adoption is genuinely falsifiable in 36 months) |
| Honesty / overclaim risk | Promises clinical candidates the team cannot guarantee | Drops clinical promises; explicit "we do not promise specific clinical outcomes" | **v3** |
| Team authority leverage | Same names, hooked to PHR-as-deliverable | Same names, authority risks reading as "borrowed" since deliverable shifted | **v2** marginally; v3 mitigates with the §17a longitudinal framing |
| Reviewer memorability (set piece) | Three-arm methodology comparison: concrete and easy to imagine | No equivalent set piece; computation-graph corpus is abstract | **v2** |
| Robustness to skeptical reading | Hostage to fortune on clinical candidates | Hedges in §29 / §30 invite "expecting to underdeliver" reading | **Tie**, different failure modes |

**Recommendation:** apply M1–M4 (must-fix) and ideally H1–H3 (~30 min editing), then submit v3. v3 is the right bet for a Google.org panel reading 600 proposals against the "AI for Science" frame; cost is one missing set piece. v2 is the fallback if a reviewer wants vivid concrete science.

If only one fix is possible: **M3** (founders on `poietic.life`). The credibility chain across §17c / §26 / §36 collapses if the website it cites does not name the people.

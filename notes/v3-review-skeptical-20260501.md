# v3 skeptical review (program officer mode)

**Headline.** "Infrastructure shop wants a research grant" pile. The science is whatever the founders publish anyway, and §30 admits it. v2 had a 36-month science deliverable; v3 dropped it but kept the science-prestige rhetoric.

(`v3-link-verification-20260501.md` does not exist at read time.)

## Overclaim hunt

- §17a: WorkGraph is "in production today." §28 more accurately calls it "functional and publicly available... in daily use across founder labs." Pick one register.
- §46: "WorkGraph adopted by 50+ labs with documented impact" by month 36 from zero external labs. vg took years.
- §19c: "BioBench established as the open standard for evaluating agentic biology systems," from "5+ community-contributed challenges" by month 18. Standard-establishment in 36 months is implausible.
- §46: "Computation graph publication recognized as practice in at least some venues" requires journal policy change. No editorial contact named.
- §16b: "AI accelerates output while degrading reproducibility." Asserted, not cited.
- §17c: Tan's hybrid-teams research is "published (Columbia University Press; ASQ)." The book is about food and innovation; ASQ 2015 is organizational uncertainty in adjacent domains. Neither covers hybrid human-AI scientific teams.

## Vague-claim hunt

- §17a: "longitudinal deployment of WorkGraph across the founders' active computational and clinical genomics programs, including the reference-resource construction work that underpins downstream science." Which programs, what scope? §29's "real research outputs (preprints, software releases, datasets)" gives no count.
- §29: "Lab adoption is the falsifiable external metric." No number. Milestone 4 says 50+. Name the number where you name the metric.
- §31: "Initial conversations are underway with clinical genomics programs." Boilerplate. Name them or drop it.
- §33: "informal advisory group spanning pangenomics, clinical genomics, computational biology, and open-science governance." Informal = uncommitted.
- §43: "Methodology paper drafted as preprint." Drafted, not submitted, in 6 months on a $1.5M grant is weak.

## §30 "where is the science" attack

Acknowledged, not answered. The mitigation ("every longitudinal case study produces a real research output... lab adoption is the falsifiable external metric") reads as "we will publish the papers we were going to publish anyway." Listing reviewer-mood as risk #1 telegraphs the weak point. v2 named a PHR atlas with diagnostic candidates as the 36-month deliverable. v3 dropped that without replacing it. Honest move: fund infrastructure on infrastructure terms, evaluate by adoption alone. Instead §17a, §17c, §26, §36 lean on vg and CRISPRme prestige while the science deliverables are gone.

## Authority gaps

- vg ~72,000 citations and HPRC: invoked in §17a, §17c, §26, §36. Grant funds WorkGraph, not vg. Borrowed authority.
- CRISPRme/Casgevy: invoked in §17c, §26, §36. Shows Pinello ships clinical-grade tools. Does not show WorkGraph improves clinical genomics. Causal link implicit.
- §28: "Tan's reasoning-scaffold prototype was demoed in October 2025." No public link. Private demo as track-record substitute.

## Internal inconsistencies

- §17a funds "reference-resource construction work that underpins downstream science." §29: "We do not promise specific clinical outcomes inside 36 months." Either the grant funds science deliverables or it doesn't.
- §29: WorkGraph is "at minimum-viable maturity today." §28: "in daily use across founder labs," with "multi-agent coordination, automatic task spawning, dependency resolution, and lifecycle management." MVP and that feature list aren't the same maturity claim.

## Liverpool overlap

§28: "Liverpool's inaugural Hive Mind grant addresses hybrid coordination for wet-lab autonomous chemistry; we address the parallel pattern for computational and clinical genomics, complementary." Asserted, not argued. WorkGraph is generic infrastructure (Rust, JSONL, agent-agnostic). Two successive grants for "persistent multi-actor task coordination for hybrid human-AI science" need explanation. One sentence on architectural divergence (e.g., Liverpool optimizes for lab-robotics scheduling; WorkGraph for git-native provenance across distributed actors) would help. As written, closer to "didn't we just fund this" than "complementary."

## Three sections I would cut the shortlist over

1. **§29 theory of change.** Three paragraphs of hedge ("honest about both," "we do not promise," "downstream public benefit follows... not from this grant's outputs alone"). Sells nothing. Reads as expecting to underdeliver.
2. **§30 risks.** First risk listed is "reviewers may want a specific scientific deliverable rather than infrastructure." Risk sections disclose project risks, not reviewer mood. Defensive and self-incriminating at once.
3. **§46 milestone 4.** "Longitudinal-deployment results published. Open governance in place. WorkGraph adopted by 50+ labs with documented impact. Computation graph publication recognized as practice in at least some venues." Four vague claims, zero specifics. v2 named "PHR atlas with named diagnostic candidates." Falsifiability deficit.

## Where evidence would convince me

- 1-2 named pilot labs with letters of interest.
- One named first-year preprint or software release the grant produces.
- One named clinical genomics partner, not "initial conversations."
- A named editor for "venues recognizing computation graph publication."
- A public, browsable WorkGraph trace from Garrison's daily research.
- One drafted BioBench challenge.
- One concrete differentiator from Liverpool beyond "different domain."

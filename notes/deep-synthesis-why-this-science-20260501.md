# Deep synthesis: why this science, why this team, why now

**2026-05-01. For Erik, pre-submission.** Approved sharpening folds back via `sync-application-to-synthesis`.

---

## A. Mission as spine

Poietic PBC's filed public benefit purpose, verbatim, is "to make human and machine collaboration legible and responsive to its participants." That is not corporate filler. Hybrid human-AI work is already producing results whose path through human judgment, agent inference, retries, and abandoned branches is opaque to everyone involved, including the participants themselves. When the process is illegible, neither humans nor agents can correct, replicate, or trust the result. Making such work legible is a real public benefit because the counterfactual is irreproducible work compounding at industrial scale. The claim has to be testable, not decorative, which means demonstrating it on something where outputs have truth-value rather than aesthetic preference.

## B. Why science is the proving ground

Scientific research is the right proving ground because scientific reasoning has external validators. Literature, replication, peer review, and downstream analyses adjudicate whether a chain of reasoning was sound. If the trace produced by hybrid human-AI work is illegible, the underlying work is exposed: incoherent rationales fail review even when a conclusion happens to be right. Code passes tests while being narratively incoherent; an essay can be persuasive without being true. Science is harder. Both the conclusion and the reasoning that produced it have to survive third-party scrutiny against an external world. That is exactly the bar legibility infrastructure must clear, and it is what makes the infrastructure claim falsifiable rather than rhetorical.

## C. Why pangenomics specifically

Pangenomics is the right scientific domain for this team. Erik created vg (Nature Methods 2024, foundational pangenomics toolkit, ~72,000 citations) and led PGGB, which the Human Pangenome Reference Consortium uses. He is not adjacent to the field; he built core tools the field uses. There are open biological questions the dominant single-reference paradigm cannot answer: structural variation, repetitive architecture, and population-divergent regions are systematically under-resolved by short-read alignment to one genome. Pangenome graphs make these regions tractable, and the open-source toolchain (vg, PGGB, seqwish, smoothxg, odgi) is mature enough to use today. That maturity matters structurally: even if the legibility demonstration falls short, the pangenomics work survives as standalone scientific output. Luca's accessibility track record (CRISPResso2, CRISPRme) and Vaughn's reasoning-scaffold framework round out the team without overclaiming domain depth either of them already has.

## D. Why PHRs in particular

Pseudo-homologous regions (PHRs) are the right specific question for two reasons flowing from one underlying biology. First, Garrison et al. Nature 2023 established the concept: regions that look homologous by standard methods but are not, whose accurate resolution requires graph-based representation across many genomes. Second, PHRs sit precisely where standard short-read clinical sequencing fails. Repetitive, structurally complex, and population-divergent intervals are exactly the regions where causal variants for undiagnosed rare disease patients hide.

The same biological feature that makes PHRs evolutionarily interesting (patterns of structural change across the vertebrate tree of life) also makes them clinically interesting (variants invisible to current diagnostic pipelines). The science is not bifurcated; one underlying phenomenon yields both relevances.

The deliverable is honest about scope. "PHRs across all species" is not literally what gets shipped in 36 months. The deliverable is a methodology and an atlas growing from a defined starting region, with a defined undiagnosed rare disease cohort as the translational anchor. Each phase produces standalone value, so partial completion remains useful. The atlas is a beginning, not a closure.

## E. What this commits to, what it doesn't

What this proposal does not promise: a clinical pipeline, a cure for any rare disease, validated therapeutics, or that CRISPRme and DNA-Diffusion are funded scope (they are track record; DNA-Diffusion is disclosed as a commercial conflict). It does not promise the full vertebrate PHR catalog in 36 months. What it does promise: an open PHR atlas growing from a defined starting region, an open methodology demonstration with a publicly browsable computation graph, an open benchmark for agentic science (BioBench), and a peer-reviewed organizational design framework from Vaughn's track. Naming what is out of scope is itself a legibility commitment; a proposal that makes its boundaries inspectable is consistent with the public benefit purpose.

## F. Honest read on the v2 application

The v2 application largely lands this synthesis but does not state the legibility-as-mission spine explicitly. Three specific sharpenings:

- **§17a:** open with the legibility public benefit verbatim, then introduce PHR work as the proving ground rather than a co-equal element.
- **§26:** add one sentence framing the team's combination as uniquely able to test legibility infrastructure against external scientific validators, not just deliver pangenomics.
- **§29:** state in the scope risk that "PHRs across all species" is not the 36-month deliverable; the atlas grows from a defined starting region.

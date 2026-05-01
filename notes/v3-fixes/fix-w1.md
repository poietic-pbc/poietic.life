---
fix_id: fix-w1
target_sections:
  - 17a (cap 75)
  - 17b (cap 75)
  - 17c (cap 75)
  - 17d (cap 75)
  - 19a (cap 75)
  - 19b (cap 75)
  - 19c (cap 75)
  - 43 (Milestone 1, cap ~100)
  - 44 (Milestone 2, cap ~100)
  - 45 (Milestone 3, cap ~100)
  - 46 (Milestone 4, cap ~100)
  - extended-outline:research-arcs (200-300w; new subsection)
status: ready-for-assembler
source_commit: 70c8e7f
supersedes:
  - fix-h2 (§17a "in production today" tone fix; this fix subsumes it)
  - fix-h5 (§43 month-18 named deliverable; this fix subsumes it)
  - fix-h6 (§19c BioBench soften; this fix subsumes it)
  - fix-h1 (§29 adoption-numbers; this fix carries the same numbers into §19a : assembler should still apply fix-h1 to §29 separately)
---

# fix-w1 : science-deliverable substrate framing (W1, W4, W7)

## Criticism (verbatim from `notes/v3-review-synthesis-20260501.md` §2)

> **No specific science deliverable.** Skeptical: v2 named a PHR atlas, v3 dropped it without replacement. Domain expert: "what specific reference resource gets built better in 36 months? v3 has no answer." Sympathetic concedes a non-program-officer panelist may ask "what is the science we are buying?" Source of most other objections.
>
> **§43–§46 milestones are vague.** Skeptical: "four vague claims, zero specifics." Domain expert wants a named co-authored deliverable by month 18.
>
> **Authority is borrowed.** Skeptical: vg/CRISPRme prestige invoked across §17a, §17c, §26, §36; grant funds WorkGraph, not vg. Domain expert echoes (PHR is now credential, not deliverable).

Erik's stated solution: WorkGraph as substrate for Garrison lab's ongoing pangenome work (HPRC, PHR, unorthodox recombination, CNV-aware methods development) AND for Luca's high-risk research arc as systematically considered direction. Inputs: discovery notes D1 (pangenome ecosystem), D2 (PHR), D3 (CNV methods), D4 (Luca high-risk arc).

---

## §17a: solution proposed (cap 75)

### Current text (verbatim from v3 at 70c8e7f)

> Poietic PBC builds WorkGraph: open-source infrastructure (MIT, Rust, in production today) where humans and AI agents act as peers in a persistent task graph that is auditable across sessions, operators, and machines. WorkGraph is agent-agnostic, integrating Claude, Gemini, AlphaGenome (via Pinello's Chorus), GPT, and open-weight models. The grant matures the infrastructure and demonstrates it longitudinally inside the founders' active computational and clinical genomics programs, including the reference-resource construction work that underpins downstream science.

### Proposed text

> Poietic PBC builds WorkGraph: open-source infrastructure (MIT, Rust, in daily use across the founders' labs) where humans and AI agents act as peers in a persistent task graph auditable across sessions, operators, and machines. The grant matures the substrate that coordinates Garrison's ongoing pangenome work (PGGB, impg, HPRC Release 3) and Pinello's clinical genomics programs (CRISPRme, IGVF). WorkGraph is agent-agnostic, integrating Claude, Gemini, AlphaGenome (via Pinello's Chorus), GPT, and open-weight models.

### Word count check
- Before: 73 / 75 (+2 headroom)
- After: 71 / 75 (+4 headroom)

---

## §17b: tools, methods, techniques (cap 75)

### Current text

> WorkGraph (Rust, MIT) coordinates multi-actor research via a git-native persistent task DAG with full audit trails and replay. Agent executors include Claude Code, Codex, AlphaGenome and AlphaFold (via Chorus), and open-weight models. The genomics work uses the Garrison ecosystem (vg, seqwish, smoothxg, odgi, PGGB) on Human Pangenome Reference Consortium assemblies, plus Pinello's CRISPResso and CRISPRme stack for clinical analysis. Computation graphs export as interactive HTML so readers can audit how a result was produced.

### Proposed text

> WorkGraph (Rust, MIT) coordinates multi-actor research via a git-native persistent task DAG with full audit trails and replay. Agent executors include Claude Code, Codex, AlphaGenome and AlphaFold (via Chorus), and open-weight models. The genomics work uses the Garrison-led pangenome stack (vg, PGGB, seqwish, smoothxg, odgi, impg, wfmash, COSIGT) on Human Pangenome Reference Consortium assemblies, plus Pinello's CRISPResso and CRISPRme tooling. Computation graphs export as interactive HTML so readers can audit how a result was produced.

### Word count check
- Before: 74 / 75 (+1 headroom)
- After: 75 / 75 (cap)

---

## §17c: evidence the solution would work (cap 75)

### Current text

> WorkGraph is in daily use coordinating Garrison's ongoing pangenomics research and other founder workflows. Underlying pangenome tools (vg, PGGB) are foundational infrastructure for the Human Pangenome Reference Consortium. Pinello's CRISPRme (Nature Genetics 2023) independently identified an off-target in the BCL11A guide later used in Casgevy, informing the FDA review. Tan's organizational research on hybrid teams under uncertainty is published (Columbia University Press; ASQ). WorkGraph is public at github.com/graphwork/workgraph (MIT).

### Proposed text

> WorkGraph is in daily use coordinating Garrison's pangenome research, including the pseudo-homologous-region program (Guarracino, Garrison et al., Nature 2023). The vg, PGGB, and impg toolkit is foundational to the Human Pangenome Reference Consortium (Garrison et al., Nature Methods 2024). Pinello's CRISPRme (Nature Genetics 2023) independently identified an off-target in the BCL11A guide later used in Casgevy, informing FDA review. Tan's organizational research is published (Columbia University Press; ASQ). github.com/graphwork/workgraph (MIT).

### Word count check
- Before: 69 / 75 (+6 headroom)
- After: 70 / 75 (+5 headroom)

Note: ties authority to *named ongoing research program* (PHR, HPRC R3) rather than leaving vg/PGGB as standalone credentials.

---

## §17d: lasting impact (cap 75)

### Current text

> Three durable contributions. First, WorkGraph as open public infrastructure for reliable hybrid human-AI scientific work, with adoption pathways for other labs. Second, longitudinal case studies (Tan) documenting how hybrid scientific organizations actually function, generalizable beyond genomics. Third, BioBench, an open benchmark for agentic science with verifiable biological challenges. Each output compounds: WorkGraph supports reproducible AI-assisted research across fields; the case studies inform organizational design; BioBench creates a community standard for evaluating agentic systems.

### Proposed text

> Three durable contributions. First, WorkGraph as open infrastructure for hybrid human-AI scientific work, with adoption pathways for other labs. Second, longitudinal case studies (Tan) of how hybrid scientific organizations actually function, generalizable beyond genomics. Third, BioBench, an open benchmark for agentic biology. Auditable coordination also lowers the cost of systematic high-risk method exploration in genomics, including generative methods where independent validation is feasible, novel CRISPR strategies, and multi-omics integration.

### Word count check
- Before: 73 / 75 (+2 headroom)
- After: 69 / 75 (+6 headroom)

Note: replaces the "each output compounds…" softness (skeptical-flagged) with the D4 high-risk-arc condensed sentence (per D4 explicit instruction: "slot a single condensed sentence into §17d, replacing the softest existing clause").

---

## §19a: specific metrics (cap 75)

### Current text

> Adoption (the falsifiable external metric): independent labs running WorkGraph for their own work, measured by service-daemon telemetry and published computation graphs. Output: number of preprints, software releases, and reference-resource updates produced through audited workflows in the founders' labs. Methodology: BioBench participation (systems evaluated, challenges submitted) and peer-reviewed publication of Tan's organizational design framework. Community: GitHub stars, forks, contributors, and downstream integrations of WorkGraph-coordinated artifacts.

### Proposed text

> Adoption (the falsifiable external metric, target 10+ labs by month 18, 50+ by month 36): independent labs running WorkGraph for their own work, measured by service-daemon telemetry and published computation graphs. Output: named software releases (impg 1.0, PGGB v1.0, vg-CNV) and HPRC Release 3 contributions delivered through audited workflows in the founders' labs. Methodology: BioBench participation, peer-reviewed publication of Tan's organizational design framework. Community: GitHub stars, forks, contributors, downstream integrations.

### Word count check
- Before: 64 / 75 (+11 headroom)
- After: 70 / 75 (+5 headroom)

Note: numbers are consistent with fix-h1 (§29) and §46 (50+ labs). Output line is now concrete : named substrate deliverables instead of generic "preprints, software releases, reference-resource updates."

---

## §19b: failure signals (cap 75)

### Current text

> Failure looks like: no labs outside the founders adopt WorkGraph after onboarding ends; published computation graphs that other researchers cannot interpret or reuse; the founders themselves quietly reverting to ad-hoc tools for their genomics work; BioBench attracting no external participants or community-submitted challenges; Tan's organizational framework receiving no uptake from other research groups; integrations with Gemini, Chorus, Claude, and open-weight models proving too brittle for sustained real use.

### Proposed text

> Failure looks like: no labs outside the founders adopt WorkGraph after onboarding ends; the founders themselves quietly reverting to ad-hoc tools for pangenome and clinical work; named substrate deliverables (PGGB, impg, vg-CNV, HPRC R3 builds) shipping without WorkGraph traces because the tooling got in the way; BioBench attracting no external participants; Tan's framework receiving no uptake; integrations with Gemini, Chorus, Claude, and open-weight models proving too brittle for sustained real use.

### Word count check
- Before: 68 / 75 (+7 headroom)
- After: 71 / 75 (+4 headroom)

Note: keeps the strongest failure signal v3 already had (founders reverting to ad-hoc tools) and adds the substrate-specific failure mode that pairs with the §19a deliverables.

---

## §19c: changes from baseline (cap 75)

### Current text

> Today, AI-assisted research produces outputs without auditable processes; reference-resource construction lacks systematic provenance; clinical genomics analyses cannot easily be reconstructed by independent reviewers. By project end: computation graph publication as routine practice for at least some genomics venues; a community of independent labs using WorkGraph for sustained hybrid research; ethnographic case studies grounding the organizational design framework; and BioBench established as the open standard for evaluating agentic biology systems.

### Proposed text

> Today, AI-assisted reference-resource construction lacks systematic provenance; pangenome graph builds, CNV-aware methods, and clinical genomics analyses cannot easily be reconstructed by independent reviewers. By project end: computation graph publication as routine practice for at least some genomics venues; HPRC Release 3 builds and named pangenome methods deliverables (impg 1.0, vg-CNV, PGGB v1.0) shipped with end-to-end audit traces; an independent-lab community sustaining WorkGraph; BioBench actively used as a public benchmark by 3+ external groups.

### Word count check
- Before: 69 / 75 (+6 headroom)
- After: 73 / 75 (+2 headroom)

Note: subsumes fix-h6 (BioBench soften) and adds named end-state deliverables tied to D1/D3.

---

## §43: Milestone 1 (Months 1–6, cap ~100)

### Current text

> 43. Milestone 1
> Timeframe: Months 1–6
>
> Activities: Begin longitudinal deployment of WorkGraph across the founders' active genomics programs (Garrison's pangenomics and HPRC work, Pinello's clinical genomics analysis), with auditable computation graphs as the primary output substrate. Develop the interactive web visualization for computation graphs. Begin recruiting pilot labs for WorkGraph adoption. Establish formal partnership with at least one external research program for adopter case-study collaboration.
>
> Outcomes: Initial longitudinal-deployment computation graphs published openly. Methodology paper drafted as preprint. Interactive graph visualization functional. At least 10 pilot labs committed.

### Proposed text

> 43. Milestone 1
> Timeframe: Months 1–6
>
> Activities: Coordinate Garrison's contribution to the Human Pangenome Reference Consortium Release 3 build (350+ samples, 700+ haplotypes via PGGB) using WorkGraph for build orchestration, parameter sweeps, and review. Begin impg scaling work toward 1.0 (sub-second region queries across 700+ haplotypes). Develop the interactive web visualization for computation graphs. Begin recruiting pilot labs.
>
> Outcomes: HPRC Release 3 PGGB build with WorkGraph-traced provenance, co-authored across the pangenome group. impg 1.0 release (github.com/pangenome/impg) co-authored by Garrison, Guarracino, Kille. Interactive graph visualization functional. 10+ pilot labs committed.

### Word count check
- Before (Activities + Outcomes, excluding heading/timeframe): ~80 / 100 (+20 headroom)
- After: 82 / 100 (+18 headroom)

Note: subsumes fix-h5 (impg 1.0 named deliverable). Source: D1 §"Recommended named deliverables for v3.1," items 1 + 2.

---

## §44: Milestone 2 (Months 7–18, cap ~100)

### Current text

> 44. Milestone 2
> Timeframe: Months 7–18
>
> Activities: Continue longitudinal deployment with broader workflow coverage; harden WorkGraph for outside-lab adoption. Deploy WorkGraph in 10+ pilot labs with hands-on onboarding. Build BioBench v1 with 5+ community-contributed challenges and baseline evaluations from at least 3 agentic systems. Multi-user collaboration features (shared graphs, permissions, federated coordination across institutions). Tan begins ethnographic case studies of pilot lab adoption.
>
> Outcomes: First longitudinal-deployment methodology paper accepted. WorkGraph actively used by 15+ research groups. BioBench v1 publicly available. Multi-user features functional. First case study working paper from Tan.

### Proposed text

> 44. Milestone 2
> Timeframe: Months 7–18
>
> Activities: Continue longitudinal deployment with broader workflow coverage. Co-author the COSIGT population-scalable low-coverage genotyping paper (Bolognini, Guarracino, Garrison) through to peer-reviewed publication. Co-author the pangenome graph augmentation paper (Guarracino, Garrison) through to peer-reviewed publication. Deploy WorkGraph in 10+ pilot labs. Build BioBench v1 with 5+ challenges and baselines from 3+ agentic systems. Multi-user collaboration features. First MemPanG cohort. Tan begins ethnographic case studies.
>
> Outcomes: COSIGT and graph-augmentation papers accepted. WorkGraph used by 15+ groups. BioBench v1 public. Multi-user features functional. First Tan working paper.

### Word count check
- Before: ~88 / 100 (+12 headroom)
- After: 84 / 100 (+16 headroom)

Note: replaces vague "first methodology paper accepted" with two named co-authored peer-reviewed papers (D1 §"Recommended named deliverables," items 3 + 5; D3 §"Active named methods-development projects"). MemPanG from D3 §"Named v3.1 deliverables" item 4.

---

## §45: Milestone 3 (Months 19–30, cap ~100)

### Current text

> 45. Milestone 3
> Timeframe: Months 19–30
>
> Activities: Expand longitudinal-deployment coverage and adopter-lab integration. Run BioBench v2 with expanded challenges. Build out the public computation graph repository. Tan publishes the organizational design framework.
>
> Outcomes: BioBench evaluating 5+ systems on 10+ challenges. Methodology framework accepted at peer-reviewed venue (target: Administrative Science Quarterly, Research Policy, or similar). Computation graph repository operational with 50+ published graphs from adopter labs.

### Proposed text

> 45. Milestone 3
> Timeframe: Months 19–30
>
> Activities: Integrate adaptive tracepoint compression (Kaushan, Marco-Sola, Garrison, Prins, Guarracino) into the production PGGB / HPRCv2 stack at HPRC Release 3 scale. Co-author the pangenome variant calling best-practice paper across the wfmash, vg, PGGB, PanVariants, and COSIGT teams. Run the second MemPanG cohort. Run BioBench v2. Build out the public computation graph repository. Tan publishes the organizational design framework.
>
> Outcomes: PGGB integrated with adaptive tracepoints in production. Cross-team variant-calling best-practice paper accepted. BioBench evaluating 5+ systems on 10+ challenges. Methodology framework accepted at peer-reviewed venue (target Administrative Science Quarterly or Research Policy). Computation graph repository operational with 50+ published graphs.

### Word count check
- Before: ~63 / 100 (+37 headroom)
- After: 97 / 100 (+3 headroom)

Note: D1 §"Recommended named deliverables" item 4 (adaptive tracepoints integration) and D3 §"Named v3.1 deliverables" item 5 (cross-team best-practice paper).

---

## §46: Milestone 4 (Months 31–36, cap ~100)

### Current text

> 46. Milestone 4
> Timeframe: Months 31–36
>
> Activities: Publish final longitudinal-deployment outcomes and adopter-lab case-study series. Open governance committee established for WorkGraph long-term stewardship. Engage with journals and funders on standards for computation graph publication.
>
> Outcomes: Longitudinal-deployment results published. Open governance in place. WorkGraph adopted by 50+ labs with documented impact. Computation graph publication recognized as practice in at least some venues.

### Proposed text

> 46. Milestone 4
> Timeframe: Months 31–36
>
> Activities: Ship vg-CNV (paralog-aware CNV genotyper integrated with vg giraffe, validated on Genome in a Bottle and HPRC samples). Ship PGGB v1.0 with CNV-aware paralog-preserving graph construction. Run the third MemPanG cohort. Publish final longitudinal-deployment outcomes and adopter-lab case-study series. Open governance committee established for WorkGraph long-term stewardship. Engage with journals and funders on standards for computation graph publication.
>
> Outcomes: vg-CNV and PGGB v1.0 released with reproducibility benchmarks on HPRC v2. WorkGraph adopted by 50+ labs with documented impact. Open governance in place. Computation graph publication recognized as practice in at least some venues.

### Word count check
- Before: ~58 / 100 (+42 headroom)
- After: 94 / 100 (+6 headroom)

Note: D3 §"Named v3.1 deliverables" items 1 + 2 (PGGB v1.0, vg-CNV) at month-36 endpoint.

---

## Extended outline: new subsection "Research arcs systematically considered" (200–300 words)

### Where this goes
Per D4 explicit recommendation: **NOT the form** (every form section is at-cap or used). Insert in `workgraph_extended_outline_v2.md` as a new subsection under approach, sitting adjacent to the longitudinal-deployment description and before the milestones. The §17d single-sentence form fix above carries the condensed claim into the form itself.

### Proposed paragraph (~272 words)

> Beyond reference-resource construction and clinical genomics, WorkGraph is designed to host high-risk, high-reward research as a class. Auditable coordination is what makes failure-tolerant research practical at lab scale: when every dead end, parameter sweep, and model interrogation lives in a persistent computation graph, the marginal cost of trying a method that does not work falls, and the institutional memory for what has already been tried rises. Pinello's track record (CRISPResso2 as the field standard for CRISPR editing analysis; CRISPRme's independent off-target discovery in the BCL11A guide later used in Casgevy; Chorus orchestrating genomic AI including AlphaGenome; IGVF Consortium characterization-center leadership) demonstrates the methodological breadth this enables: variant-aware analysis, agentic genomic AI orchestration, multi-omics integration, and novel CRISPR strategy exploration. We treat these as research directions we want to systematically consider with hybrid human-AI teams, not as 36-month deliverables. Concretely, we expect WorkGraph deployments inside the founders' active programs to surface candidate workflows in classes including generative-method exploration applied to genomics targets where independent validation is feasible, novel CRISPR design and off-target analysis strategies, multi-omics integration for clinical interpretation, and reference-graph construction methods that admit explicit error budgets. Specific products, candidates, and discoveries are intentionally not promised here, both because they depend on what the science finds and because adjacent areas (notably generative DNA design) sit inside Pinello-disclosed commercial conflicts and remain outside funded scope. What the grant funds is the coordination substrate that makes systematic exploration of these arcs auditable, reproducible, and durable across sessions, operators, and labs.

### Word count check
- 272 words / 200–300 cap (within band)

### Constraint verification
- No DNA-Diffusion in funded scope (explicitly excluded as commercial-COI area).
- No specific drug, molecule, target, or therapeutic.
- No "drug discovery," "novel drug," "competition," or "race" framing.
- No KRAS / MRTX1133 / Boltz / RFdiffusion / DiffDock terms.
- No claim WorkGraph "will produce" or "will discover" anything in 36 months.
- No first-mover claims on AlphaFold/AlphaGenome (Chorus cited as Pinello's existing prior work).
- "Research direction systematically considered" framing per D4.

---

## Rationale (why this fix lands the convergent W1/W4/W7 criticism)

The skeptical, sympathetic, and domain-expert reviewers all converged on the same gap: v3 retreated from v2's PHR atlas without naming any concrete reference resource, software release, or co-authored paper that the grant produces. As a result, the team's verifiable authority (vg, PGGB, CRISPRme, ASQ) reads as borrowed rather than tied to a 36-month deliverable, and §43–§46 read as four vague claims.

This fix replaces the "longitudinal deployment plus case studies" abstraction with a graph of named, in-flight deliverables drawn from D1 (HPRC R3 build, impg 1.0, adaptive tracepoints integration), D2 (PHR research arc cited in §17c as the named ongoing program WorkGraph substrates), and D3 (COSIGT, graph-augmentation paper, vg-CNV, PGGB v1.0, MemPanG, cross-team variant-calling best-practice paper). Each deliverable has a co-author list, a venue or release target, and a public artifact (GitHub URL, bioRxiv preprint) the panel can verify pre-submission. The substrate framing is honest: the grant does not fund vg, PGGB, or CRISPRme themselves (those have their own funding); it funds the coordination layer that makes their continued development across labs, agents, and operators reproducible. D4's high-risk-arc paragraph completes the picture by positioning Pinello's methodological breadth as a research direction WorkGraph systematically supports, without committing to specific 36-month outputs in commercially conflicted areas (DNA-Diffusion).

After this fix, a reviewer asking "what specific scientific output gets shipped in 36 months?" can point to: HPRC R3 graphs (m6), impg 1.0 (m12), COSIGT + graph-augmentation papers (m18), adaptive-tracepoints + variant-calling best-practice paper (m30), vg-CNV + PGGB v1.0 (m36), plus three MemPanG cohorts and Tan's framework. Authority is no longer borrowed because the credentials cited (Nature 2024 PGGB, Nature 2023 PHR) are continuations of named deliverables in the milestone block.


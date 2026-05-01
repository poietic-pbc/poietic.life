# Discovery D1: pangenome ecosystem + Garrison lab roadmap

Date: 2026-05-01
Purpose: replace v3 §17/§19/§28/§43–§46 vague "longitudinal deployment" language with named, verifiable deliverables tied to ongoing Garrison lab and HPRC work. Addresses panel weakness W1 (no specific science deliverable) and W7 (authority not tied to deliverable).

All URLs were checked on 2026-05-01. Where a source could not be retrieved (bioRxiv 403s, wiki gated), it is noted.

## Active named software with ongoing development

**PGGB (Pangenome Graph Builder)**
- Repo: https://github.com/pangenome/pggb
- Status: production. v0.7.4 (Apr 2025), 1,218 commits, 493 stars. Used by HPRC for both releases.
- Function: end-to-end pipeline that builds pangenome graphs from haplotype assemblies (wfmash → seqwish → smoothxg → odgi).
- Garrison lab leads. Garrison and Guarracino are lead authors of the Nature Methods 2024 paper.
- v3.1 deliverable: yes (continued maintenance, integration as the HPRC-R3 build pipeline).

**odgi (Optimized Dynamic Graph Implementation)**
- Repo: https://github.com/pangenome/odgi
- Status: production, very active (most recent push 2026-05-01), 243 stars, 58 open issues.
- Function: graph manipulation, statistics, sorting, layout, GPU layout (Li et al., SC24 2024).
- Garrison lab leads.
- v3.1 deliverable: yes (named tool for any pangenome-graph milestone).

**seqwish**
- Repo: https://github.com/pangenome/seqwish
- Status: production, recent activity (push 2026-04-11).
- Function: alignment-to-graph inducer; consumes pairwise alignments and emits a variation graph in GFA.
- Garrison lab leads.

**smoothxg**
- Repo: https://github.com/pangenome/smoothxg
- Status: maintained component of PGGB.
- Function: graph linearization and simplification via blocked POA.
- Garrison lab leads.

**impg (implicit pangenome graph)**
- Repo: https://github.com/pangenome/impg
- Status: active, v0.4.0 (Jan 2026), 1,060 commits, 101 stars. Bioconda + Docker distribution.
- Function: treats all-vs-all pairwise alignments as an implicit graph, enabling fast region queries across hundreds of genomes without materializing a full graph.
- Maintainers: Guarracino, Bryce Kille, Garrison.
- Garrison lab leads.
- v3.1 deliverable: yes (impg 1.0 / scaling milestone is a defensible named target).

**HPRCv2 graphs and alignment products**
- Repo: https://github.com/pangenome/HPRCv2
- Status: active (push 2026-04-23). 25,221 pairwise alignments, 465 haplotypes vs CHM13 and vs GRCh38, PGGB-built explicit graphs in GFA, variant calls.
- Garrison lab co-leads with HPRC pangenomics working group.
- v3.1 deliverable: yes (HPRC Release 3 graphs, see roadmap below).

**vg toolkit + vg Giraffe**
- Repo: https://github.com/vgteam/vg (1.3k stars, push 2026-05-01).
- Status: production. Recent: "Rapid, accurate long- and short-read mapping to large pangenome graphs with vg Giraffe" (bioRxiv Sep 2025, https://www.biorxiv.org/content/10.1101/2025.09.29.678807v1; PMC12633584, in print).
- Pangenome group, Garrison adjacent. UCSC-led (Chang, Novak, Eizenga, Sirén, Paten); Garrison is contributing author.
- v3.1 deliverable: cite as ecosystem partner, not as a Garrison-led milestone.

**Supporting tools.** wfmash, gfalook, panacus (Bioinformatics 2024), and nf-core/pangenome (Bioinformatics 2024) live in the same org. Pangenome group; Garrison contributes.

## Papers in progress / recent (Garrison-named)

| Year | Title | Venue | Garrison role | Link |
|------|-------|-------|---------------|------|
| 2026 | Adaptive Tracepoints for Pangenome Alignment Compression | bioRxiv | Middle (with Guarracino, Prins) | https://www.biorxiv.org/content/10.64898/2026.02.16.706236v1 |
| 2026 | Privacy-Preserving Pangenome Graphs | bioRxiv | Co-author | https://www.biorxiv.org/content/10.64898/2026.02.16.706152v1 |
| 2026 | Population-scalable genotyping from low-coverage sequencing data using pangenome graphs | bioRxiv | Senior (Bolognini, Guarracino lead) | not retrieved (bioRxiv 403) |
| 2026 | High-quality mouse reference genomes (murine pangenome) | Cell Genomics | Co-author | in print |
| 2025 | Pangenome graph augmentation from unassembled long reads | bioRxiv (v2) | Senior (Guarracino lead) | https://www.biorxiv.org/content/10.1101/2025.02.07.637057v2 |
| 2025 | Multispecies pangenomes (population size and SVs) | Science | Co-author (Edwards lead) | https://www.science.org/doi/10.1126/science.adw1931 |
| 2025 | Comparative population pangenomes (scrub-jays) | bioRxiv | Co-author (Edwards lead) | https://www.biorxiv.org/content/10.1101/2025.02.11.637762v1 |
| 2025 | Robertsonian chromosomes; ape T2T; acrocentrics | Nature x2 + bioRxiv | Co-author (Guarracino, de Lima, Koren) | published |
| 2025 | Pangenome reconstruction in rats | iScience | Senior (Villani, Guarracino lead) | published |
| 2024 | Building pangenome graphs (PGGB) | Nature Methods | First (with Guarracino) | https://www.nature.com/articles/s41592-024-02430-3 |

## HPRC roadmap items (Garrison-positioned)

Source: https://humanpangenome.org/release-timeline/. The public timeline only extends to Summer 2026; post-2026 plans live in the gated wiki (https://wiki.humanpangenome.org/) and were not retrieved here.

- **Release 3, Summer 2026.** 350+ samples, 700+ haplotypes, "essentially complete telomere-to-telomere assemblies," Mount Sinai cohort plus international partners. PGGB is the consortium's pangenome-graph build pipeline; HPRCv2 repo is the production artifact pattern. Garrison lab is positioned to deliver the R3 graphs and alignment products.
- **Beyond R3 (inferred, not committed):** continued PGGB scaling to 1,000+ haplotypes; impg at consortium scale; HPRCv2-style products for R3; companion graphs for medically complex regions (HLA, KIR, IGH, segmental duplications).

## Pangenome group active research arcs

Beyond software, four scientific arcs are visibly active and Garrison-adjacent:

1. **Multispecies and conservation pangenomics.** Edwards lab (Harvard MCZ) plus Garrison: scrub-jays, multispecies (Science 2025), see also Journal of Heredity advance article on SVs in conservation genomics (https://academic.oup.com/jhered/advance-article/doi/10.1093/jhered/esaf098/8341471).
2. **Hard-region biology of the human genome.** Centromeres, acrocentrics, rDNA, Robertsonian translocations: Guarracino, de Lima, Koren, Potapova. Pangenome graphs as the substrate.
3. **Plant pangenomes.** Rice, potato (Cheng et al., Nature 2025), Arabidopsis (Bao et al.); transposable elements (PanTE).
4. **Pangenome infrastructure scaling.** Adaptive tracepoints (compression), privacy-preserving graphs, low-coverage genotyping, GPU layout, hardware-aware pangenomics (PangenomicsBench, IEEE 2025, with Cornell ECE: Kaplan, Batten, Das).

Visible Garrison-lab and close-collaborator names in 2025–2026 author lists: Andrea Guarracino, Pjotr Prins, JN Schmelzle, SS Darnell, Bryce Kille, D Bolognini, F Villani, P Hebbar, S Marco-Sola, H Kaushan.

## Recommended named deliverables for v3.1

Each is already underway, so v3.1 commits to incremental delivery, not speculation. Timing assumes a grant clock starting ~Jan 2027.

1. **HPRC Release 3 pangenome graphs and HPRCv2-pattern data release for R3.** Garrison lab leads the PGGB build. Months 1–9. (R3 lands Summer 2026 pre-grant; companion graph products are the post-grant deliverable.)
2. **impg 1.0 with HPRC-R3-scale benchmarks.** Currently v0.4.0; 1.0 with sub-second region queries across 700+ haplotypes. Months 1–12. Garrison-led (Guarracino, Kille, Garrison).
3. **Pangenome graph augmentation from unassembled long reads (peer-reviewed publication and reference implementation).** Preprint exists (bioRxiv 2025); peer-reviewed venue plus maintained tool in pangenome org. Months 6–18. Garrison-led.
4. **Adaptive tracepoint compression integrated into PGGB and HPRCv2.** Preprint exists (bioRxiv Feb 2026); integration into the production stack at HPRC-R3 scale. Months 12–24. Garrison co-led.
5. **Population-scalable low-coverage genotyping with pangenome graphs (peer-reviewed publication and pipeline release).** Preprint exists (Bolognini, Guarracino, ..., Garrison 2026). Months 6–18. Garrison contributes.

A v3.1 §43–§46 block can name (1)+(2) at month 12, (3)+(5) at month 18, and (4) plus extension of (1) at month 24. All are in-flight work the panel can verify against bioRxiv, GitHub, and the HPRC release timeline.

## Caveats

- Three primary preprint URLs (bioRxiv full text) returned 403 to the fetcher. Titles, authors, and venues were cross-checked via WebSearch and Google Scholar listings; full-text claims here are summary-level.
- The UTHSC faculty profile page returned a template, not a profile, so current lab roster is reconstructed from coauthorship patterns rather than a published lab page. No private lab page was found.
- HPRC plans beyond Summer 2026 are inferred from current trajectories, not from a published roadmap.

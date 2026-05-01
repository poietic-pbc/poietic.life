---
title: "Discovery D3: CNV-aware aligners and pangenome methods development"
date: 2026-05-01
purpose: "Replace v3 §43-§46 vague 'methodology paper drafted' milestone with named methods-development deliverables. Addresses panel weakness W4."
audience: "v3.1 author"
---

# CNV-aware alignment: state of the field

Standard short-read aligners (BWA, minimap2) and even reference-based variant callers handle copy-number-variable (CNV) regions poorly because they collapse paralogs onto a single reference copy and discard reads that map ambiguously. Pangenome graph mappers (vg map, vg giraffe) recover much of this signal by representing alternative haplotypes explicitly, but graph-based pangenomes themselves can merge similar paralogs into shared nodes, obscuring paralog-specific variants ([Nature Genetics 2025, ctyper](https://www.nature.com/articles/s41588-025-02346-4)). The active research front is therefore CNV-aware alignment and genotyping that preserves paralog identity: methods that combine pangenome graphs, k-mer evidence, and explicit copy-number models. Recent benchmarks (PanVariants, April 2026) show 45 to 73 percent reductions in SNV/indel/SV errors versus BWA+GATK, which is the quantitative gap WorkGraph-coordinated methods development is positioned to close further.

# Active named methods-development projects

**vg / vg giraffe (long + short reads).** Mapper for pangenome graphs in the vg toolkit. The Sept 2025 preprint extends Giraffe to long reads at speeds comparable to linear mappers and an order of magnitude faster than GraphAligner. Garrison contributes (UCSC/Paten lead). [bioRxiv 2025.09.29.678807](https://www.biorxiv.org/content/10.1101/2025.09.29.678807v1.full).

**wfmash.** Pangenome-scale all-to-all aligner using MashMap 3.5 minmers + WFA. v0.24.1 released within the last week (April 2026). Garrison and Guarracino co-lead. [github.com/waveygang/wfmash](https://github.com/waveygang/wfmash).

**impg (implicit pangenome graph).** Treats all-vs-all pairwise alignments as an implicit graph, projecting target ranges through the alignment network to extract homologous loci without building a full graph. Garrison, Guarracino, Kille co-lead. Active April 2026. [github.com/pangenome/impg](https://github.com/pangenome/impg).

**COSIGT.** COsine SImilarity-based GenoTyper for population-scale low-coverage (1 to 2x) structural genotyping from pangenome graphs. Bolognini, Guarracino, Garrison. [bioRxiv 2026.02.05.704023](https://www.biorxiv.org/content/10.64898/2026.02.05.704023v1).

**Adaptive Tracepoints for Pangenome Alignment Compression.** Complexity-aware alignment encoding for pangenome-scale alignments. Kaushan, Marco-Sola, Garrison, Prins, Guarracino. [bioRxiv 2026.02.16.706236](https://www.biorxiv.org/content/10.64898/2026.02.16.706236v1).

**PGGB / seqwish / smoothxg / odgi.** The PanGenome Graph Builder pipeline. odgi updated May 1, 2026; seqwish, smoothxg active. Garrison leads PGGB and seqwish; smoothxg and odgi are co-led with Guarracino and Heumos. [github.com/pangenome/pggb](https://github.com/pangenome/pggb).

**sweepga, gfalook, gfasort.** New Rust-based pangenome utilities (alignment filtering, GFA visualization, graph sorting). All updated April 2026 under github.com/pangenome.

**HPRCv2 release tooling.** Pangenome alignment, implicit/explicit graph construction, and variant pipelines for the Human Pangenome Reference Consortium release 2. Garrison contributes. [github.com/pangenome/HPRCv2](https://github.com/pangenome).

**ctyper.** Pangenome-based CNV genotyper that recovers paralog-specific copy numbers and variants. Garrison contributes (Chaisson lab leads). [Nature Genetics 2025](https://www.nature.com/articles/s41588-025-02346-4).

**PanVariants.** Best-practice pangenome variant calling pipeline integrating k-mer and mapping methods. Independent group, but operates on PGGB/HPRC graphs. [bioRxiv 2026.04.22.720142](https://www.biorxiv.org/content/10.64898/2026.04.22.720142v1).

# Erik's recent methods work

- **Building pangenome graphs.** Garrison et al., *Nature Methods* 2024 (PMID 39433878). PGGB methods paper, Garrison leads.
- **vg Giraffe long-read extension.** *bioRxiv* Sept 2025. Garrison contributes.
- **Multispecies pangenomes reveal pervasive influence of population size on structural variation.** *Science* 2025. Garrison co-author.
- **Comparative population pangenomes reveal unexpected complexity and fitness effects of structural variants.** *bioRxiv* Feb 2025. Garrison co-author.
- **COSIGT.** *bioRxiv* Feb 2026. Garrison co-author.
- **Adaptive Tracepoints.** *bioRxiv* Feb 2026. Garrison co-author.

# Named v3.1 deliverables (suitable for §43-§46)

1. **PGGB v1.0 release with CNV-aware paralog-preserving graph construction (months 1 to 12).** Integrate impg-based projection, adaptive tracepoint compression, and ctyper-style paralog tracking into the standard PGGB pipeline. Deliverable: tagged release, methods preprint, reproducibility benchmark on HPRC v2.

2. **vg-CNV: paralog-aware CNV genotyper integrated with vg giraffe (months 6 to 18).** Bring ctyper-class CNV calling into the vg toolkit so it runs end-to-end with giraffe. Deliverable: vg subcommand, validation on Genome in a Bottle and HPRC samples, peer-reviewed methods paper.

3. **PHR atlas across 5+ vertebrate pangenomes built on the new tooling (months 12 to 30).** Pseudo-homologous region atlas computed via wfmash + impg + odgi, published as queryable resource. Deliverable: public atlas, paper, browser.

4. **MemPanG workshop series (annual, months 6, 18, 30).** Memphis Pangenomics workshop ([github.com/pangenome/MemPanG26](https://github.com/pangenome)) as recurring training and standards forum. Deliverable: 3 cohorts, published curriculum, community-authored best-practice notes.

5. **Pangenome variant calling best-practice paper, co-authored across the wfmash / vg / PGGB / PanVariants / COSIGT teams (months 18 to 24).** Multi-tool benchmark and recommended pipeline for clinical pangenome variant calling, anchored on the rare-disease cohort. Deliverable: open benchmark, peer-reviewed paper, public pipeline.

# WorkGraph's substrate role for methods development

These deliverables are not the work of one lab. PGGB, wfmash, impg, vg giraffe, ctyper, COSIGT, and PanVariants are developed by overlapping but distinct groups (Garrison at UTHSC, Guarracino at HT Genova, Paten at UCSC, Chaisson at USC, Bolognini, Heumos in Tübingen, Marco-Sola, plus the PanVariants authors). They share file formats (GFA, PAF), share benchmark cohorts (HPRC, GIAB), share users (HPRC consortium, IGVF, clinical labs), and increasingly share regression failures: a wfmash change breaks an impg downstream test, a vg release shifts giraffe behavior on the HPRC graph, a ctyper update needs odgi to expose new metadata.

WorkGraph is the substrate because methods development across this network has three properties that current tooling does not handle. First, contributions are persistent and cross-session: a benchmark scaffold or graph-construction recipe authored once should be reusable across releases, agents, and operators, which a Claude Code transcript cannot offer. Second, tasks span humans and agents as peers: an agent can run a giraffe regression suite while Garrison reviews a PGGB graph diff, both writing into the same DAG and both auditable. Third, the artifact itself, the task graph, doubles as the methods-paper supplement: every alignment parameter, every accepted or rejected candidate region, every reviewer note is preserved as a node, which is the form journals and HPRC are now asking for. The §43-§46 milestones above are concrete because they were chosen to exercise exactly these three properties; success in months 1 to 12 is a release plus the WorkGraph trace that produced it.

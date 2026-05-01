# v3 sections 29, 30, 33, 34a, 34b, 35, 36 (theory of change, risks, team evolution, sustainability, learnings, public presence)

Drafter: agent-65 (v3-fanout-e-29). Spine: open-source infrastructure
for reliable, careful, auditable hybrid human-AI work in computational
and clinical genomics; longitudinal deployment across the founders'
active programs is the demonstration; lab adoption is the falsifiable
external metric. Word counts shown after each section (caps: §29 = 200,
§30 = 100, §33 = 150, §34a/b = 50 each, §35/§36 = 100). No em-dashes;
founder order Erik / Luca / Vaughn. COI on Luca's generative DNA
commercial interests disclosed in §30. The "reviewers want a specific
scientific deliverable rather than infrastructure" risk is explicit in
§30, with the agreed mitigation: every longitudinal case study produces
a real research output and lab adoption is the falsifiable metric.

---

### §29 Theory of change (200 words)

The chain by which this grant produces public benefit has links we control upstream and links we do not control downstream. We are honest about both.

Upstream: WorkGraph is at minimum-viable maturity today, used daily by the founders. The grant funds hardening it for outside labs and a longitudinal deployment across the founders' active genomics programs (Garrison's pangenomics and HPRC work, Pinello's clinical genomics), producing real research outputs (preprints, software releases, datasets) coordinated through auditable computation graphs. Lab adoption is the falsifiable external metric.

Middle: when labs adopt and stay, hybrid human-AI genomics work becomes more reliable. Errors are caught earlier, provenance is traceable, results reproduce across operators and machines. This matters most in reference-resource construction, where errors and biases propagate to thousands of downstream studies, and in clinical genomics, where misinterpretation has direct patient consequences.

Downstream: better science contributes to clinical and translational benefit. We do not promise specific clinical outcomes inside 36 months. The chain is real but indirect, and the PBC mission ("make human and machine collaboration legible and responsive to its participants") is what we operationalize directly. Downstream public benefit follows from credible reference resources and reproducible clinical analyses, not from this grant's outputs alone.

(199 words)

---

### §30 Risks (100 words)

Five risks. First, reviewers may want a specific scientific deliverable rather than infrastructure. Mitigation: every longitudinal case study produces a real research output (preprint, software release, dataset); lab adoption is the falsifiable external metric. Second, founder distraction from university appointments. Mitigation: structured part-time effort, two full-time research software engineers. Third, single-point-of-failure on Garrison for WorkGraph core. Mitigation: documented architecture, second-engineer hire, contributor pipeline. Fourth, Pinello's generative DNA commercial interests; DNA-Diffusion is track record only, outside funded scope. Fifth, incumbent CLI vendors adding coordination features. Differentiator is structural: persistent git-native multi-actor provenance, MIT, vendor-neutral.

(99 words)

---

### §33 How would the team's structure evolve? (150 words)

Year 1: founding team plus two research software engineers (Rust, systems) for WorkGraph core, computation-graph visualization, and integrations; one AI/biology research scientist supporting BioBench, longitudinal deployment, and pilot lab onboarding. Year 2: community manager for adopters and BioBench events; informal advisory group spanning pangenomics, clinical genomics, computational biology, and open-science governance. Year 3: transition toward a community-supported open-source project with formal governance, including a steering committee with representation from adopter labs so the platform evolves to fit real research needs rather than founder preference. This trajectory mirrors successful open-source scientific infrastructure (Galaxy, Nextflow, vg) and ensures sustainability beyond the founding team. Tan's organizational design framework, published in Year 3, codifies the principles for any group adopting hybrid human-AI scientific coordination, making the methodology transferable rather than bespoke.

(133 words)

---

### §34a Financial sustainability (50 words)

Garrison and Pinello have sustained open-source scientific infrastructure (vg, PGGB, CRISPResso, CRISPRme) for over a decade through diversified funding: NIH R01s, NSF awards, foundation support. Poietic PBC follows this proven model, supplemented by optional commercial services (consulting, enterprise support) for adopters. The MIT-licensed core remains permanently free.

(47 words. v2 text retained verbatim; aligns with v3 spine.)

---

### §34b Technical sustainability (50 words)

WorkGraph's Rust codebase, JSONL storage, and MIT license ensure long-term maintainability. The platform has no proprietary dependencies. Community contributions follow standard open-source practices (GitHub, CI/CD, documentation). BioBench benchmarks, longitudinal computation-graph archives, and contributed reference-resource artifacts are self-sustaining public goods that persist independently of active development.

(46 words. Light edit from v2: "PHR atlas" replaced with "longitudinal computation-graph archives, and contributed reference-resource artifacts" to match v3 spine.)

---

### §35 Key learnings and sharing (100 words)

Three field-wide learnings. First, whether persistent multi-actor coordination measurably improves the reliability and auditability of computational and clinical genomics work, verified through longitudinal case studies in the founders' programs and adopter labs. Second, whether reference-resource construction (pangenomes, variant catalogues) becomes more careful, traceable, and reproducible when authored on top of an auditable hybrid human-AI substrate. Third, what organizational design principles make hybrid teams effective in real research, formalized as a peer-reviewed framework. Sharing through peer-reviewed publications, open-source code, BioBench, public computation-graph archives, conferences, and community workshops.

(87 words)

---

### §36 Public presence (100 words)

WorkGraph is publicly available at github.com/graphwork/workgraph (MIT, 93+ commits). Co-founders have extensive public profiles. Garrison: vg ecosystem (~72,000 citations, Nature Methods 2024), pseudo-homologous regions (Nature 2023), HPRC contributions. Pinello: CRISPResso2 (~18,700 citations, Nature Biotechnology), CRISPRme (Nature Genetics 2023, off-target identified independently in the BCL11A guide before Casgevy FDA approval), Chorus framework, IGVF Consortium center. Tan: *The Uncertainty Mindset* (Columbia University Press 2020), Administrative Science Quarterly 2015, recent Future of Life Foundation fellowship on AI for Human Reasoning. Longitudinal case-study outputs and computation-graph archives will be published openly with interactive reports.

(91 words)

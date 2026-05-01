# v3 sections 16–17 (problem and approach)

Drafter: agent-66 (v3-fanout-a-16). Spine: open-source infrastructure
for reliable, careful, auditable hybrid human-AI work in computational
and clinical genomics; reference-resource construction is the concrete
demonstration anchor. Word counts shown after each subsection (hard
cap 75).

---

### §16a

Scientific work in genomics is high-stakes, error-sensitive, and increasingly hybrid: human researchers, AI agents, and algorithmic pipelines all contribute to a single result. Current tools either treat AI as an ephemeral assistant (Claude Code, Codex, Deep Research are session-scoped) or treat science as a data pipeline (Galaxy, Nextflow, Snakemake have no agentic actors). Neither preserves auditable, persistent coordination across humans and machines. The decisions that produced a result vanish.

(69 words)

---

### §16b

Genomics outputs flow downstream as clinical interpretations, reference resources, and published findings that thousands of labs build on. When the hybrid human-AI process producing them is invisible, errors and biases propagate silently. AI accelerates output while degrading reproducibility. As agent-assisted science scales, the field needs infrastructure that makes the coordination itself a primary, inspectable artifact. Without it, the productivity gains from AI come at the cost of the trust the field depends on.

(73 words)

---

### §16c

Can persistent, multi-actor task graphs make hybrid human-AI scientific work reliable enough for high-stakes genomics, including the construction of reference resources used by thousands of downstream labs? Can the coordination substrate generalize across computational and clinical genomics workflows, and across model providers? Can such infrastructure be deployed inside working research programs, evaluated by lab adoption rather than benchmark scores, and produce reusable patterns for hybrid scientific organizations beyond genomics?

(69 words)

---

### §17a

Poietic PBC builds WorkGraph: open-source infrastructure (MIT, Rust, in production today) where humans and AI agents act as peers in a persistent task graph that is auditable across sessions, operators, and machines. WorkGraph is agent-agnostic, integrating Claude, Gemini, AlphaGenome (via Pinello's Chorus), GPT, and open-weight models. The grant matures the infrastructure and demonstrates it longitudinally inside the founders' active computational and clinical genomics programs, including the reference-resource construction work that underpins downstream science.

(73 words)

---

### §17b

WorkGraph (Rust, MIT) coordinates multi-actor research via a git-native persistent task DAG with full audit trails and replay. Agent executors include Claude Code, Codex, AlphaGenome and AlphaFold (via Chorus), and open-weight models. The genomics work uses the Garrison ecosystem (vg, seqwish, smoothxg, odgi, PGGB) on Human Pangenome Reference Consortium assemblies, plus Pinello's CRISPResso and CRISPRme stack for clinical analysis. Computation graphs export as interactive HTML so readers can audit how a result was produced.

(74 words)

---

### §17c

WorkGraph is in daily use coordinating Garrison's ongoing pangenomics research and other founder workflows. Underlying pangenome tools (vg, PGGB) are foundational infrastructure for the Human Pangenome Reference Consortium. Pinello's CRISPRme (Nature Genetics 2023) independently identified an off-target in the BCL11A guide later used in Casgevy, informing the FDA review. Tan's organizational research on hybrid teams under uncertainty is published (Columbia University Press; ASQ). WorkGraph is public at github.com/graphwork/workgraph (MIT).

(69 words)

---

### §17d

Three durable contributions. First, WorkGraph as open public infrastructure for reliable hybrid human-AI scientific work, with adoption pathways for other labs. Second, longitudinal case studies (Tan) documenting how hybrid scientific organizations actually function, generalizable beyond genomics. Third, BioBench, an open benchmark for agentic science with verifiable biological challenges. Each output compounds: WorkGraph supports reproducible AI-assisted research across fields; the case studies inform organizational design; BioBench creates a community standard for evaluating agentic systems.

(73 words)

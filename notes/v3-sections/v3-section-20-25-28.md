# v3 sections 20, 21, 23, 25, 28 (technical / operational + related work)

Drafter: agent-63 (v3-fanout-c-20-25). Spine: open-source infrastructure
for reliable, careful, auditable hybrid human-AI work in computational
and clinical genomics; reference-resource construction is the concrete
demonstration anchor. Word counts shown after each section (hard cap
100). No em-dashes; founder order Erik / Luca / Vaughn (referenced by
surname). Liverpool framing per CLAUDE.md (complementary slot, not
redundant; no independent web research). Competitor framing honest:
no claims that other systems lack multi-agent or human-in-the-loop;
the differentiator is persistence, structure, open source, and the
graph as deliverable.

---

### §20

WorkGraph is built in Rust with a JSONL-based task graph and Unix-socket service daemon. It coordinates agents from multiple providers: Claude Code, Codex, Gemini, and open-weight models (Qwen, Llama) via local inference. Reference-resource construction uses vg, PGGB, seqwish, smoothxg, and odgi (Garrison ecosystem). Clinical genomics analysis uses CRISPRme-derived variant- and haplotype-aware patterns. AlphaFold and AlphaGenome are available as agent-callable tools through Pinello's Chorus framework. Literature retrieval uses PubMed and bioRxiv APIs. Interactive computation-graph visualization is built with D3.js. Standard cloud compute (AWS, GCP) plus local GPU for open-weight inference.

(89 words)

---

### §21

Existing tools solve fragments. Claude Code and Codex spawn subagents and include human controls, but coordination is session-scoped: state and work logs end with the session. Academic frameworks (SciAgents, Virtual Lab) are paper demonstrations, not maintained infrastructure. Workflow managers (Galaxy, Nextflow, Snakemake) coordinate data pipelines, not iterative agent research. None of these provides what reliable reference-resource construction and careful clinical genomics analysis require: a persistent, git-native, multi-actor task graph where humans and agents are peers, structured as the primary research artifact, surviving sessions, operators, and machines.

(86 words)

---

### §23

WorkGraph coordinates agents; it does not train or fine-tune models, minimizing data-privacy risk. Computation graphs are authored by consenting collaborators and published with permission. Reference-resource construction is high-stakes work: errors and biases propagate to thousands of downstream labs. WorkGraph's auditable graph is the mitigation, not the risk. Clinical genomics workflows handle only de-identified data and route through standard human-subjects protocols at partner programs. Outputs are computational predictions, labeled as such, and require independent validation. We benchmark agent reliability honestly, reporting failures alongside successes. Tan's "do not outsource subjective judgment without explicit reason" rule operationalizes Google's AI Principles.

(98 words)

---

### §25

Three areas. First, integration with Google Cloud and Vertex AI for scalable agent orchestration, allowing WorkGraph to dispatch agents on Google infrastructure alongside other providers. Second, deeper integration with AlphaFold and AlphaGenome as first-class agent-callable tools within WorkGraph, building on Pinello's Chorus precedent; AlphaGenome is particularly relevant to clinical genomics workflows that touch regulatory variants. Third, engineering support for the interactive computation-graph visualization, drawing on Google's data-visualization expertise to make audit trails legible to working scientists, not only computational specialists. Accelerator participation, mentorship, and storage credits for reference-resource artifacts are welcome.

(91 words)

---

### §28

WorkGraph is functional and publicly available (github.com/graphwork/workgraph; MIT), supporting multi-agent coordination, automatic task spawning, dependency resolution, and lifecycle management. It is in daily use across founder labs. Pangenome construction (vg, PGGB, HPRC tooling) and Pinello's CRISPRme stack are mature, published, and proven at scale. Tan's reasoning-scaffold prototype was demoed in October 2025. Our design draws on prior agent prototypes (SciAgents, Virtual Lab) and workflow managers (Galaxy, Nextflow, Snakemake), filling a different slot. Liverpool's inaugural Hive Mind grant addresses hybrid coordination for wet-lab autonomous chemistry; we address the parallel pattern for computational and clinical genomics, complementary.

(95 words)

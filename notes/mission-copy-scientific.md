# Mission Copy Alternative: Scientific

Task: `mission-copy-scientific`

Scope: Rewrite only the mission body paragraphs currently in `index.html` lines 1147-1170. These are alternatives for downstream synthesis; `index.html` was not edited.

## Current Shape

The current mission body uses three paragraphs:

- Problem: AI agents can do research work, but coordination remains organizational.
- Method/tool: Poietic builds open-source products and methods; WorkGraph records task graph activity for review.
- Positioning: WorkGraph is an instrument and proof surface for broader organizational theory.

## Alternative 1: Research Coordination

AI systems can now help search literature, write analysis code, draft protocols, and inspect data. The harder research problem is coordination: keeping human judgment visible while work moves across people, models, datasets, reviews, and time.

We build open-source tools and practices for hybrid research teams that need evidence they can inspect and results they can reproduce. Our first product is [WorkGraph](https://graphwork.github.io/): a Rust task-coordination system where humans and AI agents share one dependency graph, with claims, prompts, logs, artifacts, reviews, and handoffs preserved as part of the work.

WorkGraph is a usable instrument, not a metaphor. It lets Poietic run research, product development, and public demonstrations in a form that can be reviewed after the fact: what was attempted, who or what acted, which evidence was used, where judgment entered, and why a result should be trusted.

## Alternative 2: Evidence Trail

AI agents can accelerate literature review, coding, data analysis, and experimental planning. For scientific work, speed is not enough. Research teams also need coordination records that show how conclusions were produced, challenged, revised, and connected to evidence.

Poietic builds open-source infrastructure for human-AI research work that is inspectable, reviewable, and reproducible. Our first product is [WorkGraph](https://graphwork.github.io/): a Rust system where people and agents coordinate tasks in the same dependency graph, attaching claims, execution logs, artifacts, decisions, failures, and review history to the work itself.

WorkGraph gives Poietic a practical testbed for organizational methods. We use it to run studies, demos, and product work in a way that exposes handoffs and uncertainty instead of hiding them in chat transcripts or local memory. The goal is research coordination that can be evaluated, repeated, and improved.

## Alternative 3: Reproducible Hybrid Work

Modern AI can contribute to many parts of research: searching papers, generating code, checking data, drafting arguments, and proposing next steps. The bottleneck is making those contributions accountable to human review, shared evidence, and reproducible process.

Poietic builds tools for research groups that want AI assistance without losing the structure of scientific work. Our first product is [WorkGraph](https://graphwork.github.io/): an open Rust task-coordination system where human and machine contributions live in one graph, with dependencies, artifacts, execution records, reviews, completions, and failures kept available for inspection.

WorkGraph is Poietic's operating instrument and its first public proof surface. It helps teams coordinate real human-AI work while preserving enough context to ask scientific questions about the process: what changed, what evidence supported it, what was reviewed, and whether another team could understand or reproduce the path.

## Provenance Notes

- `index.html` mission section, lines 1147-1170: source text and length/structure constraints.
- FAIR principles, Wilkinson et al. 2016, *Scientific Data*, https://www.nature.com/articles/sdata201618: supports the copy emphasis on reusable, inspectable research artifacts and metadata.
- National Academies, *Enhancing the Effectiveness of Team Science* 2015, https://www.nationalacademies.org/publications/19007: supports the copy emphasis on coordination as a core research-team problem.
- Scientific workflow provenance literature, including Lin et al. 2023 survey, https://journals.sagepub.com/doi/10.3233/JHS-222017, and workflow-run provenance work, https://arxiv.org/abs/2312.07852: supports the copy emphasis on execution records, artifacts, reviewability, and reproducibility.

## Absorptive Capacity Assessment

- High fit: the existing mission already names auditable, reproducible, inspectable work and WorkGraph already stores task dependencies, logs, artifacts, histories, and handoffs.
- Low prerequisite gap: the page already contains founder/research examples and WorkGraph positioning, so the scientific framing can be absorbed without changing the product claim.
- Main risk: overclaiming full scientific reproducibility. The alternatives avoid saying WorkGraph guarantees reproducible results; they say it preserves evidence and process so work can be reviewed, repeated, and improved.

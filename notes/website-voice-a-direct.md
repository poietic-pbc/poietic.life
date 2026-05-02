# Voice A: direct/operational

Drop-in replacement for `index.html` lines 1147-1170.

## Replacement text

WorkGraph runs a team of humans and AI agents on one shared dependency graph. You add a task with `wg add`, attach acceptance criteria, name the actor (a person, a Claude executor, a Codex executor, an open-weight model), and the service daemon dispatches when dependencies clear. Each task records its claim, prompt, execution log, artifacts, completion, failures, and handoffs. The graph lives in `.workgraph/graph.jsonl`, one JSON object per line, git-friendly, no server required. You can inspect any task with `wg show`, fan out subtasks with `wg add --after`, run probes that test whether the work actually matched its intent, and reconstruct who did what and why the result should be trusted.

The founders use WorkGraph for the work they already had to do. Erik runs his lab's pangenomics research and daily coordination on it, including ongoing pseudo-homologous region work. Luca uses it for genomic-AI workflow coordination in the Pinello lab. Vaughn uses the resulting traces as the empirical material for his organizational research. Poietic PBC itself was incorporated through a WorkGraph run, and the full task graph is browsable at https://ulivo.poietic.life/wg/feeds/incorporation-trace/.

The Delaware filing names one public benefit purpose: to make human and machine collaboration legible and responsive to its participants. That is the operating constraint on every WorkGraph feature. Evidence stays attached to tasks, handoffs are recorded, failures stay visible, and the people in the loop can intervene at any node. Open source under MIT, written in Rust.

## 50-word self-justification

Voice A starts with the verb. Para 1 answers "can you run a team on it?" with the operational shape: tasks, actors, daemon, graph file. Para 2 grounds the claim in founder dogfooding. Para 3 demotes the PBC mission to one operating constraint, not centerpiece. No "proof surface," no metaphor.

## Notes

- Length: 239 words across three paragraphs (within the 200-250 target).
- No em-dashes; founder order Erik / Luca / Vaughn; no PI language; no "in production today" or "wrote this proposal with WorkGraph" overclaim.
- Replaces the Erik-flagged self-aware framing ("WorkGraph is the instrument, not the whole institution," "proof surface for the theory of organizational patterns") with operational description plus dogfooding evidence.
- The PBC mission language is preserved verbatim from the Delaware filing but moved to a third-paragraph constraint, not the centerpiece of every sentence.
- The incorporation-trace URL is the publicly browsable evidence that backs the dogfooding claim without making the proposal-recursion overclaim.

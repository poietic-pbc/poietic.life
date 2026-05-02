# CTA Review Panel Synthesis

Task: `synthesize-cta-review-panel`
Date: 2026-05-02

## Recommendation

Rewrite section `04/04 get involved` around one concrete path:

1. Inspect Poietic's live WorkGraph.
2. Use the docs to start a graph in your own repo.
3. Use GitHub/source/theory as the deeper evidence trail.

The current CTA is credible but diffuse: docs, repo, code, paper, and live mirror all appear in one sentence, while the buttons expose only docs and GitHub. The synthesized direction is "live proof first, adoption second, theory/source third." This keeps Poietic's restrained voice but makes WorkGraph feel usable for coordinating AI/ML efforts, virtual research teams, and large or diverse dataset studies.

## Best Byline / Headline Options

Recommended:

Byline / section title:

**start a work graph**

Headline:

**Inspect the live graph. Build your own.**

Why: The byline shifts `get involved` from a vague invitation to a concrete action. The headline keeps the existing inspect/evaluate posture, adds a concrete adoption path, and avoids sounding like generic SaaS conversion copy.

Strong alternatives:

1. **Byline:** coordinate AI/ML work
   **Headline:** Run your next hybrid study in a graph.
   Best when the page wants to emphasize AI/ML and dataset-scale research more directly.

2. **Byline:** launch a virtual effort
   **Headline:** Spin up a research effort without losing the thread.
   Best when the desired audience is labs, virtual organizations, and distributed teams.

3. **Byline:** make the work inspectable
   **Headline:** Coordinate the work behind the model.
   Best for ML teams comparing methods, datasets, agents, and review outputs.

4. **Byline:** audit the agent work
   **Headline:** Turn AI help into a study you can audit.
   Best for reviewers who care most about provenance, reproducibility, and accountable agent use.

## Body Copy Options

Recommended:

> Open the same WorkGraph Poietic uses to coordinate product work, research planning, agent handoffs, and reviews. Then use the docs to start a graph for your own AI/ML study, virtual effort, or large-dataset workflow.

Alternative A, more scientific:

> Use WorkGraph to decompose an AI/ML study into tasks, dependencies, agents, artifacts, and reviews. Fan out across datasets or methods, then gather the evidence back into one inspectable record.

Alternative B, more organizational:

> WorkGraph lets a small team spin up a virtual effort without losing the thread: assign ready work, preserve handoffs, track failures, and keep decisions tied to the artifacts that produced them.

Alternative C, more skeptical/reviewer-facing:

> WorkGraph is not a canned demo. It is the coordination layer Poietic uses in public. Inspect the live graph, read the docs, and audit the source before deciding whether the practice is useful.

## Recommended Button / Link Set

Primary button:

- `Inspect the live graph` -> `https://ulivo.poietic.life/wg/feeds/workgraph-itself/`

Secondary buttons:

- `Build from the docs` -> `https://graphwork.github.io/`
- `View source on GitHub` -> `https://github.com/graphwork/workgraph`

Inline text link:

- `organizational patterns paper` -> `https://graphwork.github.io/organizational-patterns.html`

Rationale: The primary action should open the proof artifact, not the docs homepage. Docs and GitHub serve the visitor who is ready to adopt or inspect implementation details. The paper remains useful, but as an inline trust/provenance link rather than a competing primary action.

## Exact Proposed Replacement HTML

Replace only the contents of the current `<!-- ============ CTA ============ -->` section in `index.html` with:

```html
<!-- ============ CTA ============ -->
<section class="shell cta" id="cta">
  <div class="section-head">
    <span class="section-index">04<span class="slash">/04</span></span>
    <span class="section-title">start a work graph</span>
    <span class="section-rule"></span>
  </div>

  <div class="cta-inner">
    <div>
      <h2>Inspect the live graph.<br>Build your own.</h2>
      <p>
        Open the same WorkGraph Poietic uses to coordinate product work,
        research planning, agent handoffs, and reviews. Then use the docs to
        start a graph for your own AI/ML study, virtual effort, or
        large-dataset workflow. For the deeper model, read the
        <a href="https://graphwork.github.io/organizational-patterns.html">organizational patterns paper</a>.
      </p>
    </div>
    <div class="cta-actions">
      <a class="btn primary" href="https://ulivo.poietic.life/wg/feeds/workgraph-itself/">
        <svg width="14" height="14" viewBox="0 0 16 16" fill="none" stroke="currentColor" stroke-width="1.3" aria-hidden="true">
          <path d="M2.5 3.5 H6.5 V7.5 H2.5 Z"/>
          <path d="M9.5 2.5 H13.5 V6.5 H9.5 Z"/>
          <path d="M9.5 9.5 H13.5 V13.5 H9.5 Z"/>
          <path d="M6.5 5.5 H9.5"/>
          <path d="M6.5 6.5 L9.5 10.5"/>
        </svg>
        Inspect the live graph
        <span class="arrow">&rarr;</span>
      </a>
      <a class="btn" href="https://graphwork.github.io/">
        <svg width="14" height="14" viewBox="0 0 16 16" fill="none" stroke="currentColor" stroke-width="1.3" aria-hidden="true">
          <path d="M3 2 H10 L13 5 V14 H3 Z"/>
          <path d="M10 2 V5 H13"/>
          <path d="M5 8 H11"/>
          <path d="M5 10.5 H11"/>
          <path d="M5 13 H9"/>
        </svg>
        Build from the docs
        <span class="arrow">&rarr;</span>
      </a>
      <a class="btn" href="https://github.com/graphwork/workgraph">
        <svg width="14" height="14" viewBox="0 0 16 16" fill="currentColor" aria-hidden="true">
          <path d="M8 0C3.58 0 0 3.58 0 8a8 8 0 0 0 5.47 7.59c.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82a7.4 7.4 0 0 1 2-.27c.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.01 8.01 0 0 0 16 8c0-4.42-3.58-8-8-8Z"/>
        </svg>
        View source on GitHub
        <span class="arrow">&rarr;</span>
      </a>
    </div>
  </div>
</section>
```

## Rationale And Tradeoffs

This recommendation combines the strongest points from the three upstream CTA angles:

- From user/adoption: lead with a use case, make fan-out/fan-in and auditable records concrete, and invite a low-friction first action.
- From product/conversion: make the live graph the primary action, separate visitor intents, and use descriptive action labels.
- From scientific coordination: name AI/ML studies, virtual efforts, large datasets, handoffs, reviews, and inspectable provenance.

The main tradeoff is specificity versus breadth. The recommended copy names AI/ML and large-dataset work, which makes the CTA more concrete for the intended audience but slightly less universal for writing-only or general organizational visitors. That is acceptable because the rest of the page already explains Poietic broadly; the CTA should now convert a motivated technical or research visitor into inspection and trial.

The second tradeoff is "live graph" before "docs." This may send some visitors to a denser artifact first, but that density is the product proof: WorkGraph's differentiator is inspectable coordination in use. The docs button remains immediately available for visitors who want the implementation path.

Avoid stronger phrases such as "Launch your virtual lab" or "Transform AI collaboration" in the final CTA. They are energetic, but they ask the page to promise onboarding and organizational outcomes that are not yet fully supported by visible intake, templates, permissions, or hosted collaboration infrastructure.

# Synthesized Mission Copy Alternatives

Task: `synthesize-mission-copy-alternatives`

Scope: Recommend a replacement for the `index.html` mission body paragraphs only. Do not edit `index.html`.

## Recommendation

Use Version A. It is the strongest blend of the upstream alternatives: plainspoken, organizational, concrete about WorkGraph, and still tied to evidence, review, and public-benefit legibility. It is also shorter than the current body while preserving the substance.

## Version A: Recommended

AI agents can already search literature, write code, analyze data, and support scientific design. The harder problem is coordination: helping people and machines work together over days or weeks while keeping judgment, evidence, handoffs, and changes visible.

Poietic builds open-source products, live demonstrations, and working methods for that kind of collaboration. Our first product is [WorkGraph](https://graphwork.github.io/), a Rust task-coordination system where humans and AI agents share one dependency graph, with claims, execution logs, artifacts, completions, handoffs, and histories preserved for review.

WorkGraph is the first instrument, not the whole institution. It gives Poietic a practical way to test the [theory of organizational patterns](https://graphwork.github.io/theory/) in real work. The public-benefit goal is to make human-machine collaboration legible and responsive to its participants, including the work, the failures, and the evidence trail.

### Exact HTML Replacement

Replace the contents of `<div class="mission-body">` with:

```html
      <p>
        AI agents can already search literature, write code, analyze data, and
        support scientific design. The harder problem is coordination: helping
        people and machines work together over days or weeks while keeping
        judgment, evidence, handoffs, and changes visible.
      </p>
      <p>
        Poietic builds open-source products, live demonstrations, and working
        methods for that kind of collaboration. Our first product is
        <a href="https://graphwork.github.io/">WorkGraph</a>, a Rust
        task-coordination system where humans and AI agents share one dependency
        graph, with claims, execution logs, artifacts, completions, handoffs, and
        histories preserved for review.
      </p>
      <p>
        WorkGraph is the first instrument, not the whole institution. It gives
        Poietic a practical way to test the
        <a href="https://graphwork.github.io/theory/">theory of organizational patterns</a>
        in real work. The public-benefit goal is to make human-machine
        collaboration legible and responsive to its participants, including the
        work, the failures, and the evidence trail.
      </p>
```

## Alternate 1: More Plainspoken

AI agents can now do useful work: search literature, write code, analyze data, and help with scientific design. What remains difficult is keeping the collaboration organized across people, agents, days, and decisions.

Poietic builds open-source tools and practical methods for human-AI teams. Our first product is [WorkGraph](https://graphwork.github.io/), a Rust task-coordination system where humans and AI agents work in the same dependency graph, with claims, logs, handoffs, artifacts, completions, and histories kept for review.

WorkGraph is our first instrument inside a larger public-benefit project. It lets Poietic test the [theory of organizational patterns](https://graphwork.github.io/theory/) through real work, so collaboration becomes easier to inspect, question, and improve. The goal is simple: make the work, evidence, handoffs, and failures visible to the people involved.

### Exact HTML Replacement

```html
      <p>
        AI agents can now do useful work: search literature, write code, analyze
        data, and help with scientific design. What remains difficult is keeping
        the collaboration organized across people, agents, days, and decisions.
      </p>
      <p>
        Poietic builds open-source tools and practical methods for human-AI
        teams. Our first product is
        <a href="https://graphwork.github.io/">WorkGraph</a>, a Rust
        task-coordination system where humans and AI agents work in the same
        dependency graph, with claims, logs, handoffs, artifacts, completions,
        and histories kept for review.
      </p>
      <p>
        WorkGraph is our first instrument inside a larger public-benefit project.
        It lets Poietic test the
        <a href="https://graphwork.github.io/theory/">theory of organizational patterns</a>
        through real work, so collaboration becomes easier to inspect, question,
        and improve. The goal is simple: make the work, evidence, handoffs, and
        failures visible to the people involved.
      </p>
```

## Alternate 2: More Research-Oriented

AI agents can accelerate literature review, coding, data analysis, and experimental planning. Speed is not enough. Teams also need coordination records that show how work was produced, challenged, revised, and connected to evidence.

Poietic builds open-source infrastructure and methods for human-AI work that can be inspected and reviewed. Our first product is [WorkGraph](https://graphwork.github.io/), a Rust task-coordination system where people and agents share one dependency graph, preserving claims, execution logs, artifacts, handoffs, completions, and histories.

WorkGraph is Poietic's first public proof surface for the [theory of organizational patterns](https://graphwork.github.io/theory/). It lets us run product work, demos, and research practice in a form that keeps judgment visible. The aim is human-machine collaboration that participants can understand, evaluate, and improve.

### Exact HTML Replacement

```html
      <p>
        AI agents can accelerate literature review, coding, data analysis, and
        experimental planning. Speed is not enough. Teams also need coordination
        records that show how work was produced, challenged, revised, and
        connected to evidence.
      </p>
      <p>
        Poietic builds open-source infrastructure and methods for human-AI work
        that can be inspected and reviewed. Our first product is
        <a href="https://graphwork.github.io/">WorkGraph</a>, a Rust
        task-coordination system where people and agents share one dependency
        graph, preserving claims, execution logs, artifacts, handoffs,
        completions, and histories.
      </p>
      <p>
        WorkGraph is Poietic's first public proof surface for the
        <a href="https://graphwork.github.io/theory/">theory of organizational patterns</a>.
        It lets us run product work, demos, and research practice in a form that
        keeps judgment visible. The aim is human-machine collaboration that
        participants can understand, evaluate, and improve.
      </p>
```

## Rationale

- Version A best satisfies the brief: less self-aware and uncanny than the current text, more natural than the scientific versions, and more complete than the short organizational alternatives.
- It preserves the required substance: AI agents can do useful work; coordination is the hard problem; Poietic builds open tools, demos, and methods; WorkGraph is the first product/instrument; the public-benefit aim is legible, responsive human-machine collaboration.
- It keeps the existing section shape and links, so it can replace the current mission body without layout or content-architecture changes.
- It avoids overclaiming reproducibility. The copy says WorkGraph preserves process and evidence for review, not that it guarantees scientific results.

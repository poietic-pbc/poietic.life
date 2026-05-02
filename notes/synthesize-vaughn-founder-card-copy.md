# Synthesize Vaughn Founder-Card Copy

Task: `synthesize-vaughn-founder-card-copy`  
Date: 2026-05-01/02  
Scope: fan-in synthesis from the four Vaughn review artifacts. No site/source files edited.

## Recommendation

Replace the current Vaughn founder-card bio with this compact two-link version:

```html
Author of <em>The Uncertainty Mindset</em> (Columbia University Press,
2020) and a Harvard PhD in organizational behavior/sociology. Tan studies
<a href="https://vaughntan.org/notknowing">not-knowing</a>, adaptive
organization design, and
<a href="https://vaughntan.org/reasoningscaffolds">reasoning scaffolds</a>
for work where facts, tradeoffs, and human judgment must stay visible in
hybrid human-AI coordination.
```

Plain-text equivalent:

> Author of *The Uncertainty Mindset* (Columbia University Press, 2020) and a Harvard PhD in organizational behavior/sociology. Tan studies not-knowing, adaptive organization design, and reasoning scaffolds for work where facts, tradeoffs, and human judgment must stay visible in hybrid human-AI coordination.

## Why This Version

The replacement keeps roughly the same footprint as the existing blurb while making Vaughn's contribution more specific. It shifts from a loose topic list to an integrated claim: his work helps teams act under genuine uncertainty while keeping reasoning and judgment inspectable.

The two links are deliberate:

- `not-knowing` -> `https://vaughntan.org/notknowing`
  - Best stable umbrella for uncertainty, organization design, innovation, and adaptive work.
  - Stronger first click than the rolling `/page/1` archive because it explains the core framework rather than sending readers to a changing index.
- `reasoning scaffolds` -> `https://vaughntan.org/reasoningscaffolds`
  - Best WorkGraph-specific proof point for explicit reasoning, subjective judgment, AI-supported work, and auditable decision structure.
  - More directly supports the card's human-AI coordination claim than a general newsletter/archive link.

I would not add `agentconstruct` as a third link. It is highly relevant to WorkGraph's agent architecture, but three links would make the card feel like a reading list. If the card must use only one link, use `reasoning scaffolds`; it is the clearest bridge between Vaughn's public writing and WorkGraph's emphasis on visible judgment in AI-supported work.

## Fit Against Current Card

Current Vaughn card:

```html
Author of <em>The Uncertainty Mindset</em> (Columbia University Press,
2020) and a Harvard PhD in organizational behavior/sociology. Tan
<a href="https://vaughntan.org/page/1">writes about</a>
AI agents, reasoning scaffolds, public strategy, and not-knowing;
that work informs WorkGraph's approach to keeping human
judgment explicit in hybrid human-AI research coordination.
```

The proposed copy is slightly shorter in structure and similar in rendered density. It also removes the weak generic anchor text `writes about`, avoids the unstable archive target, and uses concrete linked concepts that a reader can understand before clicking.

## Rejected Alternatives

Single-link `not-knowing` version: cleanest visually, but it underplays the AI/reasoning connection that the downstream card specifically needs.

Two-link `not-knowing` plus `agentconstruct`: strong for WorkGraph architecture, but it risks making Vaughn's founder card sound like a narrow AI-agent citation rather than a broader organization-design contribution.

Post index or newsletter link: useful as a general profile destination, but too diffuse for a short founder-card claim.

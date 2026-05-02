# Review: Vaughn Founder-Card Link Options

Task: `review-vaughn-link-presentation-options`  
Date: 2026-05-01/02  
Scope: read-only review of `index.html` founder-card copy and Vaughn Tan's writing index at <https://vaughntan.org/page/1>. Site files were not edited.

## Current Markup

The Vaughn card in `index.html` currently uses one inline writing link:

```html
Tan
<a href="https://vaughntan.org/newsletter">writes about</a>
organization design, innovation, and team adaptation under uncertainty;
that work informs WorkGraph's approach to keeping human
judgment explicit in hybrid human-AI research coordination.
```

This is compact and readable, but the link target is broad and newsletter-oriented. The sentence already carries the right WorkGraph bridge: organization design, adaptation under uncertainty, and explicit human judgment.

## Source Observations

Vaughn's writing index at <https://vaughntan.org/page/1> is a dated archive with several recent posts that map closely to WorkGraph's positioning:

- <https://vaughntan.org/reasoningscaffolds> is the strongest specific post for WorkGraph. It centers explicit structures for subjective reasoning, human judgment, auditable reasoning artifacts, and AI systems that support rather than displace judgment.
- <https://vaughntan.org/meaningtools> is strong for the theme of AI tools supporting human meaning-making instead of merely generating outputs.
- <https://vaughntan.org/agentconstruct> is highly relevant to AI agents, decomposable roles, success criteria, trade-offs, and keeping meaning-making with humans, but it may read as a plug for a specific adjacent tool rather than as founder background.
- <https://vaughntan.org/notknowing> remains the best stable hub if the card gets only one conceptual link. It frames the uncertainty/not-knowing system, not just a dated post.
- <https://vaughntan.org/newsletter> is credible but weaker as the primary card link because it is partly a signup/archive page and less directly explanatory on first click.

## Options

### Option 1: One Link, Minimal Density

```html
Author of <em>The Uncertainty Mindset</em> (Columbia University Press,
2020) and a Harvard PhD in organizational behavior/sociology. Tan's
<a href="https://vaughntan.org/notknowing">work on not-knowing</a>
spans organization design, innovation, and team adaptation under
uncertainty; it informs WorkGraph's approach to keeping human judgment
explicit in hybrid human-AI research coordination.
```

Readability: high.  
Density: low.  
Best use: safest default.

This preserves the card's current shape and replaces a vague newsletter link with a stable conceptual hub. It is the best balance for a landing-page founder card because it gives reviewers one clear first click without making the bio feel like a bibliography.

### Option 2: Two Inline Links, Still Compact

```html
Author of <em>The Uncertainty Mindset</em> (Columbia University Press,
2020) and a Harvard PhD in organizational behavior/sociology. Tan writes
about <a href="https://vaughntan.org/notknowing">not-knowing</a>,
organization design, and
<a href="https://vaughntan.org/reasoningscaffolds">reasoning scaffolds</a>;
that work informs WorkGraph's approach to keeping human judgment explicit
in hybrid human-AI research coordination.
```

Readability: high-medium.  
Density: medium.  
Best use: recommended if the synthesis task wants both breadth and one WorkGraph-specific proof point.

This adds one more link but keeps both links semantically meaningful. "Not-knowing" gives the broad uncertainty framework; "reasoning scaffolds" gives the human-AI judgment bridge. It is slightly more information-dense than the current sentence but not bloated.

### Option 3: Post Index Plus One Specific Post

```html
Author of <em>The Uncertainty Mindset</em> (Columbia University Press,
2020) and a Harvard PhD in organizational behavior/sociology. Tan's
<a href="https://vaughntan.org/page/1">recent writing</a> connects
organization design, uncertainty, and human-AI work, including
<a href="https://vaughntan.org/reasoningscaffolds">reasoning scaffolds</a>
for making subjective judgment explicit.
```

Readability: medium.  
Density: medium-high.  
Best use: only if the card should foreground "recent writing" as evidence.

The post index is compact and current, but linking to `/page/1` is less stable as a semantic target because the contents will roll forward. It also makes the copy feel more like a citation trail. The specific reasoning-scaffolds link is doing most of the substantive work here.

### Option 4: Rewritten Sentence With Richer Themes

```html
Author of <em>The Uncertainty Mindset</em> (Columbia University Press,
2020) and a Harvard PhD in organizational behavior/sociology. Tan studies
<a href="https://vaughntan.org/notknowing">not-knowing</a>, adaptive
organization design, and human
<a href="https://vaughntan.org/meaningtools">meaning-making with AI</a>;
that work informs WorkGraph's approach to coordinating machine assistance
without hiding the human judgments that set direction.
```

Readability: medium-high.  
Density: medium.  
Best use: if the card wants sharper thematic alignment with WorkGraph rather than a conservative credential-plus-topic sentence.

This is richer and more differentiated, but it introduces heavier conceptual language. "Meaning-making" is accurate to Vaughn's writing, yet it may need nearby plain-language support to avoid sounding abstract. The final clause is stronger than "hybrid human-AI research coordination" because it says what WorkGraph protects.

## Recommendation

Use Option 2 if the card can tolerate two links. It is compact, keeps the existing sentence rhythm, and gives both a stable framework link and a specific WorkGraph-relevant post:

- `not-knowing` -> <https://vaughntan.org/notknowing>
- `reasoning scaffolds` -> <https://vaughntan.org/reasoningscaffolds>

If the synthesis task strongly prioritizes quiet visual density, use Option 1 instead. Avoid making `/page/1` the primary link; it is useful for review, but less durable and less self-explanatory than the not-knowing hub or the reasoning-scaffolds article.

## Density Judgment

One link is the cleanest visual choice and enough for a founder card. Two inline links are still acceptable because both are short noun phrases embedded in prose. Three or more links would make Vaughn's card visibly denser than the Erik and Luca cards and would shift the component from founder summary to reading list.

# CTA Product Demo / Conversion Notes

Task: `cta-product-demo-conversion`
Date: 2026-05-02

## Current CTA Diagnosis

The existing section is tonally aligned: "Inspect the instrument. Evaluate the practice." matches the restrained Poietic voice and treats WorkGraph as evidence, not hype. The conversion weakness is that the action is diffuse. The paragraph offers docs, repo, code, paper, and live mirror in one sentence, while the buttons only expose docs and GitHub. A motivated visitor can proceed, but the highest-value next step is not obvious.

The product-oriented CTA should make one concrete promise: see WorkGraph doing real work now, then choose the depth of engagement. This preserves the page's epistemic tone while giving visitors a clearer path from curiosity to product evaluation.

## Messaging Principles

1. Lead with the live proof surface, not the abstract product category. WorkGraph's differentiator is not "task coordination" in general; it is an inspectable graph of actual human-agent work.
2. Use verbs that name the next screen: "Open the live graph", "Read the docs", "Clone WorkGraph", "Start a virtual effort." Avoid vague verbs like "learn more" or "get involved."
3. Separate intent levels. Primary CTA = evaluate the live product. Secondary CTAs = use it, inspect source, understand theory, start a collaboration.
4. Keep claims falsifiable. Favor "inspect", "run", "trace", "clone", "coordinate" over "transform", "unlock", "revolutionize", or "future of work."
5. Make the visitor's job concrete. The CTA should invite a reviewer, researcher, or builder to test whether WorkGraph can make a real effort legible.
6. Preserve Poietic restraint. The copy can be motivating without sounding like SaaS demand generation: quiet confidence, explicit artifacts, no urgency theater.

## Provenance / Research Basis

- Current page context: `index.html` CTA offers docs, GitHub, the organizational-patterns paper, and the live WorkGraph mirror; hero already exposes "Open WorkGraph" and "Live demo."
- WorkGraph docs position the product as "task graphs for humans and agents" with no server/account requirement and a `.workgraph/` directory in a repo: https://graphwork.github.io/
- WorkGraph theory page frames trace/provenance as organizational memory and connects the product primitives to formal organizational models: https://graphwork.github.io/theory/
- Live proof target: https://ulivo.poietic.life/wg/feeds/workgraph-itself/
- Source inspection target: https://github.com/graphwork/workgraph
- CTA/link usability: HarvardSites recommends concise, action-oriented, descriptive link text that tells users what will happen when clicked: https://designsystem.harvardsites.harvard.edu/keep-cta-link-text-clear-and-actionable
- Button usability: Baymard emphasizes clear button intent, visible primary action, and descriptive microcopy so users understand the next step: https://baymard.com/learn/button-design
- CTA placement research: Hernandez and Resnick's eye-tracking study found landing pages with clearer scan paths produced more fixations and click-throughs on the target CTA: https://doi.org/10.1177/1541931213571232
- Absorptive-capacity lens: Cohen and Levinthal define absorptive capacity as the ability to recognize, assimilate, and apply external knowledge, largely dependent on prior related knowledge. For Poietic, visitors already have enough adjacent knowledge to absorb "live graph/docs/GitHub"; "start a virtual effort" may need more scaffolding: https://doi.org/10.2307/2393553

## Candidate CTA Configurations

### 1. Open the live graph

**Headline:** See WorkGraph doing real work.

**Body:** Open the same graph Poietic uses to coordinate product work, writing, research planning, and agent handoffs. Inspect the tasks, logs, artifacts, and dependencies before deciding whether the model is useful.

**Buttons:** Primary: `Open the live graph` -> live WorkGraph mirror. Secondary: `Read the docs` -> WorkGraph docs. Tertiary text link: `View source on GitHub`.

**Best for:** Highest conversion clarity. Turns "get involved" into an immediate product evaluation.

**Absorptive capacity:** High. The current page already teaches "live proof surface" and "inspectable histories."

### 2. Run the instrument

**Headline:** Run WorkGraph in your own repo.

**Body:** WorkGraph is open source, git-native coordination infrastructure for humans and agents. Read the quickstart, install the CLI, and try a small effort where every handoff remains inspectable.

**Buttons:** Primary: `Start with the quickstart` -> WorkGraph quickstart/docs. Secondary: `Clone WorkGraph` -> GitHub. Tertiary: `Inspect Poietic's live graph` -> live mirror.

**Best for:** Developers, researchers with codebases, and reviewers who want a concrete adoption path.

**Absorptive capacity:** High for technical visitors; medium for nontechnical grant reviewers unless paired with the live graph button.

### 3. Inspect first, then build

**Headline:** Inspect the proof. Then build your own.

**Body:** Start with Poietic's public graph to see how the work is represented. If the structure makes sense, use the docs and source to create a WorkGraph for a research, writing, or software effort of your own.

**Buttons:** Primary: `Inspect the live graph` -> live mirror. Secondary: `Build from the docs` -> docs. Secondary: `View source` -> GitHub.

**Best for:** Balanced product/conversion framing; keeps the evaluation posture while adding a next action.

**Absorptive capacity:** High. It reuses the page's existing "inspect/evaluate" language and adds a user path.

### 4. Make one effort legible

**Headline:** Make one effort legible.

**Body:** Bring a real collaborative task: a grant section, a software feature, a research comparison, or a small literature review. WorkGraph turns the work into tasks, dependencies, claims, artifacts, reviews, and a trace others can inspect.

**Buttons:** Primary: `Start a virtual effort` -> contact/intake target when available. Secondary: `See an example graph` -> live mirror. Secondary: `Read the WorkGraph docs` -> docs.

**Best for:** Future service/adopter-lab conversion, especially if Poietic wants conversations rather than only self-serve installs.

**Absorptive capacity:** Medium. The primitive is promising but needs a destination: intake form, email, GitHub issue template, or calendar link. Without that, the CTA overpromises.

### 5. Follow the evidence trail

**Headline:** Follow the work, not the pitch.

**Body:** The product is public enough to evaluate. Read the docs, inspect the source, and open the live graph to see how Poietic records decisions, handoffs, failures, and completed artifacts.

**Buttons:** Primary: `Open the evidence trail` -> live mirror. Secondary: `Read the docs` -> docs. Secondary: `Open GitHub` -> GitHub.

**Best for:** The most restrained Poietic tone. Strong fit for skeptical reviewers.

**Absorptive capacity:** High. It maps directly onto existing page claims about auditable, reproducible, inspectable work.

### 6. Coordinate a human-agent project

**Headline:** Coordinate human-agent work in a graph.

**Body:** WorkGraph gives each task a place, each agent a role, and each handoff a record. Use it when a project has too many people, agents, claims, and artifacts to keep in a chat transcript.

**Buttons:** Primary: `Use WorkGraph` -> docs/quickstart. Secondary: `Inspect live use` -> live mirror. Secondary: `Read the theory` -> organizational patterns/theory.

**Best for:** General product positioning. More direct than "instrument", less poetic than current copy.

**Absorptive capacity:** High for software/product audiences; medium for scientific collaborators unless examples remain nearby.

### 7. Evaluate the system in public

**Headline:** Evaluate the system in public.

**Body:** WorkGraph is not a canned demo. It is the coordination layer Poietic uses to build, review, and revise its own work. Inspect the live graph, audit the source, or start from the docs.

**Buttons:** Primary: `Inspect the live system` -> live mirror. Secondary: `Audit the source` -> GitHub. Secondary: `Start from the docs` -> docs.

**Best for:** Review-panel audience and external credibility. It turns openness into the product promise.

**Absorptive capacity:** High. "Not a canned demo" is already supported by the "what we've built" section's live examples.

## Recommended Direction

Use candidate 3 or 7 as the main replacement. They preserve the current "inspect/evaluate" stance but make the product path clearer. Candidate 3 is warmer and more adoption-oriented; candidate 7 is stronger for public-review credibility.

Recommended button order:

1. `Inspect the live graph` -> `https://ulivo.poietic.life/wg/feeds/workgraph-itself/`
2. `Build from the docs` or `Start from the docs` -> `https://graphwork.github.io/`
3. `View source on GitHub` -> `https://github.com/graphwork/workgraph`
4. Optional text link only: `Read the theory` -> `https://graphwork.github.io/theory/`

Avoid making `Open WorkGraph` the only primary CTA because it can read as docs/product homepage rather than live evaluation. The stronger conversion move is to put the proof artifact first and let docs/GitHub serve the visitor who wants to go deeper.

## New Primitive Candidates

These are role/workflow primitives that could be imported into the primitive store, stated at recombinable granularity.

1. **Live-proof CTA primitive**
   - Type: Messaging primitive
   - Definition: A CTA that points first to an inspectable live artifact rather than to marketing copy.
   - Test: Users can state what evidence they will see before clicking.
   - Provenance: WorkGraph live mirror; Baymard and Harvard descriptive-action guidance.
   - Absorptive capacity: High.

2. **Intent-tiered CTA stack**
   - Type: Conversion workflow primitive
   - Definition: One primary button for immediate evaluation, with secondary links for docs, source, and theory.
   - Test: Primary/secondary actions map to distinct visitor intents without duplicate verbs.
   - Provenance: Button hierarchy/intent guidance from Baymard; current Poietic action set.
   - Absorptive capacity: High.

3. **Bring-one-effort CTA**
   - Type: Adoption primitive
   - Definition: Invite users to apply the product to a bounded real task rather than to "join" abstractly.
   - Test: CTA names example effort types and has a working intake path.
   - Provenance: Product-led onboarding pattern adapted to WorkGraph's graph-native coordination use case.
   - Absorptive capacity: Medium; needs contact/intake infrastructure before full import.

4. **Evidence-trail framing primitive**
   - Type: Trust-building primitive
   - Definition: Present docs, live graph, source, and theory as an evidence trail rather than a menu.
   - Test: Visitor can follow from claim -> live use -> implementation -> theory.
   - Provenance: Poietic public-benefit/legibility frame; WorkGraph trace/provenance theory.
   - Absorptive capacity: High.

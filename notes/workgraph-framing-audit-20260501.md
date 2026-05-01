# WorkGraph homepage framing audit

Task: `audit-workgraph-framing`  
Date: 2026-05-01

## Summary

The current homepage framing is close, but exact repository statistics should either be removed from homepage copy or replaced with deliberately rounded numbers. The homepage should emphasize what the interface lets a reader inspect: a dependency graph, live feeds, claim/execute/complete lifecycle, agent handoffs, and durable histories. Rust, MIT, and open-source belong in metadata/CTA copy, not repeated stat blocks.

## Current Findings

- `index.html:1055` still renders a three-card stat block with `2,091` commits, `263,112` lines of code, and `83,196` test lines.
- `index.html:1052`, `index.html:1189`, and `index.html:1281` already carry the stronger non-defensive framing: MIT, Rust, open-source, live graph, dependency visualization, lifecycle, live feeds, handoffs, and inspectable histories.
- The defensive phrase `actual commits` has already been removed from the current working tree at `index.html:1058`; keep it removed.
- The CTA no longer repeats exact stats in the current working tree at `index.html:1281`; keep exact numbers out of that section.
- Prior note `notes/landing-page-v2-update-20260501.md:107` also identified the stat drift/repetition issue.

## Verified Repository Facts

Checked against `https://github.com/graphwork/workgraph.git` on 2026-05-01:

- `main` HEAD: `e70a837e`
- Commit count: `2,094` via `git rev-list --count HEAD`
- Source code: `263,544` code lines via `tokei src --exclude target`
- Test code: `83,489` code lines via `tokei tests --exclude target`

These are close to the homepage numbers but already stale. If exact numbers remain, the copy needs a refresh mechanism and a visible methodology footnote. For a landing page, the better choice is to drop exact LOC/test-line counts and use a qualitative proof point plus links to GitHub and the live graph.

## Recommended Homepage Changes

### Hero Metadata

Replace the current single metadata line and stat cards with one compact metadata line:

> MIT-licensed | Rust | open-source | live graph

Link `live graph` to `https://ulivo.poietic.life/wg/feeds/workgraph-itself/`.

If a numeric proof point is still desired, use one rounded clause only:

> MIT-licensed | Rust | open-source | 2,000+ commits | live graph

Do not include LOC or test-line counts in the hero.

### Hero Subcopy

Current direction is good. Recommended final copy:

> Persistent coordination graphs for hybrid human-AI work. Humans and agents claim, execute, hand off, and complete interdependent tasks while WorkGraph records the dependency graph, live feeds, decisions, artifacts, and histories that make the process inspectable.

This says what the interface does and avoids vague "better research" language.

### Mission WorkGraph Paragraph

Recommended copy:

> We build open-source infrastructure that makes hybrid human-AI research auditable, reproducible, and inspectable. Our first product is WorkGraph: a Rust task-coordination system where humans and AI agents work in the same dependency graph, with claims, execution logs, handoffs, completions, artifacts, and histories preserved for review.

### What We've Built Lead

Recommended copy:

> WorkGraph is functional, MIT-licensed, and open-source. It provides dependency visualization, live feeds, claim/execute/complete workflows, agent handoffs, and inspectable histories. We use it for incorporation, writing, grant drafting, and research coordination.

### CTA

Recommended copy:

> WorkGraph is MIT-licensed and actively developed. Read the docs, clone the Rust repo, inspect the code, or open the live WorkGraph mirror.

## Copy to Avoid

- `actual commits`
- Exact LOC/test-line counts unless generated automatically
- Multiple stat blocks repeating the same repository claims
- "WorkGraph builds itself" as a headline proof point unless it links directly to a clear, inspectable live graph explaining that claim

## Recommendation for Integrator

Keep the current working-tree changes that removed `actual commits` and eliminated the CTA stat repetition. Replace or remove the hero stat cards at `index.html:1055`; the strongest landing-page version removes the stat cards entirely and keeps proof in the GitHub/live-graph links. If layout needs the stat cards, use interface-surface labels instead of volatile numbers:

- Dependency graph
- Live feeds
- Inspectable histories

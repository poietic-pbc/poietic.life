# Poietic Site Agent Guide

This repository publishes the Poietic PBC landing page. Treat changes here as
live-site work: keep edits small, sync before changing files, commit, and push
to `origin/main` when the requested change is complete.

## WorkGraph First

Use WorkGraph for nontrivial work. Research, review, copy exploration, fact
checking, bug reports, and multi-step investigations should be represented as
`wg` tasks so the trace is inspectable.

In this repo, plain `wg` talks to the Poietic website graph. Use it for site
tasks:

```sh
wg status
wg add "Task title" --id task-id -d "..." --deliverable notes/task-id.md --no-place
```

For upstream WorkGraph product tasks, do not use plain `wg` from this checkout.
Use the WorkGraph graph explicitly:

```sh
wg --dir /home/erik/workgraph/.wg status
wg --dir /home/erik/workgraph/.wg add "Task title" --id task-id -d "..." --deliverable bug-or-note.md --no-place
```

## Editing The Site

Use the clean live-edit worktree for website changes:

```sh
cd /tmp/poietic-life-mission-copy
git fetch origin
git pull --ff-only origin main
```

Make page edits there, then verify and push:

```sh
git diff --check
git status --short --branch
git add <files>
git commit -m "Short imperative summary"
git push origin HEAD:main
```

The main checkout at `/home/erik/poietic.life` is often dirty with WorkGraph
state, notes, and agent worktrees. Do not use that checkout for direct live-site
edits unless the user explicitly asks you to.

## Page Conventions

- The primary page is `index.html`.
- Keep language concrete. Avoid describing real traces as "demos" when they are
  actual operating work.
- Live WorkGraph feeds are evidence surfaces. Link them inline or in relevant
  cards without over-framing them.
- Keep mobile layout readable. Do not widen all text just to fix the graph
  iframe; adjust only the graph surface when that is the issue.
- Before editing facts about people, papers, citations, or affiliations, create
  or use a fact-checking task and cite durable sources where possible.

## Current Important Links

- WorkGraph docs: `https://graphwork.github.io/`
- WorkGraph source: `https://github.com/graphwork/workgraph`
- Live WorkGraph feed: `https://ulivo.poietic.life/wg/feeds/workgraph-itself/`
- Poietic website trace: `https://ulivo.poietic.life/wg/feeds/poietic-website/`
- Incorporation trace: `https://ulivo.poietic.life/wg/feeds/incorporation-trace/index.html`
- Grant trace: `https://ulivo.poietic.life/wg/feeds/google_ai_for_science/`
- PHR trace: `https://ulivo.poietic.life/wg/feeds/phrs-cnv-study/`

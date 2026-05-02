# Website site audit — poietic.life — 2026-05-01

Auditor: agent-252 (site-audit-read).
Calibration: Erik flagged the mission paragraph 3 ("WorkGraph is the
instrument, not the whole institution. It gives Poietic a proof surface
for the theory of organizational patterns…") as too self-aware and
uncanny. Diagnosis: when the reader asks *can you run a team on it?*,
they should get YES + how, not a paragraph about proof surfaces.

Both the deployed file (`~/poietic.life/index.html`, 1417 lines) and
the over-the-wire fetch from `https://poietic.life` were read. They match.

## 1. Headline verdict

The page is **mostly clean**, but the same rough pattern Erik flagged
appears in three more places, all early on the page (hero subhead,
mission lead, built-section lead). All three reach for an abstraction
("semi-autonomous", "proof surface", "demo surface", "legible
collaboration") in the exact spot where a concrete answer to *what does
this company do? can you use it?* would land harder. The middle of the
page (mission body p1+p2, founder cards, two of the three built cards,
the CTA) reads clean by Erik's bar; do not touch those.

## 2. Rough spots

| Anchor | Current text | Diagnosis | Proposed fix |
|---|---|---|---|
| `.hero-sub` (lines 1069-1074) | "Poietic is a semi-autonomous public-benefit organization where people and AI agents build tools, demos, and theory for legible collaboration. WorkGraph is our first instrument: a live proof surface where humans and agents coordinate tasks, handoffs, decisions, artifacts, and histories." | **Same pattern as Erik's flagged paragraph, in the most-read slot on the page.** "Semi-autonomous", "live proof surface", "legible collaboration" are all abstractions where concrete should be. A reader who lands here cannot answer *what does this do?* | "Poietic PBC builds open-source tools so humans and AI agents can run real projects together: incorporation, grant writing, scientific analysis. Our first tool is WorkGraph: a task graph where people and agents share tasks, hand off work, and leave a record anyone can read back." |
| `.mission-lead` (lines 1141-1145) | "Poietic is a semi-autonomous organization. Its purpose is to make human-machine collaboration legible. It builds open tools to support that mission." | Restates the hero in the same abstractions. "Semi-autonomous" is never defined on the page; reader has to guess. | "Poietic builds open-source tools so people and AI agents can do real work together, with the work itself visible to anyone who wants to inspect it." (drop "semi-autonomous"; the operating mode is clear from the live graph in the hero) |
| `.built-lead` (lines 1244-1250) | "WorkGraph is Poietic's first product and live demo surface. It is functional, MIT-licensed, and open-source, with dependency visualization, live feeds, claim/execute/complete workflows, agent handoffs, and inspectable histories. We use it to run incorporation, writing, grant drafting, and research coordination in public enough to be evaluated." | "Live demo surface" is the same jargon family as "proof surface". "in public enough to be evaluated" is awkward and meta. | "WorkGraph is Poietic's first product. MIT-licensed, written in Rust, with dependency visualization, live feeds, agent handoffs, and inspectable histories. Three things we ran on it ourselves are below; each links to the actual graph." |
| `.repo-stats` cell 3 (lines 1106-1108) | "Theory / legible collaboration" | Mild version of the same pattern; pairs with "Product / WorkGraph" and "Practice / used internally", which are concrete. The Theory cell should also point to a thing, not a slogan. | "Theory / organizational patterns" (and link to the existing theory page) — names a real artifact instead of a frame. |

Severity: hero > mission lead > built lead > repo-stats theory cell.
The hero is the highest-impact fix because it is the first thing every
visitor reads.

## 3. Sections that read clean (do not touch)

- Mission body paragraphs 1 and 2 (lines 1147-1161). Concrete framing of
  the durable problem; concrete description of what WorkGraph is.
- All three founder cards (lines 1186-1231). Per task instructions and
  per the bar: each names real work and real artifacts.
- "Incorporated a company" card (lines 1255-1272). Action verb, concrete
  outcome, link to the actual trace.
- "Co-authored grant applications" card (lines 1275-1290). Same shape.
- "PHR enrichment trace" card (lines 1293-1314). Technical but concrete;
  the audience for this page knows what hypergeometric enrichment is.
- CTA section (lines 1320-1369). Names three real use cases ("AI/ML
  study, distributed research effort, multi-agent software project")
  and links to docs/source/theory.
- Nav, footer, public-benefit CSS (unused in body, harmless leftover).

## 4. Missing-link recommendation

The published incorporation trace
(`https://ulivo.poietic.life/wg/feeds/incorporation-trace/index.html`)
is **already linked once** from Card 01 in section 03 (line 1270).
That is the right primary placement.

One optional secondary placement: the **hero meta strip** (line 1093)
currently lists only the `workgraph-itself` feed. Make it "live
workgraph ↗ · incorporation trace ↗ · grant graph ↗" so all three
Poietic feeds are reachable above the fold. Skip threading any trace
link into the mission paragraphs; that risks reintroducing
self-reference into copy that currently reads clean.

## 5. Recommended deploy order

If multiple fixes land in one synthesis pass, ship in this order so
the page improves top-down with each commit:

1. **Hero subhead** rewrite. Highest read rate, biggest payoff.
2. **Mission lead** rewrite. Drops "semi-autonomous" so the term is
   not used twice unexplained.
3. **Built lead** rewrite. Drops "live demo surface" and "in public
   enough to be evaluated".
4. **Repo-stats Theory cell** edit (smallest change, lowest risk).
5. **Hero meta strip** link addition (incorporation trace, grant graph).

Each step is independent and reversible; do not bundle them. Erik's
calibration was about replacing meta-philosophy with concrete answers,
not about restyling.

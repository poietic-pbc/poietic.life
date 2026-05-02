# Website site audit: poietic.life (2026-05-01)

Auditor: agent-266 (continuing agent-252's audit; Erik's "live"-callout
flag added as must-fix).
Calibration: Erik flagged the mission paragraph 3 ("WorkGraph is the
instrument… proof surface for the theory of organizational patterns")
as too self-aware and uncanny. When the reader asks *can you run a team
on it?*, they should get YES + how, not a paragraph about proof surfaces.

Both the deployed file (`~/poietic.life/index.html`) and the over-the-wire
fetch from `https://poietic.life` were read. They match.

## 1. Headline verdict

The page is **mostly clean**, but the same rough pattern Erik flagged
appears in three more spots (hero subhead, mission lead, built-section
lead), and the word **"live"** is doing too much work above the fold
(Erik called this out directly, must-fix). The middle of the page
(mission body p1+p2, founder cards, all three built cards, CTA, footer)
reads clean by Erik's bar; do not touch.

## 2. Rough spots

| Anchor | Current text | Diagnosis | Proposed fix |
|---|---|---|---|
| **MUST-FIX**: hero CTA + meta strip (lines 1089, 1093) | Button: `Live demo`. Meta strip: `PBC product · live demos · theory · organizational practice · live WorkGraph ↗`. Plus `live proof surface` (1072) and nav `live graph ↗` (1047). | **Erik called this out.** Five "live" callouts above the fold (button, breadcrumb, breadcrumb-link, hero-sub adjective, nav link) read as trying-too-hard. One canonical "live" entry is enough. | Keep nav `live graph ↗` as the single canonical live-feed pointer. **Drop the `Live demo` button** (the embedded iframe is right there; nav already points at the feed). **Strip "live" from the meta strip**: rewrite as `PBC · open source · MIT · workgraph ↗`. Hero-sub "live proof surface" goes away with rough-spot #2. Other CTAs (`Open WorkGraph`, `Read the mission`, etc.) stay plain, no `live` modifier. |
| `.hero-sub` (1069-1074) | "Poietic is a semi-autonomous public-benefit organization where people and AI agents build tools, demos, and theory for legible collaboration. WorkGraph is our first instrument: a live proof surface where humans and agents coordinate tasks, handoffs, decisions, artifacts, and histories." | Same pattern as Erik's flagged paragraph, in the most-read slot. "Semi-autonomous", "live proof surface", "legible collaboration" are abstractions where concrete should be. | "Poietic PBC builds open-source tools so humans and AI agents can run real projects together: incorporation, grant writing, scientific analysis. Our first tool is WorkGraph: a task graph where people and agents share tasks, hand off work, and leave a record anyone can read back." |
| `.mission-lead` (1141-1145) | "Poietic is a semi-autonomous organization. Its purpose is to make human-machine collaboration legible. It builds open tools to support that mission." | Restates the hero in the same abstractions. "Semi-autonomous" is never defined on the page. | "Poietic builds open-source tools so people and AI agents can do real work together, with the work itself visible to anyone who wants to inspect it." (the operating mode is clear from the live graph in the hero) |
| `.built-lead` (1244-1250) | "WorkGraph is Poietic's first product and live demo surface. It is functional, MIT-licensed, and open-source, with dependency visualization, live feeds, claim/execute/complete workflows, agent handoffs, and inspectable histories. We use it to run incorporation, writing, grant drafting, and research coordination in public enough to be evaluated." | "Live demo surface" = same family as "proof surface". "in public enough to be evaluated" is awkward and meta. | "WorkGraph is Poietic's first product. MIT-licensed, written in Rust, with dependency visualization, agent handoffs, and inspectable histories. Three things we ran on it ourselves are below; each links to the actual graph." |
| `.repo-stats` cell 3 (1106-1108) | "Theory / legible collaboration" | Mild version of the pattern; pairs with concrete "Product / WorkGraph" and "Practice / used internally". | "Theory / organizational patterns" (link to existing theory page); names a real artifact, not a slogan. |

Severity: live-repetition (Erik must-fix) > hero subhead > mission lead
> built lead > repo-stats theory cell.

## 3. Sections that read clean (do not touch)

- Mission body p1 and p2 (1147-1161). "live demonstrations" (1154) is a
  feature noun, not a self-label; leave it.
- All three founder cards (1186-1231). M3 fix landed cleanly.
- All three built cards (1255-1314): action verbs, concrete outcomes,
  links to the actual graphs.
- CTA section (1320-1369). Names three real use cases and links to
  docs/source/theory. CTA buttons already plain (`Build from the docs`,
  `View source on GitHub`, `Read the theory`); no "live" modifier here.
- Nav, footer, hero h1.


### Card-count check (Erik 2026-05-01)

Three section-03 cards (Incorporated, Grant, PHR) cover three distinct
domains: legal/operational, written deliverable, technical research.
By Erik's bar, **none is redundant**, recommend keeping all three. Faint
caveat: Card 02 (grant) carries mild recursion ("we used WorkGraph to
apply for the grant that funds it"); defensible now that Card 01's
incorporation trace is publicly verifiable. If Erik wants to err clean,
Card 02 is the only drop candidate, but cutting it loses the
shared-writing demo. My read: keep all three. Founder section also passes the distinct-question bar, leave alone.

## 4. Missing-link recommendation

The published incorporation trace
(`https://ulivo.poietic.life/wg/feeds/incorporation-trace/index.html`)
is **already linked once** from Card 01 in section 03 (line 1270). That
is the right primary placement.

After the live-repetition fix, the hero meta strip will no longer link
the workgraph feed (nav still does). Do **not** add incorporation-trace
or grant-graph links into the hero meta strip; doing so would rebuild the
repetition Erik flagged in different vocabulary. Card-level links in
section 03 are sufficient.

## 5. Recommended deploy order

Independent, reversible commits, top-down:

1. **Live-repetition fix** (Erik must-fix). Drop `Live demo` button,
   strip "live" from meta strip. Smallest diff, highest priority.
2. **Hero subhead** rewrite. Removes "live proof surface" + "semi-autonomous".
3. **Mission lead** rewrite. Drops second "semi-autonomous".
4. **Built lead** rewrite. Drops "live demo surface" and "in public enough".
5. **Repo-stats Theory cell** edit (smallest, lowest risk).

Erik's calibration was about replacing meta-philosophy with concrete
answers and cutting redundant "live" callouts, not restyling.

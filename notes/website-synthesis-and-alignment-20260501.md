---
synth_id: website-synthesis-and-alignment
date: 2026-05-01
inputs: [voice-a-direct, voice-b-concrete, voice-c-understated, voice-d-firstperson, site-audit-20260501, v3-1-final-coherency-review, current index.html, workgraph_google_application_FINAL_v3_1.md]
verdict: deploy
---

# Website synthesis + grant alignment (2026-05-01)

## 1. Voice recommendation: Voice D + Voice B's concreteness

**Recommendation: Voice D (founder first-person) as the register, with
Voice B's named-uses folded in.** Erik's amendment ("We use it to run
incorporation, writing, grant drafting, and research coordination in
public enough to be evaluated. And even this website!") is verbatim
first-person plural with a playful tag. That sentence will not sit
naturally inside Voice A (operational third-person), Voice C
(understated third-person), or Voice B (third-person who-does-what); it
sits inside Voice D. Voice D also breaks the meta-philosophical voice
Erik diagnosed by replacing self-narration with people talking. Voice
B's named uses (Erik on PHRs, Luca on clinical genomics, Vaughn on
hybrid teams) are folded in for concreteness. (100 words)

## 2. Final replacement text

**Scope:** Replace **mission body paragraph 3 only** (current
`index.html` lines 1169-1178). Per the site audit, paragraphs 1 and 2
read clean and should not be touched. Other rough spots are handled in
section 3 below.

### Before (current lines 1169-1178)

```html
<p>
  WorkGraph is the instrument, not the whole institution. It gives
  Poietic a proof surface for the
  <a href="https://graphwork.github.io/theory/">theory of organizational patterns</a>:
  product, demos, research practice, and organizational design should all
  make human and machine collaboration
  <strong>legible and responsive to its participants</strong>. That public-benefit
  purpose is the operating constraint: the tools should expose the work,
  the handoffs, the failures, and the evidence trail.
</p>
```

### After (drop-in)

```html
<p>
  We use WorkGraph for our own work. Erik runs pseudo-homologous-region
  discovery across vertebrate pangenomes on it. Luca's lab uses it
  alongside <a href="https://github.com/pinellolab/chorus">Chorus</a>
  for genomic-AI orchestration. Vaughn uses the resulting traces as
  material for his research on hybrid teams. We run incorporation,
  writing, grant drafting, and research coordination through it in
  public enough to be evaluated. And even this website. Browse the
  <a href="https://ulivo.poietic.life/wg/feeds/incorporation-trace/">incorporation trace</a>
  or this
  <a href="https://ulivo.poietic.life/wg/feeds/poietic-life/">site's build trace</a>.
  The Delaware filing names one public-benefit purpose:
  <strong>to make human and machine collaboration legible and responsive
  to its participants</strong>. That is the operating constraint on every
  feature.
</p>
```

Word count: ~135 (up from ~95). Three things the new paragraph does:
swaps "instrument / proof surface / theory of organizational patterns"
abstractions for named uses, lands Erik's verbatim dogfooding line with
"And even this website" (kept as a sentence rather than an exclamation
to match the surrounding register), and demotes the PBC purpose from
centerpiece to operating constraint while preserving the bolded verbatim
phrase.

## 3. Site audit fixes consolidated

The "live"-callout must-fix is **already partially landed** in commit
`dfc0d05` ("Declutter hero links"): `Live demo` button gone, `live`
stripped from meta strip, nav `live graph ↗` preserved as the canonical
pointer. Remaining "live" tokens (hero-sub, built-lead) get cleared by
the rewrites below.

| Anchor | Priority | Action |
|---|---|---|
| Mission body p3 (1169-1178) | **must-fix** | Apply section 2 replacement. |
| `.hero-sub` (1077-1082) | **must-fix** | Apply audit-proposed rewrite. Removes "semi-autonomous", "live proof surface", "legible collaboration". |
| `.mission-lead` (1148-1152) | **must-fix** | Apply audit-proposed rewrite. Drops second "semi-autonomous". |
| `.built-lead` (1251-1257) | **must-fix** | Apply audit-proposed rewrite. Drops "live demo surface", "live feeds", and the awkward "in public enough to be evaluated" (now placed cleanly in mission p3). |
| `.repo-stats` Theory cell (1114) | nice-to-have | Change `legible collaboration` to `organizational patterns`. |
| Hero `Live demo` button + meta strip | done | Removed in `dfc0d05`. |
| Add traces to hero meta | **defer** | Audit recommends against; would rebuild repetition. |
| Section 03 card count | **defer** | Audit verifies all three cards distinct. |

HTML for the four audit fixes is taken verbatim from the audit's
"Proposed fix" column (`website-site-audit-20260501.md` section 2); not
duplicated here.

## 4. Grant ↔ website alignment

Compared the proposed website text (mission p3 above plus hero-sub +
mission-lead + built-lead + Theory-cell rewrites) against
`workgraph_google_application_FINAL_v3_1.md`.

| Item | v3.1 | Website | Aligned? |
|---|---|---|---|
| Dogfooding voice | §17a, §17c, §18b: "in daily use across founders' labs", "tool serves real workflows" | New p3: "We use WorkGraph for our own work. Erik runs PHRs..." | **Yes** |
| No "in production today" overclaim | §17a uses "in daily use" (H2 fix) | "in active use" (built-lead), "we use it" (mission p3). No "production today" | **Yes** |
| No proposal-recursion claim | 0 instances per coherency review | Cites incorporation/site-build traces only, not "wrote the grant with WG" | **Yes** |
| Founder order (Erik/Luca/Vaughn, no PI) | Preserved across all sections; 0 PI tokens | New p3 lists Erik → Luca → Vaughn. No "PI" | **Yes** |
| WorkGraph description (MIT, Rust, persistent task graph) | §17a/§17b: "open-source infrastructure (MIT, Rust)... git-native persistent task DAG" | Mission p2 (unchanged) matches verbatim concepts | **Yes** |
| Adoption claims | §19a 10+ labs by m18 / 50+ by m36 (target) | Website claims founder-lab use only. No external adoption claim | **Yes** |
| Incorporation-trace evidence | Not cited in v3.1 (software adoption is the metric) | Cited as dogfooding evidence (compatible, no contradiction) | **Yes** |
| PBC purpose phrasing | §26 verbatim "legible and responsive to its participants" | New p3 preserves bolded phrase verbatim | **Yes** |
| CRISPRme / Casgevy framing | §17c/§36: "independently identified... informing FDA review" | Luca founder card matches; slightly more cautious wording | **Yes** |
| DNA-Diffusion containment | v3.1 §30 disclosure only | Website silent on DNA-Diffusion | **Yes** |
| Liverpool Hive Mind | v3.1 §28 acknowledges | Website silent (out of scope for landing) | **Yes** |

**No drift.** All proposed website edits stay coherent with v3.1. No
v3.1 changes needed.

## 5. Deploy plan

**Repo:** `poietic-pbc/poietic.life` (separate from this `wg` worktree).
All edits in `~/poietic.life/index.html`.

### Pre-deploy verification
1. Confirm `https://ulivo.poietic.life/wg/feeds/poietic-life/` resolves
   200 (currently 404 as of 2026-05-01 03:01 UTC; Erik flagged it as
   publishing). If still 404 at deploy time, drop the second link in
   mission p3 and keep only the incorporation-trace link. The sentence
   reads cleanly with one link.
2. Confirm `https://ulivo.poietic.life/wg/feeds/incorporation-trace/`
   resolves 200 (verified 2026-05-01).

### Edit sequence (independent reversible commits, top-down)

1. **Hero subhead** (lines 1077-1082). Apply audit-proposed rewrite.
   Removes last "live proof surface" + "semi-autonomous" in
   above-the-fold copy.
2. **Mission lead** (lines 1148-1152). Apply audit-proposed rewrite.
   Drops second "semi-autonomous".
3. **Mission body p3** (lines 1169-1178). Apply section 2 replacement
   above. Erik's amendment lands here.
4. **Built lead** (lines 1251-1257). Apply audit-proposed rewrite.
   Removes "live demo surface" + "in public enough to be evaluated".
5. **Theory cell** (line 1114). Change `legible collaboration` to
   `organizational patterns`.

### Commit messages

```
git add index.html
git commit -m "rewrite hero subhead: concrete uses replace 'live proof surface' (website-synthesis-grant)"
git commit -m "rewrite mission lead: drop 'semi-autonomous' (website-synthesis-grant)"
git commit -m "rewrite mission body p3: dogfooding voice + 'and even this website' (website-synthesis-grant)"
git commit -m "rewrite built lead: drop 'live demo surface' + awkward 'in public enough' (website-synthesis-grant)"
git commit -m "Theory cell: 'organizational patterns' names a real artifact (website-synthesis-grant)"
git push
```

(Stage by hunk if doing one commit per fix. Single squashed commit also
acceptable.)

### Post-deploy verification

1. `curl -s https://poietic.life | grep -c "live"` → expect ~1 (nav
   `live graph ↗` only).
2. `curl -s https://poietic.life | grep -c "semi-autonomous"` → expect 0.
3. `curl -s https://poietic.life | grep -c "proof surface"` → expect 0.
4. Visual check: open https://poietic.life, read end-to-end, confirm no
   layout regressions. Mission p3 should now name people, not concepts.
5. Both trace links in mission p3 must resolve 200; click both.
6. Confirm bolded `legible and responsive to its participants` phrase
   still renders in mission p3 (PBC purpose preserved).

### Out of scope (do not do same-day)

- v3.1 edits: none required.
- Card 02 drop (audit's faint caveat about grant-card recursion): defer.
- Hero meta strip trace links: defer per audit.
- New section 03 cards: defer.

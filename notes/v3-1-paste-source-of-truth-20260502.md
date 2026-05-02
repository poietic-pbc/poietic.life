---
note_id: v3-1-paste-source-of-truth
date: 2026-05-02
target: workgraph_google_application_FINAL_v3_1.md (commits fe760fb + e8e8fa8 on main)
verdict: paste-ready
---

# v3.1 paste source of truth (2026-05-02)

v3.1 on main now contains every paste-blocking fix from the form-mapping
paste guide and the vaughn-agency edits, consolidated into a single
commit (`fe760fb`). All word caps verified, style sweep clean. **Paste
from v3.1 only — `v3-1-form-mapping-paste-guide-20260502.md` and
`vaughn-agency-edits-applied-20260502.md` are now redundant for paste
purposes** (still useful as decision log).

## Fixes applied

| Section | Before | After | Final wc |
|---|---|---|---|
| §5b | `[leave blank]` literal | empty (line blank) | n/a |
| §8d Erik tz | `US Eastern (ET)` | `US Central (CT)` | n/a |
| §9d Luca tz | `US Eastern (ET)` | unchanged (Luca at MGH/Boston) | n/a |
| §15 stage | `Proof of Concept / Preliminary Results` | unchanged (Erik correction: paste guide's promotion to Validated Methodology was wrong; PoC is the honest answer given §29 risks and §43-§46 milestones build validation over 36 months) | n/a |
| §17c Tan line | "research on hybrid teams... methodological frame" | "drives WorkGraph's agency framework, the subsystem developing agent primitives" | 74 / 75 |
| §26 Erik citations | `~72,000 Google Scholar citations` | `~72,000 citations` | — |
| §26 Erik NSF | `leads the NSF PPoSS LARGE award ($5M) for computational pangenomics` | `leads NSF PPoSS LARGE ($5M) for pangenomics` | — |
| §26 Vaughn add | `...Singapore Centre for Strategic Futures.` | `...; designed WorkGraph's agency framework that develops agent primitives.` | 150 / 150 |
| §29 (was Theory of change) | 200w Theory of change content | 184w Risks block from paste guide | 184 / 200 |
| §30 (was Risks 100w) | Five-risk paragraph | 97w Key team members (roles only, no names) from paste guide w/ vaughn-edit 4th role | 97 / 100 |
| §49 govt officials | `No` | `Yes` | n/a |
| §50 govt entities | `No` | `Yes` | n/a |
| §53 explanation | `N/A` | 75w explanation (UTHSC + UCL public universities; project funds to Poietic PBC only) | 75 |

Theory of change content (formerly v3.1 §29) was dropped: no slot in the
form. Source: `git show 986222f:workgraph_google_application_FINAL_v3_1.md`
preserves it in history if reviewer reference is ever needed.

## Style sweep

- 0 em-dashes (`—`); en-dashes (`–`) only in pre-existing date ranges (Months 1–6, etc.)
- 0 PI / lead PI / Principal Investigator language
- Founder order Erik / Luca / Vaughn preserved
- No v1 terms (KRAS, MRTX1133, Boltz, RFdiffusion, DiffDock)
- No recursion claim ("drafted using WorkGraph", etc.)
- CRISPRme / Casgevy framing precise (independent identification of off-target before FDA approval; no implication of direct collaboration)

## Commits

`fe760fb consolidate paste-blocking fixes into v3.1` — applied 8 of the 9
intended fixes plus initially also promoted §15 to Validated Methodology
(later reverted, see next commit).

`e8e8fa8 revert §15 stage to 'Proof of Concept / Preliminary Results'
per Erik` — Erik flagged that the paste-guide's §15 promotion was wrong:
form definition of Validated Methodology applies to components (vg,
PGGB, CRISPRme), not to the proposed longitudinal hybrid coordination
work that this grant funds validating. PoC is the honest answer.

Both commits pushed to `origin/main`
(`git@github.com:poietic-pbc/google_ai_competition.git`). New commits on
top of `986222f`; nothing amended.

## Paste guidance for Erik

**Paste from `workgraph_google_application_FINAL_v3_1.md` only**. Every
form question §1-§53 has its content correct in place. The two notes
below remain useful as decision logs but should not be opened during
paste:

- `v3-1-form-mapping-paste-guide-20260502.md` — full form-mapping table,
  Erik-only items, optional content choices for §28 / §31 / §32 / §36
  (the v3.1 versions are defensible defaults; the paste guide's
  alternatives are improvements Erik may opt into per his preference).
- `vaughn-agency-edits-applied-20260502.md` — superseded by this
  consolidation; v3.1 already contains the §17c / §26 edits.

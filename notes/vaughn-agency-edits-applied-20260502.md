---
note_id: vaughn-agency-edits-applied
date: 2026-05-02
task: vaughn-agency-edit (agent-282)
status: applied + pushed
---

# Vaughn agency edits applied (2026-05-02)

Erik flagged that v3.1 + paste guide + landing page were undersell­ing
Vaughn Tan as co-architect of WorkGraph's agency subsystem (the layer
that develops, evaluates, and dispatches agent primitives like
"Default Evaluator", "Careful Programmer", visible in coordinator
logs as `Lightweight assignment: agent=...`). Surgical edits applied
in place, ≤20 min wall-clock.

## Files edited

1. `workgraph_google_application_FINAL_v3_1.md` (agent-282 worktree, commit `0380be8` on `wg/agent-282/vaughn-agency-edit`; merge-back automatic)
2. `~/poietic.life/notes/v3-1-form-mapping-paste-guide-20260502.md` (commit `434eaee` on poietic.life main, pushed)
3. `~/poietic.life/index.html` (commit `98b3fd8` on poietic.life main, pushed live)

Edit #5 (v3.1 §43-§46 milestones) skipped: no milestone naturally
accommodates "agency framework v2" without scope creep, and the four
existing edits already reframe Vaughn cleanly across the three
public-facing surfaces.

## Diff hunks (terse)

### v3.1 §17c (line 107)
**Before:** `Tan's research on hybrid teams under uncertainty (ASQ; Columbia University Press) provides the methodological frame.`
**After:**  `Tan's hybrid-teams-under-uncertainty research (ASQ 2015; Columbia 2020) drives WorkGraph's agency framework, the subsystem developing agent primitives.`
Reframes Tan from "methodological frame provider" to active driver of a named WorkGraph subsystem.

### v3.1 §26 (line 194)
**Erik trim (5 words):**
- `with ~72,000 Google Scholar citations across the toolkit` → `with ~72,000 citations across the toolkit`
- `leads the NSF PPoSS LARGE award ($5M) for computational pangenomics` → `leads NSF PPoSS LARGE ($5M) for pangenomics`

**Vaughn add (8 words, before final period):**
- `...Singapore Centre for Strategic Futures.` → `...Singapore Centre for Strategic Futures; designed WorkGraph's agency framework that develops agent primitives.`

### Paste guide §30 4th role
**Before:** `Fourth, an organizational researcher conducting longitudinal ethnographic case studies of hybrid human-AI lab teams (part-time, drawn from founder bandwidth).`
**After:**  `Fourth, an organizational researcher: designs the agency framework that develops agent primitives and matches work to agent capabilities, drawing on hybrid-teams-under-uncertainty research; conducts longitudinal ethnographic case studies of adopter labs (part-time).`

### Website Vaughn founder card
**Before:** `Tan writes about AI agents, reasoning scaffolds, public strategy, and not-knowing; that work informs WorkGraph's approach to keeping human judgment explicit in hybrid human-AI research coordination.`
**After:**  `Tan designed WorkGraph's agency framework, the subsystem that develops agent primitives and matches work to agent capabilities, applying his research on hybrid teams, reasoning scaffolds, and not-knowing.` (vaughntan.org link preserved on "his research")

## Final word counts (verified by `len(s.split())`)

| Section | Cap | Before | After |
|---|---|---|---|
| v3.1 §17c | 75 | 73 | **74** |
| v3.1 §26 | 150 | 147 | **150** |
| paste guide §30 block | 100 | 85 | **97** |
| website Vaughn card | n/a | 49 | **44** |

## Live URL

https://poietic.life — Vaughn founder card now reads "Tan designed WorkGraph's agency framework..." (deploy via GitHub Pages from `poietic-pbc/poietic.life` main; commit `98b3fd8`).

## What Erik should re-paste

Erik is at the form actively. Two re-paste actions:

1. **Form §17c (Evidence solution works, 75w):** RE-PASTE from the
   updated v3.1 §17c (worktree `agent-282`, commit `0380be8`). The
   change is the final two sentences before the github URL.

2. **Form §26 (Why uniquely positioned, 150w):** RE-PASTE from the
   updated v3.1 §26. Erik's vg/PGGB line trimmed by 5 words and
   Vaughn's line gained 8 words; net at cap.

3. **Form §30 (Key team members, 100w):** RE-PASTE from the updated
   paste guide §4 §30 block (97w). 4th role rewritten.

The v3.1 worktree commit will merge back to main automatically per
the wg pipeline; Erik can paste from either the worktree file or
wait for merge to `main` if he wants to read from `986222f`'s
successor commit. Both contain identical content.

## Style sweep on touched text

- [x] No em-dashes introduced (verified: 0 em-dashes in v3.1 file; new content in paste guide and index.html contains no em-dashes)
- [x] No "PI" or "lead PI" language
- [x] No v1 terms (KRAS, MRTX1133, Boltz, RFdiffusion, DiffDock)
- [x] Founder order Erik / Luca / Vaughn preserved in §26
- [x] No recursion claim ("drafted using WorkGraph") added
- [x] CRISPRme/Casgevy framing untouched (precise version preserved in §17c, §26)
- [x] Vaughn's COI-relevant framing not touched (DNA-Diffusion still only in §29 risk disclosure)

## Validation

- [x] v3.1 §17c and §26 edited in place; word caps respected (74/75, 150/150)
- [x] Paste guide §30 draft edited in place (97/100)
- [x] Website index.html Vaughn card edited and pushed live (commit 98b3fd8)
- [x] Each touched section's final word count documented
- [x] No em-dashes introduced
- [x] Output note at this path

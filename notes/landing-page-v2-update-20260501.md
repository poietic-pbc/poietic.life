# Landing page v2 update — 2026-05-01

Context: grant submission day, public benefit statement and v2 hygiene fixes
landed before reviewers could click through. Task ID: `landing-page-v2`.

## 1. PBC benefit statement: where I found it

**File path (canonical):**
`~/poietic/corporate/signed/amendments/01_Certificate_of_Amendment.pdf.txt`

This is the OCR/text extraction of the PDF as filed with the Delaware Division
of Corporations on **April 13, 2026** (state receipt
`SR20261750696.pdf` in the same folder).

The matching unsigned source PDF lives at
`~/poietic/corporate/formation/certificate-of-amendment-equity-structure.pdf.txt`,
but the `signed/amendments/01_*` version is the one filed and stamped by the
state and is what I treated as authoritative. The two differ slightly in
wording: I used the filed/signed version.

(For reference, `~/poietic/corporate/formation/certificate-of-incorporation.pdf.txt`
is the original March 23 incorporation as a regular Delaware C-corp ("Poietic, Inc.").
The April 13 amendment is what converted it to a PBC and added the public benefit
purpose. So the original certificate is NOT the right source for the benefit
statement.)

## 2. Exact text used (verbatim, please sanity-check)

### Generic PBC framing (Article amending the purpose, sentence 2)

> The Corporation shall be a public benefit corporation as contemplated by
> subchapter XV of the General Corporation Law (the "DGCL"), or any successor
> provisions. It is intended that the Corporation operate in a responsible
> and sustainable manner and produce a public benefit, and is to be managed
> in a manner that balances the stockholders' pecuniary interests, the best
> interests of those materially affected by the Corporation's conduct, and
> the public benefit identified in this certificate of incorporation.

### Specific public benefit purpose (Article amending the purpose, sentence 3)

> The specific public benefit purpose of the Corporation is to make human
> and machine collaboration legible and responsive to its participants.

Both blocks are quoted verbatim. The HTML uses `&ldquo;`, `&rdquo;`, and
`&rsquo;` for the curly quotes/apostrophes that appeared in the filed text.

Source attribution rendered on the page:
> Verbatim from the Certificate of Amendment to the Certificate of
> Incorporation of Poietic PBC, filed with the Delaware Division of
> Corporations on April 13, 2026.

If you want a tighter or more formal attribution, edit the
`<div class="benefit-source">` block. I optimized for "a reviewer who clicks
through can immediately see this is real and look up the filing themselves."

## 3. Card #3 before / after

### Before (deployed file, as of this morning)

> **Pangenome methodology comparison**
>
> Three ways to do the same genomics task, side by side: WorkGraph with a
> domain expert in the loop, a single-session agentic CLI, and a solo
> bioinformatician. Full process published.
>
> _coming soon_

(Note: card #3 had ALREADY been partially de-v1'd from the original drug
discovery / Boltz / RFdiffusion / DiffDock language; it was generic
"genomics task" rather than KRAS-specific. The CLAUDE.md flag on it was
ahead of the deployed reality. The drug-discovery v1 string actually
remaining was in the CTA paragraph, line 1216, which I also fixed.)

### After

> **PHR methodology comparison**
>
> A three-way comparison on pseudo-homologous region (PHR) discovery in a
> defined pangenome interval: WorkGraph with Erik in the loop alongside
> specialist agents, a single-session agentic CLI running autonomously,
> and a solo skilled bioinformatician using vg / PGGB. Each arm produces
> a candidate set; the WorkGraph arm produces an inspectable computation
> graph alongside it.
>
> writeup → coming soon
>
> _in progress_

The card now has `id="phr-demo"` so the CTA paragraph and any future
writeup link can target it (`href="#phr-demo"`). The "writeup" link is
currently a placeholder (anchors back to itself); swap in the preprint /
graph URL when ready.

## 4. Other v2-hygiene findings (out of scope for this task, but noted)

These were noticed while scanning the landing page; flagging for follow-up:

1. **Repo stats are out of date.** Hero shows "2,091 commits · 263,112
   source lines · 83,196 test lines." Worth a periodic refresh or a tiny
   build script that fills these from `git rev-list --count HEAD` etc.
   The deployed file and the worktree copy disagree: deployed says
   "2,091 commits", worktree says "93+ commits" in one spot. Pick one
   source of truth.

2. **Two index.html files diverging.** Deployed at `~/poietic.life/index.html`,
   in-development at `~/google_ai_competition/.wg-worktrees/agent-32/index.html`.
   The latter has nicer features (repo-stats grid, terminal viz inset, "Open
   WorkGraph" CTA button) that haven't shipped. Worth a session to either
   merge worktree -> deployed in one go or pick one as canonical and delete
   the other. I applied this task's content changes to BOTH so they don't
   drift further on these specific items.

3. **Mission body still says "design molecules."** Holdover from when the
   demo was drug discovery. Still defensible (PHR work doesn't preclude
   molecule design), but if you want the mission to align with the
   PHR/clinical genomics spine you might soften that example.

4. **Footer says only "Poietic PBC · Public Benefit Corporation · United
   States" with no contact / privacy / press links.** Probably fine for
   today, worth a pass before any real PR push.

5. **Em-dashes (now removed from rendered text)** were used in seven
   places. I converted them all (`·`, `,`, `.`). The CSS comments still
   contain `─` (Unicode box-drawing horizontal) describing the logo and
   `—` in CSS comments; those don't render so I left them. If you want
   strict zero-em-dash including comments, search-and-destroy in
   `<style>` and SVG annotation comments.

6. **The "Co-authored grant applications" card #2** is technically v1
   language too — it was the v1 application. The v2 application is also
   coordinated through the WorkGraph (per CLAUDE.md), so the card is
   still accurate; but the "shipped" badge will read awkwardly today
   when v2 is being submitted live. Maybe re-badge to "ongoing" after
   today's submission.

7. **Nav status pill says "pbc · open source"** — fine, but consider
   linking it to the new `#public-benefit` section now that the page has
   one.

## 5. Deployment

Deployed file edited at `~/poietic.life/index.html`. Will commit + push to
`poietic-pbc/poietic.life` main, which is GitHub-Pages-deployed via the
`CNAME` (poietic.life) at the same path. Once pushed, the live site updates
within a couple minutes.

The worktree copy was also updated for parity; that commit goes to
`wg/agent-32/landing-page-v2` in the `google_ai_competition` repo via the
workgraph workflow, not to production.

## 6. Files touched

- `~/poietic.life/index.html` — production deployed file (this is what reviewers see)
- `~/google_ai_competition/.wg-worktrees/agent-32/index.html` — worktree mirror, kept in sync
- `~/poietic.life/notes/landing-page-v2-update-20260501.md` — this note

## 7. Reviewer dry-run

Open `~/poietic.life/index.html` in a browser. Section navigation should now read:

```
01/05  mission
02/05  public benefit   <-- new
03/05  what we've built (card #3 = PHR)
04/05  founders          (Erik / Luca / Vaughn order preserved)
05/05  get involved      (CTA points to #phr-demo)
```

Sanity checks I ran:
- `grep -E 'drug|KRAS|cancer|MRTX|Boltz|RFdiffusion|DiffDock'` -> 0 matches in both files
- `grep '—'` -> 0 matches in rendered text in both files
- HTML parses cleanly under `html.parser` (no malformed tags)
- Verbatim benefit statement string present exactly once in each file

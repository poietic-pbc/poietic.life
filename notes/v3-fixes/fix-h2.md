---
fix_id: fix-h2
target_section: 17a
word_cap: 75
status: ready-for-assembler
source_commit: 70c8e7f
---

# fix-h2 — §17a: "in production today" tone fix

## Criticism (verbatim from v3-review-synthesis-20260501.md, row H2)

> §17a says "in production today" which reads as overclaim against §28's "daily use across founder labs". Tone inconsistency between sections.
>
> **Action:** Replace "in production today" with "in daily use across the founders' labs".

## Target section + word cap

- **Section:** 17a ("The solution we are proposing is...")
- **Word cap:** 75 words

## Current text (verbatim from v3, commit 70c8e7f)

> Poietic PBC builds WorkGraph: open-source infrastructure (MIT, Rust, in production today) where humans and AI agents act as peers in a persistent task graph that is auditable across sessions, operators, and machines. WorkGraph is agent-agnostic, integrating Claude, Gemini, AlphaGenome (via Pinello's Chorus), GPT, and open-weight models. The grant matures the infrastructure and demonstrates it longitudinally inside the founders' active computational and clinical genomics programs, including the reference-resource construction work that underpins downstream science.

## Proposed text

> Poietic PBC builds WorkGraph: open-source infrastructure (MIT, Rust, in daily use across the founders' labs) where humans and AI agents act as peers in a persistent task graph that is auditable across sessions, operators, and machines. WorkGraph is agent-agnostic, integrating Claude, Gemini, AlphaGenome (via Pinello's Chorus), GPT, and open-weight models. The grant matures the infrastructure and demonstrates it longitudinally inside founders' computational and clinical genomics programs, including reference-resource construction work that underpins downstream science.

## Word count check

| Stage | Words | Cap | Headroom |
|---|---|---|---|
| Before (v3 current) | 73 | 75 | +2 |
| After (this fix) | 74 | 75 | +1 |

Diff accounting:
- Replaced "in production today" (3 words) with "in daily use across the founders' labs" (7 words): **+4**
- Trimmed "the founders' active computational and clinical genomics programs" → "founders' computational and clinical genomics programs": **-2** (drop "the", drop "active")
- Trimmed "including the reference-resource construction work" → "including reference-resource construction work": **-1** (drop "the")
- Net: **+1** word (73 → 74), still under the 75-word cap.

(Manual recount of the proposed text confirms 74 words.)

## Rationale

The criticism is a tone-consistency fix: §28 elsewhere says "daily use across founder labs", and §17a's bolder "in production today" reads as an overclaim against that more precise phrasing. The fix substitutes the §28 framing verbatim (with the explicit possessive "the founders' labs", per the synthesis directive), so a reviewer reading the application end-to-end finds one consistent self-description of the deployment status rather than two competing claims. The substitution adds four words, which would push the section over its 75-word cap; I recover two of those by dropping a redundant "the" and the soft adjective "active" from the later "founders' active computational and clinical genomics programs" clause (the second mention of founders no longer needs the article since the parenthetical already established them), and one more by dropping the article from "the reference-resource construction work". None of those trims removes substantive content. No em-dashes; no PI language; no v1/KRAS terms; no recursion claim; CRISPRme/DNA-Diffusion framing untouched (not present in §17a). Founder ordering not at issue in this section (only Pinello is named, in attribution of Chorus).

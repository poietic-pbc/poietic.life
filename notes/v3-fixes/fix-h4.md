---
fix_id: H4
target_section: 31
target_word_cap: 100
status: ready-for-assembly
source_task: fix-h4-31-clinical
source_review: notes/v3-review-synthesis-20260501.md
recommendation: option-a-drop
---

# fix-h4: §31 clinical programs — name 1-2 or drop

## Criticism

Verbatim from `notes/v3-review-synthesis-20260501.md` §3 (must-fix table, row H4):

> | H4 | §31 | "Initial conversations are underway with clinical genomics programs" reads as boilerplate | Either name 1–2 programs or drop the sentence |

Reinforced verbatim in the underlying skeptical review (`notes/v3-review-skeptical-20260501.md` line 20):

> §31: "Initial conversations are underway with clinical genomics programs." Boilerplate. Name them or drop it.

The domain-expert review (`notes/v3-review-domain-expert-20260501.md` lines 85-87) does NOT object to §31 staying clean of named partners and explicitly endorses keeping the partner fields blank:

> One named external pangenomics collaborator. §31 keeps partner fields blank; that's fine for the form but a domain reviewer would want at least one HPRC or VGP figure named in §26.

This is important: the domain expert pushes named-collaborator content toward §26, not §31. That converges with the "drop" branch of the H4 alternatives.

## Target section + word cap

- **Section:** 31 (Partner organizations)
- **Word cap:** §31 is not listed in CLAUDE.md's explicit cap table; it is an open-text supplement to a structured form field with the explicit instruction "[If the form requires individual partner entries: leave individual partner fields blank and use this paragraph in any open notes field. Do not list employer institutions as partner organizations.]" Treat 100 words as the working cap (matches neighboring §30, §35) since the current v3 text is 96 words and any rewrite should not balloon past that.

## Current text (verbatim from v3 at 70c8e7f, lines 229-231)

> Poietic PBC is the sole applicant and sole grantee. Co-founders maintain separate academic appointments at UTHSC, Massachusetts General Hospital / Harvard Medical School, and University College London respectively. The proposal is structured to operate independently of those institutions: no institutional IP, indirect costs, or shared resources are entangled in this application. Initial conversations are underway with clinical genomics programs interested in adopter-lab collaboration on auditable hybrid workflows; partnerships will be formalized post-award. Pilot lab partners for WorkGraph adoption will be recruited in Year 1 from the founders' networks across the genomics, pangenomics, and computational biology communities.
>
> [If the form requires individual partner entries: leave individual partner fields blank and use this paragraph in any open notes field. Do not list employer institutions as partner organizations.]

The flagged sentence is the fourth sentence:

> Initial conversations are underway with clinical genomics programs interested in adopter-lab collaboration on auditable hybrid workflows; partnerships will be formalized post-award.

(21 words.)

## Proposed text

Two options are produced as the task requires; **the assembler should apply Option A**.

### Option A (RECOMMENDED) — drop the sentence entirely

> Poietic PBC is the sole applicant and sole grantee. Co-founders maintain separate academic appointments at UTHSC, Massachusetts General Hospital / Harvard Medical School, and University College London respectively. The proposal is structured to operate independently of those institutions: no institutional IP, indirect costs, or shared resources are entangled in this application. Pilot lab partners for WorkGraph adoption will be recruited in Year 1 from the founders' networks across the genomics, pangenomics, and computational biology communities.
>
> [If the form requires individual partner entries: leave individual partner fields blank and use this paragraph in any open notes field. Do not list employer institutions as partner organizations.]

### Option B (NOT RECOMMENDED) — replace with the most defensible specific framing

This option swaps the boilerplate sentence for one that names already-existing consortium relationships rather than imagined "clinical genomics programs." It is honest, but answers a question the criticism did not ask (it names pangenomics/functional-genomics consortia, not clinical-genomics programs), and it overlaps with §26 where the domain-expert review wants HPRC/VGP specificity to live.

> Poietic PBC is the sole applicant and sole grantee. Co-founders maintain separate academic appointments at UTHSC, Massachusetts General Hospital / Harvard Medical School, and University College London respectively. The proposal is structured to operate independently of those institutions: no institutional IP, indirect costs, or shared resources are entangled in this application. Concrete adopter-lab leads draw on the founders' active consortium relationships, including the Human Pangenome Reference Consortium and the NHGRI IGVF Consortium where Pinello leads a characterization center. Pilot lab partners for WorkGraph adoption will be recruited in Year 1 from the founders' networks across the genomics, pangenomics, and computational biology communities.
>
> [If the form requires individual partner entries: leave individual partner fields blank and use this paragraph in any open notes field. Do not list employer institutions as partner organizations.]

## Diff (minimal, for the recommended Option A)

```
- The proposal is structured to operate independently of those institutions: no institutional IP, indirect costs, or shared resources are entangled in this application. Initial conversations are underway with clinical genomics programs interested in adopter-lab collaboration on auditable hybrid workflows; partnerships will be formalized post-award. Pilot lab partners for WorkGraph adoption will be recruited in Year 1 from the founders' networks across the genomics, pangenomics, and computational biology communities.
+ The proposal is structured to operate independently of those institutions: no institutional IP, indirect costs, or shared resources are entangled in this application. Pilot lab partners for WorkGraph adoption will be recruited in Year 1 from the founders' networks across the genomics, pangenomics, and computational biology communities.
```

The bracket note ("[If the form requires individual partner entries...]") is unchanged.

## Word count check

| Version | Words | Cap | Margin |
|---|---|---|---|
| Current (v3) | 96 | 100 (working) | +4 |
| Option A (recommended) | 75 | 100 (working) | +25 |
| Option B | 102 | 100 (working) | -2 (over) |

Counts produced by `wc -w` on the body paragraph only (the bracket note is form instruction, not prose, and is excluded — same convention used by fix-m1 and the v3 word-count audit). Option B is over the working cap by two words and would require a separate trim if the assembler chose it; this is one more reason to apply Option A.

## Constraint compliance check (Option A)

- Word cap respected (75 ≤ 100 working cap, well inside margin). ✓
- No em-dashes introduced. ✓ (none in the surviving text; the dropped sentence had none either).
- No PI / lead-PI language. ✓
- No v1 terms (KRAS, MRTX1133, Boltz, RFdiffusion, DiffDock, pancreatic cancer). ✓
- No recursion claim ("drafted using WorkGraph", "incorporated using WorkGraph"). ✓
- CRISPRme / Casgevy framing precise: not relevant to §31; unchanged elsewhere. ✓
- DNA-Diffusion not mentioned in §31. ✓
- Founder order: §31 lists employer institutions in the order UTHSC (Garrison) / MGH-HMS (Pinello) / UCL (Tan), which preserves Erik / Luca / Vaughn ordering. Unchanged by the fix. ✓
- "Do not list employer institutions as partner organizations" instruction in the bracket note is preserved verbatim. ✓
- The sentence "Pilot lab partners for WorkGraph adoption will be recruited in Year 1 from the founders' networks" is retained, so the section still answers the form's intent (how partners will be acquired) without making an unverifiable claim about ongoing conversations. ✓

## Rationale

The H4 criticism is that the sentence makes a claim ("conversations are underway") with no verifiable referent. A skeptical reviewer treats unverifiable claims as either careless or strategic, and either reading is worse than no claim at all. The criticism gives two branches: name 1-2 programs, or drop the sentence. Both branches lower risk relative to the status quo; the question is which branch is honestly available.

Naming requires a real, namable clinical-genomics adopter program with at least an informal commitment. The team does not have one to name as of submission day. Pinello's clinical work runs inside MGH/HMS/Broad, which the bracket note explicitly forbids listing as a partner organization. The IGVF Consortium and HPRC are real consortium relationships, but IGVF is functional genomics and HPRC is a reference-resource consortium, not clinical genomics — so naming them does not actually neutralize the "clinical genomics programs" framing the criticism flagged; it changes the subject. The domain-expert review (lines 85-87) independently routes named-collaborator specificity to §26, not §31, and explicitly says §31 staying blank is fine. The CLAUDE.md style guide adds a third constraint: "Never use em-dashes" and "Keep language direct and concrete. Avoid academic fluff" both cut against keeping a vague-future-tense sentence whose only function is reassurance.

That converges on Option A. The remaining text in §31 still does the work the section needs: it states the legal structure (sole applicant, sole grantee), acknowledges the three home institutions without entangling them, declares no institutional IP or indirect costs, and commits to recruiting pilot partners from the founders' networks in Year 1. Removing the boilerplate sentence makes the section shorter (75 words vs 96) and stronger: every remaining claim is verifiable from the form fields and public CVs, and the form's structured partner fields stay blank in line with the bracket note's explicit instruction.

Option B is included because the task spec required producing both options. It is honest in the narrow sense that HPRC and IGVF are real relationships, but it is the wrong fix for H4: it answers a different criticism (lack of named collaborators) than the one raised (boilerplate "clinical genomics programs"), it lands at 102 words against a 100-word working cap, and it duplicates content the domain-expert review wants in §26. The assembler should reject Option B unless an explicit clinical-genomics-program name is added to the team's commitments before submission, in which case this spec should be re-opened with the new name substituted.

---
fix_id: fix-h7
target_section: 28 (and external repo)
word_cap: 100
status: ready-for-assembler
source_commit: 70c8e7f
flag: erik-only-action-required
---

# fix-h7: `phr-methodology-comparison` repo, drop "demonstration in motion" implication

## Criticism (verbatim from v3-review-synthesis-20260501.md, row H7)

> H7 | `phr-methodology-comparison` repo | 1 commit, region not selected as of submission day | Push at least one commit naming the region and species set OR remove "demonstration in motion" implications from §28

Cross-references in the same synthesis:
- §7 (web-link issues): "`github.com/poietic-pbc/phr-methodology-comparison`: 200 OK; 1 commit, region pending → H7."
- §8 (v2 vs v3 final, "Reviewer memorability (set piece)"): v3 explicitly *dropped* the three-arm methodology comparison set piece that v2 carried. The repo is a v2-era artifact whose visible state contradicts what v3 actually claims.

## Target section + word cap

- **Section:** 28 ("Technical feasibility")
- **Word cap:** 100 words
- **Coordination note:** fix-h3 also targets §28 and brings it to 99/100 words. There is no remaining word budget in §28 for an additional substitution. This spec therefore proposes **no §28 text change beyond fix-h3** and routes the actionable part to an Erik-only repo action (see "Erik-only action" below).

## Current text (verbatim from v3, commit 70c8e7f)

> 28. Technical feasibility (100 words)
>
> WorkGraph is functional and publicly available (github.com/graphwork/workgraph; MIT), supporting multi-agent coordination, automatic task spawning, dependency resolution, and lifecycle management. It is in daily use across founder labs. Pangenome construction (vg, PGGB, HPRC tooling) and Pinello's CRISPRme stack are mature, published, and proven at scale. Tan's reasoning-scaffold prototype was demoed in October 2025. Our design draws on prior agent prototypes (SciAgents, Virtual Lab) and workflow managers (Galaxy, Nextflow, Snakemake), filling a different slot. Liverpool's inaugural Hive Mind grant addresses hybrid coordination for wet-lab autonomous chemistry; we address the parallel pattern for computational and clinical genomics, complementary.

Adjacent v3 text the criticism could reach (audited so the assembler can confirm none of it needs to change):

- §17a (post-fix-h2): "MIT, Rust, in daily use across the founders' labs ... The grant matures the infrastructure and demonstrates it longitudinally inside founders' computational and clinical genomics programs...". This frames demonstration as **future** ("the grant matures and demonstrates"), not as a comparison currently underway. No change needed.
- §17c: "WorkGraph is in daily use coordinating Garrison's ongoing pangenomics research and other founder workflows." This describes WorkGraph use, not a methodology comparison. No change needed.
- §29 / §17d: "longitudinal deployment across the founders' active genomics programs", explicitly future-tense ("the grant funds"). No change needed.
- §28 itself: "It is in daily use across founder labs", endorsed verbatim by fix-h2 as the canonical phrasing for tone consistency. No change available without contradicting H2.

There is no v3 sentence that asserts the three-arm methodology comparison is currently in motion. v3 already dropped the v2 set piece. The contradiction the panel flagged is purely between the **public repo's existence** (with one stub commit and no region named) and the inference a reviewer makes after reading the v3 narrative plus checking the org page.

## Proposed text

**No change to v3 §28** (capacity exhausted by fix-h3).

The fix is **external to the application document** and is an Erik-only action on the GitHub repo `github.com/poietic-pbc/phr-methodology-comparison`. The application as fixed by fix-h3 already works regardless of which Erik-only option is chosen, because no §28 sentence asserts that the methodology comparison is in motion.

### Erik-only action (pick one before submission window closes)

Ranked by effort/effect, lowest-effort first:

1. **GitHub-archive the repo** (one click in repo Settings → "Archive this repository"). Adds the visible "Public archive" badge and removes the repo from the default `poietic-pbc` org page filter. This is the same remediation as M4 (`deep-research-competition`), so the two repo issues collapse to one consistent action: any v2-era public scaffold that has not been picked up under v3 gets archived. Recommended.

2. **Stub the README to a one-line pointer at the v3 longitudinal-deployment plan.** Replace the current README with: "Superseded by the v3 longitudinal-deployment plan; WorkGraph adoption is now measured by lab uptake across the founders' active genomics programs (see [poietic.life](https://poietic.life))." Push as a single commit. This option is appropriate if archiving feels too final and Erik wants to retain editorial control over the repo for a possible future revival.

3. **Push a commit naming the region and species set, plus a one-paragraph protocol stub.** Highest effort; only worth doing if Erik has actually selected the region/species set and is willing to commit to a pre-submission methodology comparison run. Per CLAUDE.md "Still to Lock Down" §11, this is *not* yet decided as of 2026-05-01, so this option requires a real prior decision Erik has not made on the timeline available. Not recommended under time pressure.

The criticism's text ("Push at least one commit naming the region and species set OR remove 'demonstration in motion' implications from §28") presents these as alternatives. Option 1 is the minimum viable fix; the §28 alternative is foreclosed by the H3 word-cap collision plus the absence of any "demonstration in motion" language to actually remove.

### Section text that works regardless

§28 as fixed by fix-h3 (verbatim from fix-h3.md):

> WorkGraph is functional and publicly available (github.com/graphwork/workgraph; MIT), supporting multi-agent coordination, automatic task spawning, dependency resolution, and lifecycle management. It is in daily use across founder labs. Pangenome construction (vg, PGGB, HPRC tooling) and Pinello's CRISPRme stack are mature, published, and proven at scale. Tan's reasoning-scaffold prototype was demoed in October 2025. Our design draws on prior agent prototypes (SciAgents, Virtual Lab) and workflow managers (Galaxy, Nextflow, Snakemake). Liverpool's inaugural Hive Mind grant addresses hybrid coordination for wet-lab autonomous chemistry. Liverpool optimizes for lab-robotics scheduling and physical-experiment coordination; WorkGraph optimizes for git-native provenance across distributed human and computational actors.

Reading this against any of the three Erik-only options above:
- Option 1 (archive): "in daily use across founder labs" remains true and now refers only to ongoing internal use, not to a comparison the panel can fact-check against an empty repo.
- Option 2 (README stub): same, plus the stubbed README signals to a curious reviewer that the v3 plan is the live one.
- Option 3 (commit with region named): same, plus the repo now substantiates an even stronger reading of "in daily use," which v3 does not require but would not contradict.

No additional v3 text edit is required for this fix to land.

## Word count check

| Stage | Words | Cap | Headroom |
|---|---|---|---|
| §28 before (v3 current) | 95 | 100 | +5 |
| §28 after fix-h3 alone | 99 | 100 | +1 |
| §28 after fix-h7 (this spec) | 99 | 100 | +1 |

This spec contributes **0 word delta to §28**. The §28 final state is fully determined by fix-h3.

(Manual recount of the assembler-target §28 text confirms 99 words.)

Constraint pass:
- No em-dashes in the spec or in the (unchanged) §28 text. ✓
- No PI language; "founders" and "co-founders" only. ✓
- No v1 terms (KRAS, MRTX1133, Boltz, RFdiffusion, DiffDock, pancreatic, drug-discovery, three-arm, methodology comparison demonstration). ✓
- No recursion claim ("drafted using WorkGraph", "incorporated using WorkGraph"). ✓
- CRISPRme/Casgevy framing: §28 references only "Pinello's CRISPRme stack ... mature, published, and proven at scale"; no Casgevy claim attached. ✓
- DNA-Diffusion: not invoked in §28 or in this spec. ✓
- Founder order: §28 names only Pinello and Tan via possessives, in the order they are introduced; not a contested ordering site. ✓

## Rationale

The criticism describes a contradiction between two surfaces a panel reviewer can read end-to-end: the v3 application narrative on one side, and the public `poietic-pbc` org page (and the stub `phr-methodology-comparison` repo it links to) on the other. The synthesis offered the panel two repair paths: substantiate the repo by pushing real content, or remove the application-side language that makes the repo's emptiness conspicuous. Auditing v3 against this criticism shows that the application-side language is already gone: v2's three-arm methodology-comparison set piece was deliberately cut in v3 (synthesis §8 explicitly notes this as a v2 → v3 trade-off), and what remains in §28 ("in daily use across founder labs") is the canonical phrasing fix-h2 uses for tone consistency across §17a and §28; weakening it would create a fresh inconsistency without resolving the underlying repo problem. Worse, fix-h3 already brings §28 to 99/100 words to install the architectural-divergence sentence Liverpool reviewers asked for, leaving no word budget for an additional §28 substitution that would not collide with H3's edits. So the only honest path forward is the Erik-only repo action the criticism explicitly offered as the alternative, with the application document left exactly as fix-h3 leaves it. Among the three repo options, GitHub-archive (Option 1) is the lowest-effort and the most consistent with M4's parallel remediation of `deep-research-competition`: any v2-era public scaffold that has not been picked up under v3 gets a "Public archive" badge, which both removes it from the default org filter and signals to any reviewer who clicks through that the repo is intentionally inert rather than abandoned-mid-flight. README-stub (Option 2) is acceptable if archiving feels premature; commit-with-region (Option 3) is foreclosed by the fact that, per CLAUDE.md "Still to Lock Down" §11 and per the panel's own observation, the region and species set have not yet been selected as of submission day. The assembler should record this fix as "no v3 text change; routed to Erik-only action" and pass the Erik action list through to whatever pre-submission checklist tracks repo-side hygiene.

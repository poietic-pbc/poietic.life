# v3 review: domain expert (pangenomics / clinical genomics)

Reviewing `workgraph_google_application_FINAL_v3.md` at commit `70c8e7f`.
`~/poietic.life/notes/v3-link-verification-20260501.md` does not exist;
flagging missing input.

## Headline

The science *partly* lands for a pangenomics reader: the team is
unimpeachable and the reference-resource framing is true on its
face, but v3 reads as infrastructure-with-genomics-as-stage-set
rather than genomics-with-infrastructure. A sample of three
pangenomics PIs would respect the people, nod at the framing,
and ask: "what specific reference resource gets built better in
36 months?" v3 has no answer.

## Reference-resource framing

Substantively true. "Reference-resource construction is high-stakes
work: errors and biases propagate to thousands of downstream labs"
(§23) is exactly the right operational claim. The HPRC's 2023 draft
human pangenome had real curation tradeoffs (haplotype selection,
coordinate ambiguity, graph normalization choices) where audit
trails would matter.

But the framing stays gestural. v3 never names *which* reference
resource the grant operates on, what error class an audit trail
catches that current practice misses, or what a "reference-grade"
output looks like in WorkGraph terms. A pangenomics PI would
expect: "we will use WorkGraph to coordinate the curation of
[specific HPRC year-N expansion / specific vertebrate pangenome /
specific variant catalogue], with [specific quality metric] versus
the prior process." None of this is in §17a, §17b, or the
milestones. The closest §43 gets is "Garrison's pangenomics and
HPRC work," which is the founder's day job, not a deliverable.

## Track record claims

Mostly accurate.

- **vg / PGGB / HPRC**: claims hold. vg is foundational; PGGB built
  the HPRC graph (Liao et al. 2023). The "~72,000 citations" figure
  in §26 / §36 is a Garrison-corpus aggregate, not a single paper;
  consistent with Scholar profiles but unusual to cite without
  footnote.
- **CRISPResso2**: ~18,700 cumulative citations, field standard.
  Accurate.
- **CRISPRme / Casgevy**: §26 phrasing is careful and consistent
  with CLAUDE.md guidance: "CRISPRme (Nature Genetics 2023)
  *independently identified* an off-target in the guide that
  *became* Casgevy, informing FDA review (the enhancer strategy
  *traces to* Canver et al. Nature 2015)." No implied direct
  collaboration. §36 repeats this correctly. ✓
- **Chorus**: correctly attributed to Pinello as orchestration
  for genomic AI including AlphaGenome.
- **C.Origami / Chromnitron**: not present in v3. ✓
- **PHR (Nature 2023)**: cited as Garrison track record in §36.
  Note: this is now legacy citation only. v3 dropped PHR as
  *deliverable* but kept it as *credential*. Defensible but
  slightly awkward.

## Demonstration credibility

"Longitudinal deployment in the founders' active research" reads
more honest than v2's PHR-atlas-with-named-clinical-candidates,
but the cost is concreteness. "Lab adoption" as the falsifiable
metric is real, yet adoption telemetry tells you uptake, not
scientific quality. A pangenomics reviewer will want at least one
concrete co-authored deliverable from the deployment by month 18:
e.g., a pangenome construction paper or variant catalogue update
where the methods section literally points at a published
WorkGraph computation graph. v3 implies this in §43 ("preprints,
software releases, datasets") but does not commit to a specific
artifact. This reads soft.

## What's missing scientifically

- Specific genomic scope (which species, which chromosomes, which
  cohort, which graph build).
- Specific quality metric (graph compression, alignment recall,
  variant calling F1, curation decision count).
- Compute-scale reality check: HPRC-class graph construction is
  thousands of CPU-hours; $300K cloud over 36 months is plausible
  for coordination and demos but not for atlas-scale work.
- One named external pangenomics collaborator. §31 keeps partner
  fields blank; that's fine for the form but a domain reviewer
  would want at least one HPRC or VGP figure named in §26.

## What v3 lost relative to v2

The three-way methodology comparison (WG-with-Erik vs
single-session CLI vs solo bioinformatician). Even granting it was
"built for the format," it was *concrete and falsifiable* and gave
a reviewer something to imagine reading. v3 has no equivalent set
piece. The PHR-rare-disease bridge was the riskier loss
scientifically, but defensible: 36 months is too short for clinical
validation, and tying success to an outside cohort partnership was
fragile. Dropping that was correct. Dropping the comparison demo
without a replacement set piece was costly.

## Feasibility

Plausible. Team is real, senior, and the right people for this
problem. Budget structure (~$900K personnel + $300K compute +
$150K infra + $150K amplification) is sane for a 3-founder PBC
with two RSEs. The 50-lab adoption target by month 36 is
ambitious but not unprecedented (vg, CRISPResso reached this
scale). Real risk is single-point-of-failure on Garrison for
WorkGraph core; §30 names this but the second-engineer hire is
the only mitigation, which is thin.

Overall: scientifically honest, less scientifically *vivid* than
it could be. The team can carry this, but the proposal is asking
reviewers to take that on faith.

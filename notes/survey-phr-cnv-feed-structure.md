# Survey: PHR Copy-Number Enrichment Feed Structure

Source: https://ulivo.poietic.life/wg/feeds/phrs-cnv-study/

## Findings

1. The feed is a 574-task WorkGraph export, with the relevant work concentrated in completed copy-number-aware PHR gene enrichment, validation, and synthesis branches. The visible core tasks are overwhelmingly `done`; a small number of abandoned/open items are mostly meta verification/evaluation branches, not core scientific work.

2. The first major cluster is a sequential PHR enrichment pipeline: `research-inventory-files -> step-1-extract-chm13 -> step-2-intersect-genes -> step-3-run-go -> step-4-compare-phr -> step-5-reconcile-with`. Logs show CHM13 PHR BED extraction, 412 gene entries/245 unique gene names, GO enrichment with 25 BP and 3 MF significant terms, then comparison against Angela/Andrea analyses.

3. The central cluster is copy-number-aware enrichment methodology. `research-copy-number` fans out into methods/tooling/statistics tasks, including GREAT/rGREAT, permutation, weighted gene, weighted hypergeometric, `phyper()` mapping, validation, benchmarking, R implementation, and final recommendations. Later repair/retry branches (`fix-map-copy-2`, `statistical-validation-framework-2`, `synthesize-r-phyper-2`) converge into `integrate-final-recommendations`.

4. The third major cluster is biological interpretation of the signal. Deep research branches cover OR4F/olfactory receptors, DUX4/FRG2 regulation, TUBB8/tubulin biology, and GTP/GPCR-related genes. OR4F and TUBB8 each fan out further into copy-number, disease/function, assembly, paralog, and subtelomeric-positioning literature tasks, then converge through `integrate-or4f-deep`, `integrate-tubb8-literature`, and `synthesis-integrate-deep`.

5. The scientific activity appears to have moved from raw interval/gene extraction to enrichment, artifact checking, copy-number correction, weighted/hypergeometric methodology, validation, and paper-ready synthesis. Logged claims include PHR-only analysis removing neighborhood artifacts, identifying RNA splicing as a true PHR profile, documenting copy-aware enrichment effects such as 598x olfactory, 309x GTP binding, and 928x transcription regulation enrichment, and validating 20+ claims with a reported 95% perfect-match rate.

## Ultra-Short Card Copy

A living research graph turned PHR intervals into copy-aware enrichment, validation, and paper-ready biological interpretation.

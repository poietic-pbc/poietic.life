# Erik Garrison Bio Fact-Check - 2026-05-01

## Replacement bio

Erik Garrison is Associate Professor in Genetics, Genomics and Informatics at the University of Tennessee Health Science Center. He created `vg`, the variation-graph toolkit published in *Nature Biotechnology* in 2018, and co-led PGGB, the PanGenome Graph Builder published in *Nature Methods* in 2024. PGGB is one of the pangenome graph approaches used/tested by the Human Pangenome Reference Consortium; frame it as HPRC-scale pangenome graph infrastructure, not as the sole HPRC builder. Google Scholar currently lists about 57,800 total citations for Garrison's profile, while the 2018 `vg` paper has about 631 Google Scholar citations and the 2024 PGGB paper has about 175 Nature-tracked citations, so avoid the "72,000 citations" wording. WorkGraph can be described as a system he is building and leading; local `graphwork/workgraph` history shows Erik as the dominant author by commit count.

## Landing-page version

Erik Garrison is Associate Professor of Genetics, Genomics and Informatics at UTHSC. He created `vg`, the variation-graph toolkit published in *Nature Biotechnology* in 2018, and co-led PGGB, the PanGenome Graph Builder published in *Nature Methods* in 2024. His pangenome graph work is part of the tool ecosystem used at HPRC scale. He is WorkGraph's architect and lead developer.

## Grant-copy version

Reference-grade pangenomics: Garrison created `vg` (Garrison et al., *Nature Biotechnology* 2018), co-led PGGB (Garrison et al., *Nature Methods* 2024), and contributes pangenome graph tooling used at Human Pangenome Reference Consortium scale. He is Associate Professor at UTHSC and holds active NHGRI pangenome-tooling funding (U01HG013760, "Building Tools and Community to Make Pangenomes Accessible"). WorkGraph is his current open-source coordination substrate for auditable human/agent research work.

## Claim-by-claim verdict

| Claim | Verdict | Notes |
|---|---|---|
| Affiliation: University of Tennessee Health Science Center | Keep, strengthen if desired | UTHSC lists Erik Garrison, PhD as Associate Professor in the Department of Genetics, Genomics and Informatics. NHGRI also lists him at UTHSC for active HGRP tool-development award U01HG013760. |
| "Created `vg`" | Keep | Supported by the 2018 *Nature Biotechnology* `vg` paper with Garrison first author and by his 2019 blog saying he built the working system and the vgteam formed around it. |
| "`vg` (Nature Methods 2024)" | Remove/fix | This is incorrect. `vg` is *Nature Biotechnology* 2018. *Nature Methods* 2024 is PGGB / "Building pangenome graphs." |
| "Built PGGB" | Keep, preferably "co-led PGGB" | The PGGB citation lists Erik Garrison and Andrea Guarracino as equal first/co-leading authors. "Built" is acceptable for short landing copy; "co-led" is cleaner in grant copy. |
| "PGGB used by HPRC to build the human pangenome reference" | Soften | Safer wording: "used/tested at HPRC scale" or "one of the pangenome graph approaches used by HPRC." HPRC/NHGRI list Pangenome Graph Builder alongside Minigraph and Minigraph-Cactus. |
| "~72,000 Google Scholar citations across the toolkit" | Remove or replace | Google Scholar profile currently shows 57,801 total citations, not 72k. The 2018 `vg` paper shows 631 citations in Google Scholar; Nature shows 782 tracked citations. If a number is needed, use "Google Scholar lists 57k+ citations across Garrison's profile" but this includes major consortium papers, not only the `vg` toolkit. |
| "Author on Nat Biotechnol 2018 and Nat Methods 2024" | Keep, but specify papers | Better: "`vg`, *Nature Biotechnology* 2018; PGGB, *Nature Methods* 2024." |
| "Leads NSF PPoSS LARGE award ($5M) for computational pangenomics" | Soften unless separately documented | Cornell's 2021 article says the Panorama project is led by Christopher Batten and includes Erik Garrison from UTHSC. Papers acknowledge NSF PPoSS Award #2118709 to E.G./P.P., but the public article does not support "Garrison leads the $5M award." |
| "WorkGraph architect and lead developer" | Keep with local-evidence caveat | Public web sources do not independently label him this way, but local `graphwork/workgraph` git history shows 1,906 of 2,000+ commits by Erik Garrison. This is supportable for owned landing copy. |

## Sources

- UTHSC faculty page: https://www.uthsc.edu/genetics/faculty-staff.php
- NHGRI HGRP participants / active U01HG013760: https://www.genome.gov/Funded-Programs-Projects/Human-Genome-Reference-Program
- `vg` paper: https://www.nature.com/articles/nbt.4227
- PGGB / "Building pangenome graphs": https://www.nature.com/articles/s41592-024-02430-3
- PGGB repository / HPRC-scale wording: https://github.com/pangenome/pggb
- HPRC overview: https://humanpangenome.org/
- Google Scholar profile resolved via DBLP: https://scholar.google.com/citations?user=d5TKoncAAAAJ and https://dblp.org/pid/98/9718
- Erik's `vg` background post: https://ekg.github.io/2019/07/09/Untangling-graphical-pangenomics.html
- NSF/Cornell Panorama project article: https://news.cornell.edu/node/322861
- Local WorkGraph evidence: `/home/erik/workgraph`, `git rev-list --count HEAD` = 2094; `git log --format='%an <%ae>' --max-count=2000 | sort | uniq -c | sort -nr | head` = 1906 commits by Erik Garrison.

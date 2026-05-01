# Fact-check: Luca Pinello bio and grant copy

Date: 2026-05-01
Task: factcheck-luca-bio

## Recommended replacement bio

**Affiliation line**

> Massachusetts General Hospital / Harvard Medical School / Broad Institute

**Landing-page bio**

> Luca Pinello is an Associate Professor of Pathology at Massachusetts General Hospital and Harvard Medical School, with affiliations to the Broad Institute. His lab develops computational tools for genome editing and regulatory genomics, including CRISPResso/CRISPResso2 for quantifying genome-editing outcomes and CRISPRme for variant-aware CRISPR off-target assessment. CRISPRme identified a population-specific candidate off-target for the BCL11A enhancer guide used in exa-cel/Casgevy, and that locus was discussed in FDA advisory materials for Casgevy. His lab also develops Chorus, an open-source framework that exposes sequence-to-function models, including AlphaGenome, through a common API and MCP interface.

**Shorter landing-card version**

> Develops computational tools for genome editing and regulatory genomics, including CRISPResso/CRISPResso2 and CRISPRme. CRISPRme identified a variant-dependent candidate off-target for the BCL11A enhancer guide used in exa-cel/Casgevy, later discussed in FDA advisory materials. His lab also develops Chorus, a common interface for sequence-to-function AI models including AlphaGenome.

## Claim checks

### Affiliation string

Keep "Massachusetts General Hospital / Harvard Medical School / Broad Institute" for a compact landing-card affiliation. Support:

- Harvard Chan profile lists Luca Pinello as Associate Professor of Biostatistics and lists "Associate Professor of Pathology, Pathology-Massachusetts General Hospital, Harvard Medical School" under other positions: https://hsph.harvard.edu/profile/luca-pinello/
- MGH Pinello Lab page lists Associate Professor of Pathology, Harvard Medical School, Mass General Brigham Cancer Institute, Faculty, Mass General Pathology: https://www.massgeneral.org/cancer-center/clinical-trials-and-research/center-for-cancer-research/investigators/pinello-lab
- CRISPResso2 paper lists Luca Pinello affiliations at Broad Institute, MGH, and Harvard Medical School: https://www.nature.com/articles/s41587-019-0032-3

If there is room, the most precise long form is:

> Associate Professor of Pathology, Massachusetts General Hospital and Harvard Medical School; affiliated with the Broad Institute.

### CRISPResso2 wording

Current copy says:

> Built CRISPResso2, the standard for CRISPR editing analysis (18,700+ citations).

Replace or soften. "Built" is acceptable if used informally, but "created/developed" is more precise because CRISPResso2 is coauthored. "The standard" is supportable from MGH's own lab page for CRISPResso, but a safer third-party wording is "widely used." The citation number should be removed unless a current Google Scholar source is captured, because Nature's live metric for the 2019 CRISPResso2 paper is about 1.6k citations, not 18.7k.

Recommended:

> co-developed CRISPResso/CRISPResso2, widely used tools for quantifying and visualizing genome-editing outcomes

Sources:

- CRISPResso2 paper, Nat Biotechnol 2019, lists code availability and Luca Pinello as a corresponding/senior author: https://www.nature.com/articles/s41587-019-0032-3
- PubMed record for CRISPResso2: https://pubmed.ncbi.nlm.nih.gov/30809026/
- MGH Pinello Lab page says CRISPResso became a standard for quantifying and visualizing CRISPR editing outcomes: https://www.massgeneral.org/cancer-center/clinical-trials-and-research/center-for-cancer-research/investigators/pinello-lab

### CRISPRme / Casgevy framing

Current copy says:

> His group's CRISPRme independently identified an off-target in the BCL11A guide that became Casgevy, informing the FDA review.

This is directionally right but too compressed. More precise:

> CRISPRme identified a variant-dependent candidate off-target for the BCL11A enhancer guide used in exa-cel/Casgevy; that locus was discussed in FDA advisory materials and assessed in the off-target risk review.

Support:

- Cancellieri et al., Nat Genet 2023, developed CRISPRme and tested a BCL11A enhancer gRNA in clinical trials for sickle cell disease and beta-thalassemia, finding a top candidate off-target produced by an African-ancestry allele: https://www.nature.com/articles/s41588-022-01257-y
- FDA workshop summary notes Luca Pinello presented CRISPRme and describes analyses for sickle cell disease and beta-thalassemia trials using a BCL11A enhancer-targeting gRNA: https://www.fda.gov/media/171593/download
- FDA advisory committee transcript states guide RNA 1617 was the guide used in the editing therapy under discussion, and that the Cancellieri et al. site was evaluated in the off-target assessment: https://www.fda.gov/media/175686/download
- Vertex/FDA-facing product framing for Casgevy: exa-cel edits autologous CD34+ cells at the erythroid-specific enhancer region of BCL11A: https://news.vrtx.com/news-releases/news-release-details/vertex-and-crispr-therapeutics-announce-us-fda-approval

Avoid:

- "identified an off-target in Casgevy" without "candidate" or "variant-dependent"
- "caused FDA approval" or "validated by FDA"
- Any wording implying direct collaboration with Vertex/CRISPR Therapeutics unless separately sourced

### Chorus framing

Current copy says:

> Built Chorus to orchestrate genomic AI models.

Keep but make the function concrete and avoid overclaiming "orchestration" if readers may expect production workflow orchestration. GitHub supports:

> His lab develops Chorus, an open-source common API and MCP interface for sequence-to-function models including Enformer, Borzoi, ChromBPNet/BPNet, Sei, LegNet, and AlphaGenome.

Source:

- pinellolab/chorus README describes "one API over six state-of-the-art deep-learning models," natural-language use via Claude, and AlphaGenome support: https://github.com/pinellolab/chorus

Avoid:

- "first to integrate AlphaGenome"
- "clinical-grade AI orchestration"
- "Google/DeepMind partnership" unless separately documented

### IGVF / Broad / HMS / MGH claims

Supported:

- Luca Pinello is listed by IGVF/NHGRI as an awardee on HG012010, "Comprehensive characterization of variants underlying heart and blood diseases with CRISPR base editing": https://igvf.org/awardees/
- NHGRI IGVF page lists the same characterization award: https://www.genome.gov/Funded-Programs-Projects/Impact-of-Genomic-Variation-on-Function-Consortium
- MGH Pinello Lab page says the lab is leading one of the characterization centers of the NHGRI IGVF Consortium: https://www.massgeneral.org/cancer-center/clinical-trials-and-research/center-for-cancer-research/investigators/pinello-lab
- Broad 2021 article calls Pinello a Broad associate member and associate professor at MGH/HMS, but says the Broad IGVF project is led by Bernstein/Buenrostro/Epstein: https://www.broadinstitute.org/news/broad-scientists-join-new-consortium-studying-function-genetic-variation

Recommended grant wording:

> Pinello is an IGVF awardee whose lab leads one IGVF characterization center focused on heart and blood disease variants using CRISPR base editing.

Avoid:

- "leads the Broad IGVF project"
- "Broad IGVF center lead" unless the specific Broad center is meant and sourced

### COI-sensitive claims

Keep DNA-Diffusion and generative DNA outside funded scope. MGH page discusses generative AI and DNA-Diffusion as active Pinello lab research, but the proposal should present it as track record or adjacent capability only, not as a funded deliverable, product, therapy, or clinical promise.

Recommended:

> Adjacent generative-DNA work, including DNA-Diffusion, is disclosed as related track record and remains outside the funded WorkGraph scope.

Avoid:

- "WorkGraph will design therapeutic DNA sequences"
- "synthetic regulatory elements are a grant deliverable"
- "new drugs," "therapeutic applications," or "targeted treatments" in WorkGraph-funded scope

## Claims to remove or soften

- Remove "(18,700+ citations)" unless a current source is captured and identified as Google Scholar or another specific metric. Nature's own metric for the CRISPResso2 paper is about 1.6k citations as of this check.
- Replace "the standard for CRISPR editing analysis" with "widely used tools for quantifying and visualizing genome-editing outcomes" or attribute the stronger claim to the MGH lab page.
- Replace "off-target in the BCL11A guide that became Casgevy" with "variant-dependent candidate off-target for the BCL11A enhancer guide used in exa-cel/Casgevy."
- Replace "informing the FDA review" with "discussed in FDA advisory materials and assessed in the off-target risk review."
- Replace "Built Chorus to orchestrate genomic AI models" with "develops Chorus, an open-source common API and MCP interface for sequence-to-function models including AlphaGenome."
- Avoid using Pinello's DNA-Diffusion/generative-DNA work as funded scope or as a promised WorkGraph output.

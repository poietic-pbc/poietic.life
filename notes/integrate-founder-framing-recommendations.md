# Integrate Founder Framing Recommendations

Task: `integrate-founder-framing-recommendations`  
Date: 2026-05-01/02  
Scope: Erik Garrison and Vaughn Tan founder-card wording only. No site files edited.

## Recommendation

Use small replacements inside the existing founder cards rather than expanding the section. The current live `index.html` is already close; these edits make two improvements:

- Erik: signal long-running open-source genomics infrastructure across variant calling, variation graphs, pangenome graph construction, and chromosome biology without adding citation-count or sole-builder claims.
- Vaughn: switch the primary link from the newsletter to the more directly relevant not-knowing hub and tighten the wording around organization design under uncertainty.

Do not add a second Vaughn link unless the card later becomes a longer profile. One link is cleaner here.

## Exact Proposed HTML Edits

### Erik Garrison

Replace the current Erik `<p class="founder-bio">...</p>` block at `index.html` lines 1189-1199 with:

```html
      <p class="founder-bio">
        Builds open genomics infrastructure for reading genomes as shared
        structure, from
        <a href="https://github.com/freebayes/freebayes">FreeBayes</a> and
        <a href="https://doi.org/10.1038/nbt.4227"><em>vg</em></a>
        to <a href="https://doi.org/10.1038/s41592-024-02430-3">PGGB</a>,
        the pangenome graph builder used at Human Pangenome Reference
        Consortium scale. His recent work connects pangenome methods to
        <a href="https://doi.org/10.1038/s41586-025-09540-8">Robertsonian chromosome biology</a>,
        resolving breakpoints behind one of the most common human chromosomal
        rearrangements. WorkGraph architect and lead developer.
      </p>
```

Link targets:

- `FreeBayes`: `https://github.com/freebayes/freebayes`
- `vg`: `https://doi.org/10.1038/nbt.4227`
- `PGGB`: `https://doi.org/10.1038/s41592-024-02430-3`
- `Robertsonian chromosome biology`: `https://doi.org/10.1038/s41586-025-09540-8`

Why this version: it keeps the current card length about the same, preserves the strongest existing `vg` / PGGB / Robertsonian signal, and adds FreeBayes as a light cue that Erik's work predates the pangenome graph era. It avoids "sole HPRC builder", citation-count, and overprecise 109-year historical framing.

### Vaughn Tan

Replace the current Vaughn `<p class="founder-bio">...</p>` block at `index.html` lines 1222-1229 with:

```html
      <p class="founder-bio">
        Author of <em>The Uncertainty Mindset</em> (Columbia University Press,
        2020) and a Harvard PhD in organizational behavior/sociology. Tan
        studies <a href="https://vaughntan.org/notknowing">not-knowing</a>,
        organization design, and team adaptation under uncertainty; that work
        informs WorkGraph's approach to keeping human judgment explicit in
        hybrid human-AI research coordination.
      </p>
```

Link target:

- `not-knowing`: `https://vaughntan.org/notknowing`

Why this version: the not-knowing hub is a better reviewer click than the newsletter because it directly presents the uncertainty/not-knowing framework and links onward to the relevant essays. The wording remains conservative: it says Tan's work informs WorkGraph's approach, not that his book or ASQ article directly studied human-AI scientific teams.

## Alternate More Minimal Text-Only Edit

If the implementation should keep current line breaks and links nearly intact, make only these substitutions:

```diff
-        Created <a href="https://doi.org/10.1038/nbt.4227"><em>vg</em></a>
-        and co-led <a href="https://doi.org/10.1038/s41592-024-02430-3">PGGB</a>,
-        open pangenome graph tools used at Human Pangenome Reference Consortium
-        scale. He has led work on
-        <a href="https://doi.org/10.1038/s41586-023-05976-y">pseudo-homologous regions</a>
-        and <a href="https://doi.org/10.1038/s41586-025-09540-8">recurrent Robertsonian chromosomes</a>,
-        resolving breakpoints behind one of the most common human chromosomal
-        rearrangements.
+        Builds open genomics infrastructure for reading genomes as shared
+        structure, from <a href="https://github.com/freebayes/freebayes">FreeBayes</a>
+        and <a href="https://doi.org/10.1038/nbt.4227"><em>vg</em></a>
+        to <a href="https://doi.org/10.1038/s41592-024-02430-3">PGGB</a>,
+        the pangenome graph builder used at Human Pangenome Reference
+        Consortium scale. His recent work connects pangenome methods to
+        <a href="https://doi.org/10.1038/s41586-025-09540-8">Robertsonian chromosome biology</a>,
+        resolving breakpoints behind one of the most common human chromosomal
+        rearrangements.
```

```diff
-        <a href="https://vaughntan.org/newsletter">writes about</a>
-        organization design, innovation, and team adaptation under uncertainty;
-        that work informs WorkGraph's approach to keeping human
+        studies <a href="https://vaughntan.org/notknowing">not-knowing</a>,
+        organization design, and team adaptation under uncertainty; that work
+        informs WorkGraph's approach to keeping human
```

## Fact-Check Notes

- FreeBayes is a Bayesian haplotype-based variant detector; the public repository names Erik Garrison and Pjotr Prins as maintainers and cites Garrison & Marth arXiv:1207.3907.
- `vg` is the variation-graph toolkit from Garrison, Siren, Novak et al., *Nature Biotechnology* 36:875-879 (2018), DOI `10.1038/nbt.4227`.
- PGGB is the PanGenome Graph Builder from Garrison and Guarracino et al., *Nature Methods* 21:2008-2012 (2024), DOI `10.1038/s41592-024-02430-3`; "used at HPRC scale" is safer than implying PGGB is the sole HPRC graph builder.
- The Robertsonian chromosome paper is de Lima, Guarracino, Koren et al., *Nature* 647:952-961, published 2025-09-24, DOI `10.1038/s41586-025-09540-8`; Erik Garrison is an author.
- Vaughn Tan's best primary landing-page link is `https://vaughntan.org/notknowing`, not the newsletter page, because it directly frames his not-knowing/uncertainty work.
- Tan wording should remain "informs WorkGraph's approach" rather than claiming his public writings are about human-AI scientific teams.

## Validation

- Upstream Erik, Vaughn, and Robertsonian research outputs reviewed.
- Current `index.html` founder-card markup reviewed.
- Exact proposed HTML/text replacements and link targets provided.
- No site files edited.

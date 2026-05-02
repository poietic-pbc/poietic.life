# PHR CNV Landing Card Framing

Task: `evaluate-phr-cnv-landing-card-framing`

## Recommendation

Replace the current broad "Diverse scientific activity" card with a focused trace of copy-number-aware gene enrichment analysis around PHRs. The card should read as a concrete WorkGraph example, not as a general science portfolio card.

Best title:

> PHR enrichment trace

Other viable title options:

- Copy-number-aware enrichment
- PHR analysis workflow
- Pangenome enrichment work
- PHR research graph

Recommended description:

> WorkGraph coordinated copy-number-aware gene enrichment analysis around PHRs, spanning mapping, weighted hypergeometric methods, validation, and synthesis. The result is an inspectable research trace rather than a static project summary.

Recommended link text:

> open PHR trace ->

Target:

> https://ulivo.poietic.life/wg/feeds/phrs-cnv-study/

## Rationale

The current card at `index.html:1305` is titled "Diverse scientific activity" and then uses a four-item list at `index.html:1307` through `index.html:1315`. That makes it longer and less specific than the neighboring demo cards, which use compact two-sentence descriptions and a single link.

The live feed supports a more specific trace. The center of gravity is copy-number-aware gene enrichment around PHRs: weighted hypergeometric methods, parameter mapping, validation, benchmarking, synthesis, and later GO/enrichment reconciliation. Subtelomeric and copy-number task names are supporting evidence, not the headline.

The safest framing is therefore not "generic CNV discovery" and not "subtelomere discovery." It is "copy-number-aware gene enrichment analysis around PHRs, coordinated through mapping, weighted methods, validation, and synthesis."

## Wording To Avoid

- Avoid "Diverse scientific activity"; it is vague and makes the card less demo-like.
- Avoid "subtelomere discovery" as the main title unless the final synthesizer wants to foreground OR4F/TUBB8 specifically.
- Avoid "CNV discovery" alone; the trace is about copy-number-aware methodology and enrichment, not just discovering CNVs.
- Avoid "clinical PHR results," "diagnostic candidates," or "rare-disease diagnosis" unless a separate source verifies that this specific live trace produced those outputs.
- Avoid "PHR atlas" for this landing card; it sounds like a product or completed resource rather than a trace of ongoing research coordination.

## Drop-In Shape

```html
<h3 class="built-title">PHR enrichment trace</h3>
<p class="built-desc">
  WorkGraph coordinated copy-number-aware gene enrichment analysis around PHRs,
  spanning mapping, weighted hypergeometric methods, validation, and synthesis.
  The result is an inspectable research trace rather than a static project summary.
  <a href="https://ulivo.poietic.life/wg/feeds/phrs-cnv-study/" class="phr-link">open PHR trace &rarr;</a>
</p>
```

If the card feels one line too long in layout, cut the second sentence to:

> Every handoff and check remains inspectable.

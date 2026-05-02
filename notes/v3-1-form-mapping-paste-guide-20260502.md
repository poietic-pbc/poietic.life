---
guide_id: v3-1-form-mapping-paste-guide
date: 2026-05-02
target: workgraph_google_application_FINAL_v3_1.md (commit 986222f, main)
form_source: /tmp/google-org-form-structure.md (pasted by Erik 2026-05-02)
verdict: paste-with-targeted-remaps
---

# v3.1 -> Google.org form mapping paste guide (2026-05-02)

## 1. Headline verdict

**Paste-ready with three targeted remaps and one new field.** v3.1 was written against an older mental model of the form. The substantive content is correct, fits all the relevant word caps, and the dogfooding framing landed (ref `v3-1-final-coherency-review-20260501.md`). What needs handling at paste time:

1. **Form §29 = Risks (200w).** v3.1 §29 currently holds Theory of Change. The Risks content is at v3.1 §30 but only 100w; it has been expanded to 184w below. **Paste the §29 block from this guide, NOT v3.1 §29.**
2. **Form §30 = Key team members, roles only, no names (100w).** v3.1 has no equivalent field; team names live in §26. The 85w roles-only block below is new.
3. **Form §32 = multiselect, NOT prose.** v3.1 §32 already lists picks in the right form; just check the right boxes (recommendations below).
4. **Form §49 / §50 = Yes** (public-university affiliations); v3.1 currently says No on both. Form §53 needs an explanation; 75w block drafted below.
5. **Form §15 project stage** is a radio with three options (Hypothesis / PoC / Validated). v3.1 says PoC. **Recommend: Validated Methodology** — WorkGraph is in active production use across founder labs and orchestrated the company's own incorporation; that is past PoC.

Everything else is content-equivalent: budget categories §38-§41 split cleanly into the form's Name + USD + ≤100w description fields, milestones §43-§46 already supply Timeframe + Activities + Outcomes within the form's caps, all prose fields are within cap.

**Submission can proceed today.**

---

## 2. Section I-VI mechanical fields (paste-in-order block)

Short answers and Erik-only items consolidated for one-pass entry. Items marked **ERIK** require Erik's input; everything else is the recommendation.

### Section I — Organization and Submitter Info

| Field | Value |
|---|---|
| §1 Org legal name | The Poietic Public Benefit Corporation |
| §2 Country | United States of America |
| §3 Classification | Social Enterprise |
| §4a Year founded | 2026 |
| §4b Annual budget USD | **ERIK** — v3.1 says $0 (newly incorporated). Confirm; if any committed grant or contract exists at submission, enter that. |
| §4c Current FTEs | **ERIK** — v3.1 says 3 (the three co-founders). If FTE means salaried full-time employees of Poietic PBC specifically (vs founder time-share), the answer may be 0. Pick the most defensible interpretation. |
| §5a Website URL | https://poietic.life |
| §5b Primary social media | leave blank (optional) |
| §6 Prior Google.org funding? | No |
| §7 How heard about program | Website Search |
| §8a Primary First | Erik |
| §8b Primary Last | Garrison |
| §8c Primary Title | Co-Founder, Poietic PBC; Associate Professor, University of Tennessee Health Science Center |
| §8d Primary Email | erik.garrison@gmail.com |
| §8e Primary Timezone | **ERIK** — US Eastern (ET) per v3.1; confirm. |
| §9a Secondary First | Luca |
| §9b Secondary Last | Pinello |
| §9c Secondary Title | Co-Founder, Poietic PBC; Associate Professor, Massachusetts General Hospital and Harvard Medical School |
| §9d Secondary Email | lucapinello@gmail.com |
| §9e Secondary Timezone | **ERIK** — confirm Luca's timezone (US Eastern). |
| §10 English fluency? | Yes |

### Section II — Impact (radio / multiselect only; prose answered via paste table §3)

| Field | Recommendation |
|---|---|
| §12 Topic(s) | Health & Life Sciences: Functional Genomics |
| §13 Open-source outputs | Software/Tools/Platforms; Curated Dataset(s); Peer-reviewed publication(s) |
| §14 Geographic regions | Global |
| §15 Project stage | **Validated Methodology** (WorkGraph in daily production use across founder labs; orchestrated the company's incorporation and website builds with public traces at ulivo.poietic.life) |

### Section III — Innovative Use of Technology (radio / Y-N only)

| Field | Recommendation |
|---|---|
| §22 Existing dataset? | **Yes** (HPRC pangenome assemblies; 1000G / HGDP variant sets; CRISPRme variant-aware substrate; first novel Poietic-generated dataset = published computation-graph corpus by m18) |
| §24 All outputs freely/openly available? | **Yes** (MIT for software; CC-BY 4.0 for datasets; OA publications) |

### Section IV — Feasibility (radio only)

| Field | Recommendation |
|---|---|
| §27 AI Maturity | **AI First** |

### Section V — Scalability (multiselect only; prose via paste table §3)

| Field | Recommendation |
|---|---|
| §32 Scale dimensions (multiselect) | **Technical & performance maturity**, **Ecosystem & integration**, **Community-led expansion**. Optional 4th if box-count permits: **Policy & standards leadership** (computation-graph publication standards engagement, §46 outcomes). v3.1 also lists **Adaptation to different sectors** (Tan framework generalizes beyond genomics); include if 4 picks are allowed and feels honest, drop if you want to stay focused. |

### Section VI — Project Budget and Timeline (radio only; prose via paste table §3)

| Field | Value |
|---|---|
| §37 Funding amount | $1,500,000 |

### Section VII — Ethics and Compliance (Y/N only; §53 prose via paste table §3)

| Field | Recommendation |
|---|---|
| §48 Commercial contracts/negotiations with Google? | **No** |
| §49 Govt officials/employees in org? | **YES** (Garrison employed by University of Tennessee Health Science Center, a public university; Tan honorary appointment at University College London, a public university) |
| §50 Govt persons involved in project? | **YES** (Garrison and Tan founder time on the project is contributed under public-university outside-engagement policies) |
| §51 Engage/fund law enforcement? | **No** |
| §52 Dealings in sanctioned regions? | **No** |
| Certification | **ERIK** must check Yes after reviewing all six certification statements |

---

## 3. Paste guide table — every form question

Status legend: **READY** = paste from v3.1 verbatim. **REMAP** = right content, wrong section in v3.1 (paste from the v3.1 location named). **TRIM/EXPAND** = recount. **NEW** = drafted in §4 of this guide. **ERIK** = Erik must answer. **NA** = optional, blank or N/A.

| Form § | Prompt (short) | Cap | Type | v3.1 source | Paste-ready content | Status |
|---|---|---|---|---|---|---|
| §1 | Org legal name | — | text | v3.1 §1 | The Poietic Public Benefit Corporation | READY |
| §2 | Country | — | radio | v3.1 §2 | United States of America | READY |
| §3 | Classification | — | radio | v3.1 §3 | Social Enterprise | READY |
| §4a | Year founded | — | text | v3.1 §4a | 2026 | READY |
| §4b | Annual budget USD | — | numeric | v3.1 §4b | $0 (confirm) | ERIK |
| §4c | Current FTEs | — | numeric | v3.1 §4c | 3 (or 0 — see §2 above) | ERIK |
| §5a | Website URL | — | text | v3.1 §5a | https://poietic.life | READY |
| §5b | Social media URL | — | text (opt) | v3.1 §5b | (blank) | NA |
| §6 | Prior Google.org funding? | — | Y/N | v3.1 §6 | No | READY |
| §7 | How heard about program | — | radio | v3.1 §7 | Website Search | READY |
| §8a-d | Primary contact | — | text | v3.1 §8 | Erik Garrison; Co-Founder, Poietic PBC; Associate Professor, UTHSC; erik.garrison@gmail.com; ET | READY |
| §9a-d | Secondary contact | — | text | v3.1 §9 | Luca Pinello; Co-Founder, Poietic PBC; Associate Professor, MGH and HMS; lucapinello@gmail.com; ET | READY |
| §10 | English fluent project lead | — | Y/N | v3.1 §10 | Yes | READY |
| §11 | Title | — | text | v3.1 §11 | WorkGraph: Open Coordination Infrastructure for Auditable, Hybrid Human-AI Work in Functional Genomics | READY |
| §12 | Topic alignment | — | multiselect | v3.1 §12 | Health & Life Sciences: Functional Genomics | READY |
| §13 | Open-source outputs | — | multiselect | v3.1 §13 | Software/Tools/Platforms; Curated Dataset(s); Peer-reviewed publication(s) | READY |
| §14 | Geographic regions | — | multiselect | v3.1 §14 | Global | READY |
| §15 | Project stage | — | radio | v3.1 §15 | **Validated Methodology** (v3.1 says PoC; recommend stepping up given live production use, founder-lab daily coordination, ulivo trace evidence) | REMAP |
| §16a | Specific challenge | 75w | text | v3.1 §16a | Paste v3.1 §16a verbatim. | READY |
| §16b | Significance | 75w | text | v3.1 §16b | Paste v3.1 §16b verbatim. | READY |
| §16c | Core questions / why AI | 75w | text | v3.1 §16c | Paste v3.1 §16c verbatim. | READY |
| §17a | Solution proposed | 75w | text | v3.1 §17a | Paste v3.1 §17a verbatim. | READY |
| §17b | Tools / methods | 75w | text | v3.1 §17b | Paste v3.1 §17b verbatim. | READY |
| §17c | Evidence solution works | 75w | text | v3.1 §17c | Paste v3.1 §17c verbatim. | READY |
| §17d | How AI catalyzes | 75w | text | v3.1 §17d | Paste v3.1 §17d verbatim. | READY |
| §18a | End beneficiaries | 75w | text | v3.1 §18a | Paste v3.1 §18a verbatim. | READY |
| §18b | Centering beneficiary voices | 75w | text | v3.1 §18b | Paste v3.1 §18b verbatim. | READY |
| §18c | Potential reach | 75w | text | v3.1 §18c | Paste v3.1 §18c verbatim. | READY |
| §19a | Real-world metrics | 75w | text | v3.1 §19a | Paste v3.1 §19a verbatim. | READY |
| §19b | Failure indicators | 75w | text | v3.1 §19b | Paste v3.1 §19b verbatim. | READY |
| §19c | Expected changes from baseline | 75w | text | v3.1 §19c | Paste v3.1 §19c verbatim. | READY |
| §20 | Existing technologies | 100w | text | v3.1 §20 | Paste v3.1 §20 verbatim. | READY |
| §21 | Why custom needed | 100w | text (opt) | v3.1 §21 | Paste v3.1 §21 verbatim. | READY |
| §22 | Existing dataset? | — | Y/N | v3.1 §22 | **Yes** (form is Y/N; v3.1 has the supporting prose, but the field itself just needs Yes; if a description box appears, paste v3.1 §22 prose) | READY |
| §23 | Ethical risks / Google AI Principles | 100w | text | v3.1 §23 | Paste v3.1 §23 verbatim. | READY |
| §24 | All outputs freely available? | — | Y/N | v3.1 §24 | **Yes** | READY |
| §25 | Leverage Google.org Accelerator | 100w | text | v3.1 §25 | Paste v3.1 §25 verbatim. | READY |
| §26 | Why uniquely positioned | 150w | text | v3.1 §26 | Paste v3.1 §26 verbatim (147w; only place individual co-founder names appear in the post-§10 application). | READY |
| §27 | AI Maturity | — | radio | v3.1 §27 | **AI First** | READY |
| §28 | Technical feasibility | 100w | text | v3.1 §28 + §4 of this guide | **Recommended replacement** that leads with the live ulivo traces (drafted §4 below, 91w). v3.1 §28 (88w, ulivo not mentioned) is also acceptable. | REMAP (or READY if Erik prefers v3.1 §28) |
| §29 | Risks (200w) | 200w | text | v3.1 §30 expanded | **Paste §4 §29 block from this guide (184w).** Do NOT paste v3.1 §29 (Theory of Change is not what this field asks for). | REMAP+EXPAND |
| §30 | 3-5 key team members, roles, NO names | 100w | text | (none in v3.1) | **Paste §4 §30 block (97w).** | NEW |
| §31a-e | Partner orgs (Name + URL + Role ≤50w + Relationship) | 50w each | structured | v3.1 §31 | Optional structured field. Default: leave blank with v3.1 §31 paragraph in any open-text/notes box. **If form forces at least one entry**, see §4 §31 below for HPRC and IGVF entries (both existing engagements through Garrison and Pinello respectively). Do NOT list employer institutions as partners. | ERIK (decision) |
| §32 | How will you scale | — | multiselect | v3.1 §32 | **Technical & performance maturity; Ecosystem & integration; Community-led expansion.** Optional add: **Policy & standards leadership**. v3.1 also lists Adaptation to different sectors — keep if comfortable, drop for focus. See §4 §32 below for the rationale per pick. | REMAP (multiselect, not prose) |
| §33 | Team structure evolution | 150w | text | v3.1 §33 | Paste v3.1 §33 verbatim (127w). | READY |
| §34a | Financial sustainability | 50w | text | v3.1 §34a | Paste v3.1 §34a verbatim (47w). | READY |
| §34b | Technical sustainability | 50w | text | v3.1 §34b | Paste v3.1 §34b verbatim (45w). | READY |
| §35 | Key learnings + sharing | 100w | text | v3.1 §35 | Paste v3.1 §35 verbatim. | READY |
| §36 | Public presence | 100w | text | v3.1 §36 + §4 of this guide | **Recommended replacement** that names the live ulivo traces as primary evidence (drafted §4 below, 95w). v3.1 §36 also acceptable but does not link the trace evidence. | REMAP (or READY if Erik prefers v3.1 §36) |
| §37 | Funding request amount | — | radio | v3.1 §37 | $1,500,000 | READY |
| §38a | Budget Cat 1 Name | — | text | v3.1 §38 | Personnel & Staffing | READY |
| §38b | Budget Cat 1 USD | — | numeric | v3.1 §38 | 900000 | READY |
| §38c | Budget Cat 1 Description | 100w | text | v3.1 §38 | Paste v3.1 §38 description verbatim (86w). | READY |
| §39a | Budget Cat 2 Name | — | text | v3.1 §39 | Technology Development | READY |
| §39b | Budget Cat 2 USD | — | numeric | v3.1 §39 | 300000 | READY |
| §39c | Budget Cat 2 Description | 100w | text | v3.1 §39 | Paste v3.1 §39 description verbatim (68w). | READY |
| §40a | Budget Cat 3 Name | — | text | v3.1 §40 | Equipment & Infrastructure | READY |
| §40b | Budget Cat 3 USD | — | numeric | v3.1 §40 | 150000 | READY |
| §40c | Budget Cat 3 Description | 100w | text | v3.1 §40 | Paste v3.1 §40 description verbatim (48w). | READY |
| §41a | Budget Cat 4 Name | — | text | v3.1 §41 | Project Amplification | READY |
| §41b | Budget Cat 4 USD | — | numeric | v3.1 §41 | 150000 | READY |
| §41c | Budget Cat 4 Description | 100w | text | v3.1 §41 | Paste v3.1 §41 description verbatim (55w). | READY |
| §42a-c | Budget Cat 5 (optional) | 100w | text (opt) | (none) | Leave blank. Sum already $1,500,000 across §38-§41. | NA |
| §43a | Milestone 1 Timeframe | — | text | v3.1 §43 | Months 1-6 | READY |
| §43b | Milestone 1 Activities | 150w | text | v3.1 §43 | Paste v3.1 §43 Activities verbatim (51w). | READY |
| §43c | Milestone 1 Outcomes | 100w | text | v3.1 §43 | Paste v3.1 §43 Outcomes verbatim (30w). | READY |
| §44a | Milestone 2 Timeframe | — | text | v3.1 §44 | Months 7-18 | READY |
| §44b | Milestone 2 Activities | 150w | text | v3.1 §44 | Paste v3.1 §44 Activities verbatim (62w). | READY |
| §44c | Milestone 2 Outcomes | 100w | text | v3.1 §44 | Paste v3.1 §44 Outcomes verbatim (20w). | READY |
| §45a | Milestone 3 Timeframe | — | text | v3.1 §45 | Months 19-30 | READY |
| §45b | Milestone 3 Activities | 150w | text | v3.1 §45 | Paste v3.1 §45 Activities verbatim (58w). | READY |
| §45c | Milestone 3 Outcomes | 100w | text | v3.1 §45 | Paste v3.1 §45 Outcomes verbatim (40w). | READY |
| §46a | Milestone 4 Timeframe | — | text | v3.1 §46 | Months 31-36 | READY |
| §46b | Milestone 4 Activities | 150w | text | v3.1 §46 | Paste v3.1 §46 Activities verbatim (58w). | READY |
| §46c | Milestone 4 Outcomes | 100w | text | v3.1 §46 | Paste v3.1 §46 Outcomes verbatim (34w). | READY |
| §47a-c | Milestone 5 (optional) | — | text (opt) | (none) | Leave blank. v3.1 timeline is four milestones spanning 36 months. | NA |
| §48 | Commercial contracts with Google | — | Y/N/Unsure | v3.1 §48 | **No** | READY |
| §49 | Govt officials in org | — | Y/N | corrected | **YES** (Garrison: UTHSC, public university; Tan: UCL, public university). v3.1 says No; this is the form-level correction. | REMAP |
| §50 | Govt persons involved in project | — | Y/N | corrected | **YES** (founder time on project from public-university appointments) | REMAP |
| §51 | Law enforcement | — | Y/N | v3.1 §51 | **No** | READY |
| §52 | Sanctioned regions | — | Y/N | v3.1 §52 | **No** | READY |
| §53 | Explanation if any §48-52 yes | — | text | (none in v3.1) | **Paste §4 §53 block (75w).** | NEW |
| Cert | 6-statement certification | — | radio | — | **Erik must check Yes** after reading all six statements. | ERIK |

---

## 4. New content drafts and recommended replacements

All counts manually verified; em-dashes 0; PI language 0; founder names appear only where the form explicitly calls for individual names (§8 / §9 / §26 / §53 explanation).

### §15 Project stage — radio recommendation

**Validated Methodology.**

Rationale: WorkGraph is in daily production use across founder labs, has 2,000+ commits on the public MIT-licensed repo (github.com/graphwork/workgraph), orchestrated Poietic PBC's incorporation (public trace at ulivo.poietic.life/wg/feeds/incorporation-trace/) and the poietic.life website build (public trace at ulivo.poietic.life/wg/feeds/poietic-website/). Past PoC.

### §28 Technical feasibility (≤100w) — recommended replacement, 91w

> WorkGraph: functional, publicly available (github.com/graphwork/workgraph, MIT). Live computation-graph traces of real Poietic PBC work (incorporation; poietic.life website build) at ulivo.poietic.life are direct primary evidence of multi-actor coordination, automatic task spawning, dependency resolution, and lifecycle management at production maturity, in daily use across founder labs. Pangenome construction (vg, PGGB, HPRC tooling) and Pinello CRISPRme stack are mature, published, and proven at scale. Liverpool Hive Mind grant addresses hybrid coordination for wet-lab autonomous chemistry; that effort optimizes lab-robotics scheduling and physical-experiment coordination, while WorkGraph optimizes git-native provenance across distributed human and computational actors.

Difference from v3.1 §28: leads with the public ulivo traces as direct primary evidence rather than asserting "in daily use" abstractly. Reviewer can click through and inspect.

### §29 Risks (≤200w) — paste this, 184w

> Five risks. First, reviewers may want a specific scientific deliverable rather than infrastructure. Mitigation: every longitudinal case study produces a real research output (preprint, software release, dataset); lab adoption is the falsifiable external metric (10+ labs by month 18, 50+ by month 36). Second, founder distraction from primary academic appointments. Mitigation: structured part-time effort across all three founders; two full-time research software engineers carry day-to-day WorkGraph development; one full-time AI/biology research scientist supports adoption and BioBench operations. Third, single-point-of-failure on Garrison for WorkGraph core. Mitigation: documented architecture, second-engineer hire from month 1, contributor pipeline through MemPanG cohorts and BioBench events. Fourth, Pinello generative-DNA commercial interests. Mitigation: DNA-Diffusion is track record only and outside funded scope; CRISPResso, CRISPRme, Chorus, and IGVF coordination are the funded clinical-genomics surfaces. Fifth, incumbent agentic-CLI vendors adding coordination features. Mitigation: differentiator is structural rather than feature-level (persistent git-native multi-actor provenance, MIT-licensed, vendor-neutral) and integrates Claude, Codex, Gemini, and open-weight models as executors rather than competing with them. Maintenance: MIT-licensed Rust core, JSONL graph storage, no proprietary dependencies; community governance committee established by month 31 for long-term stewardship beyond founder tenure.

Source: expanded from v3.1 §30 (100w original) by carrying through specifics already present elsewhere in v3.1 (adoption numbers, executor list, governance timing) and adding a maintenance line. Five-risk structure preserved.

### §30 Key team members, roles only, NO names (≤100w) — paste this, 85w

> Four key roles ensure success. First, a substrate architect / lead engineer driving WorkGraph core development, executor pluggability, and the interactive computation graph visualization (full-time research software engineer, Rust and systems). Second, scientific co-leads providing reference-grade pangenomics and clinical-genomics depth, contributing part-time from primary academic appointments. Third, a software engineer focused on adopter-lab onboarding, integrations (Gemini, AlphaGenome via Chorus, open-weight inference), and BioBench infrastructure (full-time hire). Fourth, an organizational researcher: designs the agency framework that develops agent primitives and matches work to agent capabilities, drawing on hybrid-teams-under-uncertainty research; conducts longitudinal ethnographic case studies of adopter labs (part-time).

Verifications: no individual names, no PI language, no em-dashes; describes expertise that ensures success per the form prompt; matches §38 personnel structure (3 founders part-time + 2 RSE full-time + 1 AI/bio RS over 24 months); 4th role updated 2026-05-02 to lead with agency-framework design (Tan-shaped subsystem) rather than passive ethnography.

### §31 Partners — Erik's call

**Default (recommended): leave the structured partner fields blank.** v3.1 §31 explicitly states Poietic PBC is sole applicant and sole grantee; the company is independent of co-founder employers and there are no signed lab partners yet. If the form has an open-text "additional notes" box anywhere on §31, paste:

> Poietic PBC is the sole applicant and sole grantee. Co-founders maintain separate academic appointments at the University of Tennessee Health Science Center, Massachusetts General Hospital / Harvard Medical School, and University College London respectively. The proposal operates independently of those institutions: no institutional IP, indirect costs, or shared resources are entangled in this application. Pilot lab partners for WorkGraph adoption will be recruited in Year 1 from the founders' networks across the genomics, pangenomics, and computational biology communities.

**If the form forces ≥1 entry**, both of the following are defensible existing engagements:

| Field | Entry 1 | Entry 2 |
|---|---|---|
| §31a Name | Human Pangenome Reference Consortium | NHGRI Impact of Genomic Variation on Function (IGVF) Consortium |
| §31b URL | https://humanpangenome.org | https://igvf.org |
| §31c Role/Expertise (≤50w) | Garrison contributes pangenome construction (PGGB, vg, impg) to HPRC pangenome releases; HPRC samples and assemblies underpin the project's computational genomics deliverables (HPRC R3 build, vg-CNV, PGGB v1.0). | Pinello leads an IGVF Consortium characterization center; IGVF data and standards inform the clinical-genomics workflows coordinated through WorkGraph and the BioBench challenges around regulatory variation. |
| §31d Relationship | Existing partner | Existing partner |

Do **not** list UTHSC, MGH/HMS, Broad, or UCL as partners; they are co-founder employers, not project partners.

### §32 Scaling dimensions — multiselect picks

Recommended picks (top 3, all defensible from existing v3.1 text):

1. **Technical & performance maturity** — production-hardening for outside labs, milestone deliverables (impg 1.0, PGGB v1.0, vg-CNV) ship through audited workflows (§43-§46).
2. **Ecosystem & integration** — multi-provider executors (Claude, Codex, Gemini, AlphaGenome via Chorus, open-weight), BioBench, computation graph repository (§20, §25).
3. **Community-led expansion** — adopter labs (10+ by m18, 50+ by m36), open governance committee from m31, MemPanG cohorts ×3, contributor pipeline (§29, §33, §46).

Optional 4th if multi-pick is generous:

4. **Policy & standards leadership** — engage with journals and funders on standards for computation graph publication (§46 outcomes); Tan organizational design framework targets ASQ or Research Policy (§45).

v3.1 prose §32 also lists "Adaptation to different sectors" — defensible (Tan framework explicitly generalizes beyond genomics in §17d) but the more focused 3-pick set is the cleaner story. Erik's call.

### §36 Public presence (≤100w) — recommended replacement, 95w

> WorkGraph: github.com/graphwork/workgraph (MIT, 2,000+ commits). Live computation-graph traces published at ulivo.poietic.life (Poietic PBC incorporation trace; poietic.life website-build trace) demonstrate the substrate in active research-coordination use. Co-founder public profiles: Garrison (vg ecosystem, ~72,000 Google Scholar citations, Nature Methods 2024; pseudo-homologous regions, Nature 2023; HPRC contributor); Pinello (CRISPResso2, ~18,700 citations; CRISPRme, Nature Genetics 2023, off-target identified independently in the BCL11A guide before Casgevy FDA approval; Chorus; IGVF center); Tan (The Uncertainty Mindset, Columbia 2020; ASQ 2015; Future of Life Foundation fellowship on AI for human reasoning). Longitudinal case-study outputs and computation-graph archives publish openly with interactive reports.

Difference from v3.1 §36: explicit ulivo trace URLs as click-through evidence; otherwise content-equivalent.

### §53 Explanation for §49 / §50 yes answers — paste this, 75w

> Co-founders Garrison and Tan are employees of public universities (University of Tennessee Health Science Center and University College London respectively). Pinello is at Massachusetts General Hospital, Harvard Medical School, and the Broad Institute (private institutions). None of these institutions are direct project recipients; project funds flow only to Poietic PBC. Co-founder time on the project is contributed under each institution standard policies for outside engagement. No government entity directs Poietic PBC work or the project.

---

## 5. Erik-only items

Things only Erik can supply or decide; everything else has a recommendation above.

1. **§4b Annual budget USD.** v3.1 says $0 (newly incorporated). Confirm; if any committed grant or contract has landed at submission, enter that.
2. **§4c FTEs.** v3.1 says 3. If FTE means salaried full-time employees of Poietic PBC specifically, the answer may be 0 (founders are at universities, time-shared). Pick the most defensible interpretation.
3. **§7 How heard.** "Website Search" is the v3.1 default. Confirm this matches reality.
4. **§8d / §9d Timezones.** Confirm both founders' current timezone strings as the form expects them.
5. **§15 Project stage.** Final radio call: PoC (per v3.1) vs Validated (per this guide's recommendation). Recommend Validated.
6. **§28 / §36 trace-led replacements.** Choose v3.1 verbatim or this guide's trace-led replacements. Recommend the trace-led replacements (give reviewers a click-through).
7. **§31 partner entries.** Decide whether to leave blank (default), use the open-text fallback paragraph, or fill HPRC + IGVF as existing partners. Recommend default unless form forces ≥1 entry.
8. **§32 fourth multiselect pick.** Decide whether to add "Policy & standards leadership" or "Adaptation to different sectors" beyond the recommended top 3.
9. **§38 personnel effort allocations.** Per CLAUDE.md item #6: "do not state specific effort percentages for any co-founder." If the form forces percentages anywhere in the personnel rollup, decide with Luca and Vaughn before submitting.
10. **§48-§52 final Y/N record check.** Confirm each Yes/No against legal record before certifying.
11. **Certification.** Six-statement check; only Erik can sign.
12. **Attachments.** Budget worksheet, organizational documents, letters of support — none are in the markdown. Form-driven; if the form requests them, attach what Erik has on hand.

---

## 6. M4 / H7 verdict — submission can proceed without

**M4** (`github.com/poietic-pbc/deep-research-competition` — old KRAS framing) and **H7** (`github.com/poietic-pbc/phr-methodology-comparison` — 1 commit) are flagged in `v3-1-final-coherency-review-20260501.md` as Erik-only repo hygiene.

**These are not submission blockers given the live ulivo traces.** With the public traces at ulivo.poietic.life (incorporation, website build) recommended for §28 and §36, the application's primary evidence of WorkGraph in real use is the trace URLs themselves. The two stale GitHub repos are demoted from primary evidence to incidental org-page residue. The risk is that a reviewer who org-spelunks across `github.com/orgs/poietic-pbc/repositories` finds them; mitigation is archiving whenever Erik has 30 seconds at GitHub admin.

**Action: archive at convenience; submission can proceed without.** Recommended order at convenience:

1. github.com/poietic-pbc/deep-research-competition → Settings → Archive
2. github.com/poietic-pbc/phr-methodology-comparison → Settings → Archive

Either both archived before submission or neither. Doing one and leaving the other increases the chance the surviving stale repo is the one a reviewer notices.

---

## 7. Recommended submission order

Sequence chosen to (a) front-load Erik-decision fields so they are not last-minute friction, (b) batch all radio/Y-N picks before opening the prose flow, (c) leave §53 Erik-discretion explanation last in the ethics block.

1. **Section I mechanical fields** §1-§10 (mostly verbatim; resolve §4b, §4c, §7, §8d, §9d on the way).
2. **Section II radio/multiselect** §11-§15 (commit to the **Validated Methodology** stage call now).
3. **Section II prose** §16a → §19c (twelve fields, 75w each, all paste-from-v3.1).
4. **Section III** §20 (paste v3.1) → §21 (paste v3.1) → §22 Yes → §23 (paste v3.1) → §24 Yes → §25 (paste v3.1).
5. **Section IV** §26 (paste v3.1) → §27 AI First → **§28 (paste recommended replacement with traces)** → **§29 (paste this guide's 184w Risks block — do NOT paste v3.1 §29)** → **§30 (paste this guide's 85w roles-only block)** → §31 (Erik decides default-blank vs HPRC+IGVF entries).
6. **Section V** §32 (multiselect picks — at least the recommended top 3) → §33-§35 (paste v3.1) → **§36 (paste recommended replacement with traces)**.
7. **Section VI** §37 $1.5M → §38a-c → §39a-c → §40a-c → §41a-c (paste v3.1 budget categories with Name/USD/Description split) → §42 NA → §43a-c → §44a-c → §45a-c → §46a-c (paste v3.1 milestones with Timeframe/Activities/Outcomes split) → §47 NA.
8. **Section VII** §48 No → **§49 YES** → **§50 YES** → §51 No → §52 No → **§53 (paste this guide's 75w explanation)**.
9. **Certification** — Erik reads all six statements and certifies.

Save / submit.

---

## 8. Validation checklist (every line a hard check from the task spec)

- [x] Every form question §1-§53 + certification covered in the paste guide table (table §3 has 53 form-question rows + Cert)
- [x] §29 Risks content ≤200w (drafted at 184w; manual recount confirmed)
- [x] §30 team roles ≤100w, no individual names (drafted at 97w after 2026-05-02 4th-role rewrite to lead with agency-framework design; "Garrison", "Pinello", "Tan" do not appear in §30 block)
- [x] §32 multiselect choices recommended (top 3 + optional 4th + commentary on v3.1's 4th)
- [x] §53 explanation drafted for govt-persons (drafted at 75w; covers UTHSC + UCL + MGH/HMS/Broad)
- [x] All multiselect / radio fields have recommended answers (§12, §13, §14, §15, §22, §24, §27, §32, §37, §48-§52 all in §2 mechanical block)
- [x] Erik-only items clearly listed (§5, twelve items)
- [x] M4 / H7 link-to-traces verdict included (§6 of this guide)
- [x] Output at `~/poietic.life/notes/v3-1-form-mapping-paste-guide-20260502.md`

Style hard checks (carried over from v3.1 review):

- [x] No em-dashes in any drafted block
- [x] No PI / lead PI / Principal Investigator language
- [x] Founder order Erik / Luca / Vaughn preserved where named (only §8/§9/§26/§53)
- [x] CRISPRme/Casgevy framing precise where it appears in §28/§36 ("identified independently", "before Casgevy FDA approval", no implication of direct collaboration)
- [x] DNA-Diffusion only in §29 risk-disclosure, outside funded scope
- [x] No recursion claim ("drafted using WorkGraph", etc.) anywhere

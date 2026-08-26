# Digital Thermometers

**Type:** Diagnostic (device — evaluated with agreement/accuracy metrics, NOT drug-efficacy language)
**Category:** Diagnostics
**Verification Status:** AI-compiled from primary sources, unverified — not yet reviewed by a pharmacist/physician
**Evidence Grade:** Moderate — real pooled meta-analytic data exists for tympanic and temporal artery methods, and both are consistently found less accurate than rectal (reference-standard) thermometry, not merely "different"
**Last updated:** 2026-08-26
**Sources:** raw/primary-sources/digital-thermometers/pubmed-geijer-2016-temporal-artery-meta-analysis.md, raw/primary-sources/digital-thermometers/pubmed-shi-2020-tympanic-pediatric-meta-analysis.md, raw/primary-sources/digital-thermometers/nokc-2009-thermometry-review.md

---

## What This Page Is
Thermometer performance is evaluated by agreement with a reference thermometer (rectal/core temperature) at a given measurement site, not by a drug-style efficacy percentage. **Key distinction: a device's stated display resolution (e.g., 0.1°F increments) is not the same as its true accuracy against a reference standard** — a meter can display fine increments while still having a much wider real error margin.

## Efficacy/Accuracy Evidence (accuracy-metric framing)

**Temporal artery thermometers — Geijer et al. 2016 (PMID 27033957, BMJ Open):** 37 articles, 5,026 participants, vs. core-temperature reference methods:
- Pooled mean difference: **-0.19°C** (95% limits of agreement -1.16 to +0.77°C) — a wide scatter, moderate-quality evidence
- Pooled sensitivity for fever detection: **0.72** (95% CI 0.61–0.81)
- Pooled specificity: **0.94** (95% CI 0.87–0.97)
- Trend toward UNDERESTIMATING temperature specifically in febrile patients — the group where accuracy matters most clinically
- **Authors' conclusion: temporal artery thermometers are NOT sufficiently accurate to replace rectal/bladder/invasive reference methods**, and perform similarly to (i.e., no better than) tympanic thermometers — "both methods are inaccurate" in the authors' own words

**Tympanic thermometers, pediatric — Shi et al. 2020 (PMID 32398036, BMC Pediatr):** 12 studies, 4,639 pediatric patients, cutoffs tested from 37.0–38.0°C:
- Optimal cutoff identified: **37.8°C**, with sROC AUC **0.97** and Youden Index **0.83** at that cutoff
- (Note: the exact pooled sensitivity/specificity percentage pair at this optimal cutoff was not confirmed from the PubMed abstract text in this pass — only AUC and Youden Index are cited here; a WebSearch-only-sourced pair of ~92%/91% was seen but is not independently confirmed against the primary abstract, so it is deliberately omitted rather than asserted as fact)
- Conclusion: new-generation tympanic thermometry has high diagnostic accuracy for pediatric fever screening at the 37.8°C cutoff specifically — a different (and more favorable) picture than older tympanic-thermometer literature

**Older background (NOKC 2009 report, Norwegian government HTA, hosted on NCBI Bookshelf):** an earlier systematic review (11 studies, N=1,426, adult hospitalized patients) found infrared tympanic thermometry did NOT identify an acceptable proportion of fever cases detected by rectal thermometry (low sensitivity) despite high specificity — i.e., older-generation tympanic thermometers tend to under-detect fever rather than over-detect it. This is consistent with the newer literature's overall message that tympanic/temporal methods trade sensitivity for specificity relative to rectal reference, though device generation and cutoff choice matter a great deal (see Shi 2020 above, which is notably more favorable for newer devices at the right cutoff).

## What to Measure and Why
Agreement with a reference (usually rectal) thermometer; measurement site (oral / axillary / rectal / tympanic / temporal — not interchangeable, can give systematically different readings for the same true body temperature); sensitivity/specificity for fever detection at a stated cutoff; and the cutoff temperature itself, which meaningfully changes reported accuracy (see Shi 2020: 37.8°C performed best among tested cutoffs in children).

## Special Notes
- Different measurement sites are not interchangeable and must always be recorded alongside any reading or accuracy claim — site-swapping a "normal" reading from one method to another's threshold can create a false reassurance or false alarm.
- Across both major methods reviewed here (temporal and tympanic), the consistent finding is that non-invasive/non-rectal methods are less accurate than rectal reference, with tympanic accuracy in particular improving in newer-generation devices used at well-chosen cutoffs (Shi 2020) but historically weak per older literature (NOKC 2009).
- No axillary- or oral-specific pooled accuracy data with hard numbers was located in this pass.

## Pharmacy Times Context (recommendation share — NOT efficacy)
Per this database's own subcategory file (Pharmacy Times 2026 OTC Guide, ~1,700 pharmacists surveyed): **Braun ThermoScan — 50%** (a tympanic thermometer — see Shi 2020 / NOKC 2009 above), **Vicks — 22%**, **Safety 1st — 17%**, **Exergen — 9%** (a temporal artery thermometer — see Geijer 2016 above), **MOBI — 2%** of Digital Thermometer recommendations (1,189,286/month category volume). These are pharmacist recommendation shares, not accuracy rankings — the market-leading brand (Braun ThermoScan, tympanic) is not thereby shown to be the most accurate; that depends on device generation and cutoff, per the evidence above.

---

## Brands Using This Category (in this database — formulation not individually verified per SKU)
Brand-page research (2026-08-26) has since located brand-specific data for four of the five brands: **Braun ThermoScan** (tympanic, 50% share) — best-in-class head-to-head accuracy found (0.044°C mean error vs. gold standard) plus a strong pediatric reliability study, more favorable than the general tympanic literature above might suggest on its own; **Exergen** (temporal artery, 9%) — directly and specifically covered by the Geijer 2016 review already cited above, since Exergen is essentially the commercial embodiment of that technology; **Vicks** (22%, digital oral-type per its FDA 510(k) filing) — a real pivotal non-inferiority clinical study (165 subjects) found equivalence to a Welch Allyn reference device across all age groups and specifically in febrile subjects; **MOBI** (2%, infrared forehead) — measured in the same head-to-head study as Braun, showing meaningfully worse agreement (-0.184°C mean error) and reduced sensitivity to real temperature change. **Safety 1st** (17%) remains without any located brand-specific study — a genuine gap; the closest available evidence is a class-level non-contact-infrared-thermometer study finding 48-88% of readings outside labeled accuracy across six unnamed commercial models, not confirmed as including this brand. See each brand's own `drugs/*.md` page for full detail and sourcing.

## Related
- [[pharmacy overview]]

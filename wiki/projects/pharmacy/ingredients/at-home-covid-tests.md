# At-Home COVID Tests

**Type:** Diagnostic (device — evaluated with diagnostic-performance metrics, NOT drug-efficacy language)
**Category:** Diagnostics (rapid antigen self-tests)
**Verification Status:** AI-compiled from primary sources, unverified — not yet reviewed by a pharmacist/physician
**Evidence Grade:** Moderate-to-high for the antigen-test class as a whole (large pooled datasets exist), but performance is brand/timing/population-specific — no single accuracy number applies to "at-home COVID tests" generally
**Last updated:** 2026-08-26
**Sources:** raw/primary-sources/at-home-covid-tests/cochrane-dinnes-2022-antigen-accuracy.md, raw/primary-sources/at-home-covid-tests/pubmed-cai-2024-self-test-meta-analysis.md, raw/primary-sources/at-home-covid-tests/cadth-rapid-antigen-considerations.md

---

## What This Page Is
Diagnostic devices are evaluated on a different evidence schema from drugs: sensitivity, specificity, PPV, NPV, likelihood ratios, false-positive/negative rate, limit of detection, agreement with a reference standard (usually RT-PCR), time to result, and performance broken out by symptomatic vs. asymptomatic status and by brand — never a single blanket "accuracy" percentage.

## Mechanism
Antigen tests are lateral-flow immunoassays that detect SARS-CoV-2 nucleocapsid protein in an anterior nasal swab sample, typically producing a result in under 30 minutes (vs. one or more days for lab-based PCR). They are highly specific but less sensitive than molecular (PCR) tests, meaning a positive result is highly trustworthy but a negative result does not rule out infection.

## Efficacy Evidence (accuracy-metric framing)

**Cochrane review (Dinnes et al. 2022, PMID 35866452)** — 155 study cohorts, 100,462 samples, 16,822 confirmed cases, 49 commercial antigen assays:
- Sensitivity, symptomatic: **73.0%** (95% CI 69.3–76.4%)
- Sensitivity, asymptomatic: **54.7%** (95% CI 47.7–61.6%)
- Sensitivity, first week of symptoms: **80.9%** (95% CI 76.9–84.4%) vs. second week: **53.8%** (95% CI 48.0–59.6%)
- Specificity: **99.1%** symptomatic, **99.7%** asymptomatic
- By brand: sensitivity ranged **34.3–91.3%** (symptomatic) and **28.6–77.8%** (asymptomatic) across individually evaluated assays — only 7 of 20 assays met the WHO's ≥80% sensitivity bar for symptomatic testing
- PPV illustration: at 5% prevalence (symptomatic, week 1), PPV ≈89% (~1 in 10 positives false, ~1 in 5 cases missed); at 0.5% prevalence (asymptomatic), PPV only 38–52%

**Self-testing-specific meta-analysis (Cai et al. 2024, PMID 39494084)** — 45 studies, 50,897 patients, fully self-performed antigen tests vs. RT-PCR: pooled sensitivity **77%**, specificity **~100%**, diagnostic odds ratio 625.95. Higher sensitivity observed with Abbott Panbio assays, self-collected nasal (vs. other) swabs, and higher viral load (lower PCR Ct cutoff) at time of testing.

**Bottom line:** these two independent pooled analyses roughly agree — sensitivity in the 55–80% range depending heavily on symptom status/timing, with consistently high (~99–100%) specificity. No single ingredient-style "efficacy grade" applies; performance must be read by population and timing, not as one number.

## What to Measure and Why (per CADTH review)
Performance depends on variant, viral load, symptom timing, vaccination status, specimen type, test generation, and the comparator PCR assay's Ct cutoff. Serial testing (repeating over several days) is recommended specifically because single-test sensitivity is limited — this is a designed-in mitigation, not an incidental detail. Combined nasal + throat sampling produced higher detection rates than nasal-only sampling in cited literature, though FDA-authorized home tests are nasal-only.

**Required fields for any specific product/study record:** reference standard, sample type, population (symptomatic vs. asymptomatic), sensitivity, specificity, PPV, NPV, LR+/LR−, limit of detection, time to result, device version/manufacturer, study date, and circulating variant at time of study. Correct storage format: "Test X: sensitivity X%, specificity Y%, population Z, vs. reference standard Q, period D" — never a blanket "rapid tests are 80% accurate."

## Key Safety / Usability Data
- Real-world accessibility barriers (CADTH): manual dexterity and vision requirements for self-administration; nasal swab discomfort was the most commonly cited barrier to use; cost ($19.99–$46/package in the cited Canadian market data); temperature storage constraints (2–30°C); instruction-language and distribution-access barriers for vulnerable populations.
- A 2021 German study cited in the CADTH review found over a quarter of participants doubted test validity, particularly for negative results — a real adherence/trust consideration for an at-home product.
- False-negative risk rises the longer a person has had symptoms (viral load declines) and is higher in asymptomatic testing generally — both are inherent to antigen-test biology, not a defect of any one brand.

## Special Notes
- Symptomatic vs. asymptomatic testing populations must be tracked separately — performance in each group is not interchangeable, per both pooled sources above.
- A sensitivity figure from an earlier study period/variant should not be assumed to hold for later variants — none of the sources gathered here provide variant-stratified data, which is itself a real gap.

## Pharmacy Times Context (recommendation share — NOT efficacy)
No dedicated at-home-COVID-test brand-share category was found among this database's Pharmacy Times subcategory files in this pass — no percentage is invented here.

---

## Brands Using This Category (in this database — formulation not individually verified per SKU)
Brand-page research (2026-08-26) has since pulled individual EUA/independent-study performance data for all five brands in this category: **BinaxNOW** (53% share) — 91.7% sensitivity manufacturer study vs. 67.6% independent rural-population study; **FlowFlex** (33%) — 93% sensitivity manufacturer study, no independent study located; **CareStart** (8%) — 88.4% sensitivity manufacturer study vs. as low as 49.0% in independent asymptomatic-heavy community testing, the largest documented manufacturer-vs-independent gap in this category; **Ellume** (4%) — strong initial 96%/91% sensitivity (symptomatic/asymptomatic) but subject to a **Class I FDA recall** affecting ~2 million kits for an elevated false-positive rate from a manufacturing defect; **iHealRapid/iHealth** (2%) — 94.3% sensitivity / 98.1% specificity in a lay-user study. See each brand's own `drugs/*.md` page for full detail and sourcing. This confirms the point already made above: manufacturer-reported sensitivity is consistently higher than independent real-world figures, sometimes dramatically so.

## Related
- [[pharmacy overview]]
- [[blood-glucose-monitors]]
- [[digital-thermometers]]

# Kidney Disease — OTC Decision Guide

**Type:** Analysis (special-population synthesis)
**Verification Status:** AI-compiled from primary sources, unverified — not yet reviewed by a pharmacist/physician
**Last updated:** 2026-08-28
**Sources:** Synthesized entirely from the "Special Population Flags," "Contraindications," and "Dosing" sections already sourced across `ingredients/*.md` pages in this database. No new primary research was performed for this page — every judgment below traces to a specific ingredient page, linked inline.

---

## How to read this page

Same structure as [[pregnancy]] and [[breastfeeding]]. Kidney disease is unusual among the populations covered in this layer because the risk is frequently **dose-dependent and threshold-based** (a specific CrCl/eGFR cutoff) rather than a flat avoid/allow — so several entries below carry a specific number rather than a general caution. This page is not a substitute for a nephrologist's or pharmacist's guidance, especially since actual kidney function (not just a diagnosis label) determines most of the thresholds cited here.

---

## Tier 1 — Generally considered safe / no dose adjustment typically needed

| Ingredient | Note | Source |
|---|---|---|
| [[loperamide]] | No dose adjustment needed across mild-to-severe renal impairment | [[loperamide]] |
| [[dextromethorphan]] | No dose adjustment advised per manufacturer label (though severe renal disease is a contraindication) | [[dextromethorphan]] |
| [[peg-3350]] | No specific dose-adjustment guidance in manufacturer labeling; minimal systemic absorption | [[peg-3350]] |
| [[bisacodyl]] | May help reduce elevated potassium in advanced CKD, but requires careful electrolyte monitoring — a real, if narrow, potential benefit rather than pure neutrality | [[bisacodyl]] |
| [[simethicone]] | Zero systemic absorption mechanistically rules out kidney injury as a concern | [[simethicone]] |

---

## Tier 2 — Dose-adjust or use with caution at specific kidney-function thresholds

| Ingredient | Threshold / adjustment | Source |
|---|---|---|
| [[acetaminophen]] | Severe impairment (CrCl ≤30 mL/min): extend dosing intervals, reduce total daily dose | [[acetaminophen]] |
| [[famotidine]] | CrCl <50 mL/min: reduce dose 50% or extend interval to 36–48h; half-life extends from 2.5–3.5h to **>20h** at CrCl <10 mL/min, raising CNS adverse-effect risk; 2023 Beers Criteria also flags dose reduction at CrCl <50 mL/min in elderly patients specifically | [[famotidine]] |
| [[naproxen]] | No adjustment needed if CrCl ≥30 mL/min; **not recommended if CrCl <30 mL/min** | [[naproxen]] |
| [[ibuprofen]] | eGFR-based dosing limits apply (see the ingredient page's own dosing table) | [[ibuprofen]] |
| [[second-generation-antihistamines]] (cetirizine) | Reduce to 5mg/day for CrCl 11–31 mL/min or hemodialysis (age ≥12) | [[second-generation-antihistamines]] |
| [[bismuth-subsalicylate]] | Use the lowest effective dose for the shortest feasible period — salicylates may worsen renal function | [[bismuth-subsalicylate]] |
| [[melatonin]] | Caution in dialysis patients specifically, due to impaired elimination | [[melatonin]] |
| [[proton-pump-inhibitors]] | Kidney disease appears among StatPearls' own list of long-term-use associations that have **not** been confirmed in prospective studies (isolated observational links, significant confounding) — a real, unresolved question, not an established harm; kidney transplant patients specifically warrant magnesium-level monitoring during PPI therapy | [[proton-pump-inhibitors]] |

---

## Tier 3 — Avoid, or avoid without explicit medical direction

| Ingredient | Why | Source |
|---|---|---|
| [[aspirin]] | Avoid if CrCl <10 mL/min (general OTC pain/fever dosing) — though KDIGO guidance supports *low-dose* aspirin specifically for secondary ASCVD prevention in CKD patients with established cardiovascular disease, a distinct, medically-supervised use case from OTC pain/fever dosing (see [[pregnancy]]'s own analogous low-dose-aspirin carve-out) | [[aspirin]] |
| [[magnesium-hydroxide]] | **Should be avoided by CKD/dialysis patients unless specifically physician-directed** — real, documented, sometimes-fatal hypermagnesemia case reports exist because the kidneys cannot clear a laxative-dose magnesium load; contraindicated for anyone with impaired renal function per the ingredient's own Contraindications section | [[magnesium-hydroxide]] |
| [[phenazopyridine]] | Contraindicated below GFR 50 | [[phenazopyridine]] |
| [[sodium-phosphate]] | Real, FDA-documented acute kidney injury risk ("acute phosphate nephropathy") from calcium-phosphate crystal deposits in renal tubules — serious enough to prompt two FDA safety communications (2006, 2014) and a 2008 boxed warning on related prescription bowel-prep products. **Diabetes, age over 65, dehydration, and concurrent NSAID/ACE-inhibitor/ARB/diuretic use are specifically named risk-amplifying factors** — several of which co-occur with CKD itself | [[sodium-phosphate]] |
| [[guaifenesin]] | Severe kidney disease is a specific contraindication (separate from its unrelated kidney-stone-history contraindication) | [[guaifenesin]] |

---

## The NSAID-class risk, stated once for the whole class

Ibuprofen, naproxen, and aspirin all reduce renal blood flow via the same COX-inhibition mechanism — this is a **class-wide** NSAID concern, not specific to one molecule, and it compounds with existing kidney disease rather than acting independently of it. Per [[oral-pain-relievers]], ibuprofen carries a cited NNH of 5.5 for acute kidney injury even in healthy (dehydrated) individuals — a real signal that pre-existing CKD would only be expected to worsen. **Acetaminophen is the NSAID-avoiding option for pain/fever in kidney disease**, subject to its own dose-interval extension at CrCl ≤30 mL/min above.

---

## Bottom lines

1. **Pain/fever with kidney disease:** acetaminophen (with dose-interval extension at CrCl ≤30 mL/min) is generally preferred over the NSAID class (ibuprofen, naproxen, aspirin), which all reduce renal blood flow and carry specific CrCl cutoffs below which they're not recommended or should be avoided.
2. **Heartburn/GERD:** famotidine needs real dose reduction as kidney function declines (50% reduction or extended interval at CrCl <50 mL/min) — this is not optional at advanced impairment given the dramatic half-life extension (>20h at CrCl <10 mL/min).
3. **Constipation:** **avoid magnesium hydroxide (Milk of Magnesia) in CKD/dialysis without physician direction** — this is the single sharpest, most consequential avoid-flag in this entire page, given real documented fatal case reports. PEG 3350 and bisacodyl are the safer laxative choices in this population per the sources reviewed.
4. **Never use an oral sodium phosphate bowel-prep product without medical supervision if you have any kidney risk factor** — the FDA's own two safety communications and boxed-warning history on related prescription products make this one of the more serious avoid-flags in this database generally, not specific to CKD alone.
5. **Allergies:** cetirizine needs a real dose reduction (5mg/day) at CrCl 11–31 mL/min or on hemodialysis.
6. **When in doubt, actual kidney function (a real CrCl/eGFR number) matters more than a diagnosis label** — several of the thresholds above are specific numeric cutoffs, not blanket avoid-if-CKD rules, so a pharmacist or nephrologist consult that accounts for the individual's actual lab values will be more precise than this page's category-level synthesis.

## Related
- [[pregnancy]]
- [[breastfeeding]]
- [[oral-pain-relievers]]
- [[famotidine]]
- [[magnesium-hydroxide]]
- [[sodium-phosphate]]
- [[red-flags]]
- [[pharmacy overview]]

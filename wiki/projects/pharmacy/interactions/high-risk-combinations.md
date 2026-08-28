# High-Risk OTC Combinations

**Type:** Analysis (curated interaction synthesis)
**Verification Status:** AI-compiled from primary sources, unverified — not yet reviewed by a pharmacist/physician
**Last updated:** 2026-08-28
**Sources:** Curated entirely from the "Drug Interactions" and "Key Safety Data" sections already sourced across `ingredients/*.md` pages in this database — no new primary research performed for this page. See `README.md` in this folder for why this page is curated rather than an exhaustive pairwise matrix.

---

## How to use this page

This is not a list of every possible OTC interaction — it's the real-world-common, high-consequence combinations that surfaced repeatedly during this database's ingredient-by-ingredient research, organized by mechanism so the underlying logic (not just a memorized pair) transfers to similar situations. For the full sourced detail behind any entry, follow the ingredient link.

---

## 1. Acetaminophen duplicate-dosing (the single most common real-world OTC overdose mechanism)

**The risk:** acetaminophen hides inside far more products than its name suggests — plain Tylenol, Tylenol PM, Tylenol 8HR Arthritis, all three Excedrin variants, BC Max, Goody's Powder, and many cold/flu combination products. Taking two of these on the same day, without recognizing they share the same active ingredient, is explicitly named in this database's [[acetaminophen]] page as **a leading real-world cause of unintentional overdose** — contributing to an estimated ~500 US deaths/year and ~50,000 ED admissions/year.

**The rule:** never combine two different acetaminophen-containing products, full stop — check every label, not just the brand name. See [[substitutions-and-duplicates]] Section C for the full list of where acetaminophen hides, and [[red-flags]] Section 4 for the liver-injury symptoms this can cause.

**Source:** [[acetaminophen]]

---

## 2. NSAID stacking (ibuprofen + naproxen + aspirin, in any combination)

**The risk:** ibuprofen, naproxen, and aspirin are all NSAIDs sharing the same COX-inhibition mechanism and the same class of risks — GI bleeding, kidney injury, and (per FDA boxed warning language on ibuprofen/naproxen) cardiovascular events. Taking two different NSAID-containing products at once (e.g., a plain NSAID during the day plus a "PM" combination product like Advil PM or Aleve PM at night, without recognizing both contain an NSAID) compounds these risks without adding meaningfully more pain relief.

**The rule:** use only one NSAID at a time. Aspirin's own [[aspirin]] page lists "**corticosteroids, other NSAIDs:** synergistic GI bleeding/ulceration" as a specific, sourced interaction.

**Source:** [[ibuprofen]], [[naproxen]], [[aspirin]]

---

## 3. Ibuprofen blocking low-dose aspirin's cardioprotective effect

**The risk:** this is a real, quantified pharmacokinetic interaction, not a general class-stacking concern. Ibuprofen and aspirin compete for the same binding site on platelet COX-1. If ibuprofen is taken too close to a daily low-dose aspirin dose, it can block aspirin's intended antiplatelet (cardioprotective) effect:

| Timing | Platelet inhibition (aspirin's effect) | Interaction present? |
|---|---|---|
| Ibuprofen 2h *before* aspirin | 53% | Yes — meaningfully blunted |
| Ibuprofen 8h *before* aspirin | 90.7% | Reduced |
| Ibuprofen 2h *after* aspirin | 99.2% | No — full effect preserved |
| Ibuprofen 400mg TID, timed 1h/7h/13h post-aspirin | 98.3% mean inhibition | No |

**The rule:** if you take daily low-dose aspirin for heart protection, dose any ibuprofen at least 2 hours *after* your aspirin — or use acetaminophen for occasional pain relief instead, since it does not compete for the same binding site. See [[oral-pain-relievers]] for the full comparison this feeds into.

**Source:** [[ibuprofen]]

---

## 4. Warfarin (or other anticoagulants) + NSAIDs or aspirin

**The risk:** per [[ibuprofen]], ibuprofen does not significantly affect warfarin's PT/clotting-factor activity directly in controlled studies — but **combined GI bleeding risk is synergistic (higher than either drug alone)**. Aspirin's own page separately lists anticoagulants (warfarin, heparin) and antiplatelets (clopidogrel, dipyridamole) as carrying a synergistic bleeding risk, and acetaminophen itself is not risk-free here either: prolonged use at 4000mg/day is associated with elevated INR, meaning warfarin monitoring frequency should increase even with the "safer" analgesic choice.

**The rule:** anyone on warfarin or another anticoagulant should treat any regular NSAID or aspirin use as a real bleeding-risk multiplier, and should not assume acetaminophen is entirely interaction-free either (increase INR monitoring with sustained high-dose use).

**Source:** [[ibuprofen]], [[aspirin]], [[acetaminophen]]

---

## 5. Serotonergic combinations with dextromethorphan

**The risk:** dextromethorphan is metabolized through a pathway that interacts seriously with drugs affecting serotonin. Per [[dextromethorphan]]:
- **MAOIs** (or within 2 weeks of stopping one): **contraindicated** — major serotonin syndrome risk.
- **SSRIs, SNRIs, TCAs:** increased serotonin syndrome risk (a real risk even outside the MAOI-specific contraindication).

**The rule:** check for any antidepressant use before recommending a dextromethorphan-containing cough suppressant — this is not limited to the well-known MAOI warning printed on the label.

**Source:** [[dextromethorphan]]

---

## 6. MAOIs + oral decongestants (pseudoephedrine, oral phenylephrine)

**The risk:** both oral decongestants are sympathomimetics. Combined with an MAOI (or within 2 weeks of stopping one), the risk is a hypertensive crisis — this is a flat **contraindication** on both labels, not a "use caution" note.

**The rule:** always ask about current or recent (within 2 weeks) MAOI use before recommending either decongestant. See [[nasal-decongestants]] for the fuller comparison these two sit inside.

**Source:** [[pseudoephedrine]], [[oral-phenylephrine]]

---

## 7. Aspirin's other real, sourced interactions worth flagging individually

Beyond the anticoagulant/NSAID risks above, [[aspirin]]'s own Drug Interactions section documents several specific, less-obvious combinations:
- **Methotrexate:** decreased renal MTX clearance, increased toxicity — avoid combination.
- **SSRIs:** synergistic upper GI bleeding risk (platelet serotonin depletion plus aspirin's own GI effect) — a second, GI-specific reason (beyond dextromethorphan's serotonin-syndrome risk above) that antidepressant use matters when recommending OTC products.
- **Digoxin, lithium:** aspirin reduces renal clearance of both — monitor levels. (Ibuprofen carries a related, separately-quantified lithium interaction: plasma lithium ↑15%, renal clearance ↓19% in one cited study.)
- **ACE inhibitors, diuretics:** increased acute-kidney-injury risk — a combination also documented independently on [[ibuprofen]] and, for a mechanistically different reason (phosphate/fluid shift), on [[sodium-phosphate]].
- **Valproate, phenytoin:** aspirin displaces both from protein binding — monitor free phenytoin levels specifically.

**Source:** [[aspirin]]

---

## 8. Loperamide + P-glycoprotein inhibitors (cardiotoxicity risk multiplier)

**The risk:** loperamide's safety at OTC doses depends on P-glycoprotein keeping it out of the brain and away from cardiac tissue. Drugs that inhibit P-gp raise loperamide's CNS penetration and cardiotoxicity risk — directly relevant given loperamide's own FDA Boxed Warning for torsades de pointes/sudden death at high exposure. Per [[loperamide]], P-gp inhibitors include: **amiodarone, carvedilol, ritonavir, quinidine, itraconazole, verapamil, clarithromycin, ranolazine.** Lonafarnib (a CYP3A4 inhibitor) separately raises loperamide levels enough that the label recommends limiting loperamide to 1mg/day initially if combined.

**The rule:** anyone on one of these heart-rhythm or antifungal/antiviral medications should be cautious about even labeled-dose loperamide use, not just abuse-level dosing.

**Source:** [[loperamide]]

---

## 9. Salicylate stacking (aspirin + bismuth subsalicylate)

**The risk:** aspirin and bismuth subsalicylate (Pepto-Bismol, Kaopectate) are both salicylates. Taking an aspirin-containing pain reliever (including Excedrin/BC Powder/Goody's Powder, all aspirin-containing per [[aspirin]]) while also using Pepto-Bismol or Kaopectate for stomach upset compounds salicylate exposure — relevant both to general salicylate-toxicity risk and, in children/teens with a viral illness, to Reye syndrome risk (see [[red-flags]] Section 8).

**Source:** [[aspirin]], [[bismuth-subsalicylate]], [[substitutions-and-duplicates]]

---

## 10. St. John's Wort (mood/herbal supplements) + common prescription drug classes

**The risk:** per [[mood-health-supplements]], St. John's Wort should not be combined with SSRIs/SNRIs/MAOIs (serotonin syndrome risk) or with CYP3A4/P-glycoprotein-substrate medications — which includes hormonal contraceptives, anticoagulants, and other antidepressants — without physician guidance, since it can reduce their effectiveness via enzyme induction.

**Source:** [[mood-health-supplements]]

---

## 11. Sodium phosphate enemas + NSAIDs, ACE inhibitors, ARBs, or diuretics

**The risk:** per [[sodium-phosphate]], concurrent use of any of these four drug classes is an FDA-identified risk factor for acute phosphate nephropathy — all four reduce the kidney's ability to handle the phosphate/fluid-shift load a sodium phosphate enema imposes.

**Source:** [[sodium-phosphate]]

---

## 12. First-generation antihistamines/anticholinergics + alcohol or other sedatives

**The risk:** diphenhydramine and doxylamine (Benadryl, Unisom SleepGels, ZzzQuil, and the "PM" combination analgesics) both carry label instructions against combining with alcohol or other sedatives (additive CNS depression), and against combining with any other diphenhydramine- or doxylamine-containing product (additive anticholinergic/sedative risk — see [[substitutions-and-duplicates]] Section C for where these hide). Cetirizine (Zyrtec/Xyzal) carries a related but smaller-magnitude version of this same risk with CNS depressants (alcohol, benzodiazepines, opioids) despite being a second-generation, less-sedating agent.

**Source:** [[oral-diphenhydramine-sleep-aid]], [[doxylamine]], [[second-generation-antihistamines]]

---

## Related
- [[README]]
- [[substitutions-and-duplicates]]
- [[red-flags]]
- [[oral-pain-relievers]]
- [[nasal-decongestants]]
- [[pharmacy overview]]

# Substitutions and Duplicate-Ingredient Safety

**Type:** Analysis (cross-cutting synthesis)
**Verification Status:** AI-compiled from primary sources, unverified — not yet reviewed by a pharmacist/physician
**Last updated:** 2026-08-28
**Sources:** Synthesized from confirmed findings already documented across `drugs/*.md` and `ingredients/*.md` during the brand-by-brand research phase — this page performs no new research, it aggregates.

---

## Why this page exists

Two opposite mistakes are common with OTC products, and this database has independently confirmed real examples of both across its 719-brand research pass:

1. **Paying more / switching brands for "something different" that is actually the identical formulation.** A consumer bouncing between two "competing" products may be buying the same drug twice, at the same dose, from the same or different manufacturers — not a safety problem by itself, but a real waste of money and a genuine risk if they don't realize the two together mean a doubled dose.
2. **Assuming a familiar brand name always means the same drug.** Several brand names in this database span two or more chemically unrelated active ingredients — sometimes for a legitimate line-extension reason (a "PM" variant, a kids' variant), sometimes because the FDA forced a whole-molecule swap (Zantac). Treating these as interchangeable is the more dangerous mistake.

A third, related pattern is **accidental duplicate-dosing**: taking two different-looking products that both happen to contain the same active ingredient (acetaminophen is the paradigm case), which is a leading real-world cause of unintentional OTC overdose. See [[red-flags]] for the emergency thresholds this can trigger, and `interactions/high-risk-combinations.md` for the specific pairwise mechanisms.

---

## Section A — Confirmed Identical Formulations (Different Brand Name, Same Drug)

These are cases where this database independently pulled DailyMed/FDA labels for two or more "competing" brands and found the same active ingredient(s) at the same dose. Buying the pricier one buys nothing pharmacologically different.

| Active ingredient(s) & dose | Brand names confirmed identical | Category | Notes |
|---|---|---|---|
| Bismuth subsalicylate 525mg/30mL | [[Pepto-Bismol]] = [[Kaopectate]] | Antidiarrheals / Upset Stomach / Nausea | Kaopectate's own name ("kao" + "pectin") is now chemically inaccurate — it was reformulated to bismuth subsalicylate in 2004 after a lead-contamination lawsuit over its prior attapulgite-clay formula. See [[bismuth-subsalicylate]]. |
| Docusate sodium 100mg | [[Colace]] = [[Phillips' Stool Softener]] = Dulcolax Stool Softener (part of the [[Dulcolax]] brand family) | Stool Softeners | Three separately marketed, separately priced brands selling the identical molecule and dose. Per [[docusate]]'s own Efficacy Controversy section, a 2021 review of 7 RCTs found docusate no better than placebo — a genuinely important caveat given one of these three is the category-dominant (61%) brand. |
| Dextran 70 0.1% + glycerin 0.2% + hypromellose 0.3% | [[GenTeal Tears]] (Moderate) = [[Tears Naturale]] | Artificial Tears/Ophthalmic Lubricants | Both manufactured by Alcon; GenTeal Tears was in fact the rebrand of the older "Tears Naturale Forte" line. Tracked as two separate Pharmacy Times brands despite being effectively sibling products. |
| Acetaminophen 250mg + aspirin 250mg + caffeine 65mg | [[Excedrin]] (Extra Strength) = Excedrin Tension Headache = [[Excedrin Migraine]] | Headache/Migraine Products | Identical triple-combination formulation sold under three different marketing names targeted at three different symptoms. Excedrin Migraine carries dedicated brand-specific RCT evidence (Lipton et al. 1998, PMID 9482363) that the other two names do not separately re-earn — same pill either way. |
| Ibuprofen 100mg/5mL | Children's Motrin = [[Children's Advil]] | Children's Analgesics | Identical concentration under two competing brand names. |
| Solubilized ibuprofen 200mg | [[Advil Migraine]] = [[Motrin Migraine]] | Migraine/Headache Products | Both labels state "Treats migraine" as an FDA-recognized Use. |
| Ibuprofen 200mg (standard) | [[Advil Easy Open Arthritis Cap]] = regular [[Advil]] | Oral Arthritis Pain Relievers | "Arthritis" here refers only to an accessible bottle-cap design (Arthritis Foundation Ease-of-Use Commendation) — not a different dose or extended-release formulation. Contrast with genuine reformulations below. |
| Acetaminophen 160mg/5mL | Children's Tylenol = Genexa Children's Acetaminophen | Children's Analgesics | Genexa differentiates only on "clean"/organic inactive ingredients and marketing — the active ingredient and dose are identical. |
| Famotidine 20mg | Pepcid AC Maximum Strength = [[Zantac 360°]] | H2 Receptor Antagonists | See Section B below — Zantac's brand history makes this pairing worth extra caution, not less. |

**Not a duplicate — a genuine reformulation (listed for contrast):** [[Tylenol 8 HR Arthritis Pain]] is a real bi-layer extended-release 650mg acetaminophen tablet (immediate + extended-release layers), mechanistically different from standard Tylenol — unlike Advil's "Arthritis" cap above, this one is not just packaging.

---

## Section B — Same Brand Name, Different (Sometimes Unrelated) Active Ingredient

The more dangerous trap: assuming brand-name familiarity guarantees the same drug. Check the product's actual Drug Facts panel, not just the name on the box.

| Brand name | Sub-product A | Sub-product B | Sub-product C | Why it matters |
|---|---|---|---|---|
| Zantac | Pre-2020 "Zantac" = **ranitidine** (withdrawn from market April 2020 over NDMA/carcinogen contamination) | [[Zantac 360°]] (2021 relaunch) = **famotidine**, chemically unrelated | — | The single most consequential same-brand-name-different-molecule finding in this database: the drug wasn't just reformulated, the original molecule was recalled entirely and the name was reused for a different one. A consumer's memory of "Zantac" from before 2020 does not describe what's on shelves today. See [[famotidine]]. |
| Unisom | SleepTabs = **doxylamine succinate** 25mg | SleepGels = **diphenhydramine HCl** 50mg | — | Two chemically distinct first-generation antihistamines sold as sleep aids under one brand. Both carry the same class-level AGS Beers Criteria "avoid in older adults" flag, so the safety takeaway is the same either way, but the molecules (and this database's own tracked 58% Unisom recommendation share) are not interchangeable data points. See [[doxylamine]] and [[oral-diphenhydramine-sleep-aid]]. |
| Vicks ZzzQuil | Standard ZzzQuil = **diphenhydramine HCl** 50mg | ZzzQuil Pure Zzzs = **melatonin** | — | Same brand family, two entirely different mechanisms (anticholinergic antihistamine vs. pineal hormone) — see [[oral-diphenhydramine-sleep-aid]] and [[melatonin]]. |
| Dramamine | Original Dramamine = **dimenhydrinate** | Dramamine Nausea (Non-Drowsy) = **meclizine** | — | Two chemically distinct antihistamines under one trusted motion-sickness brand name. See [[dimenhydrinate]] and [[meclizine]]. |
| Dulcolax | Core [[Dulcolax]] tablet = **bisacodyl** 5mg (stimulant laxative, onset 6–12h) | Dulcolax Stool Softener / Pink Stool Softener = **docusate sodium** 100mg (surfactant, onset 12–72h) | — | Different mechanism classes, different onset times, different evidence tiers (bisacodyl is FDA-approved and ACG/AGA-endorsed; docusate per [[docusate]] has no FDA-approved indication). A shopper grabbing "Dulcolax" without reading past the brand name may get a fundamentally different drug than intended. |
| Phillips' | Plain Phillips' (Milk of Magnesia) = **magnesium hydroxide** | Phillips' Stool Softener = **docusate sodium** | Phillips' Fiber Good = **inulin** (dietary-supplement fiber gummy) | Three genuinely different mechanisms under one family brand name — the most fragmented single-brand mechanism spread found in this database's laxative research. See [[magnesium-hydroxide]], [[docusate]], [[fiber]]. |
| Mederma | Mederma (Scar Treatments) = **allantoin** | Mederma Stretch Marks = **dimethicone 2%** | — | Same brand, two different actives for two different (if related-sounding) skin indications — do not assume the Scar Treatments evidence applies to the Stretch Marks product or vice versa. |
| Neosporin | Neosporin Original = **bacitracin zinc + neomycin sulfate + polymyxin B sulfate** (triple antibiotic) | Simply Neosporin = **bacitracin zinc + polymyxin B sulfate** (neomycin-free) | — | Simply Neosporin exists specifically for neomycin-allergic users. See [[Neosporin]] and [[topical-antibiotics]] — the two-ingredient version carries a meaningfully smaller allergy-risk surface (one fewer common contact allergen). |
| Bayer | Bayer Genuine Aspirin = **aspirin 325mg**, immediate-release, for acute pain/fever | Bayer Aspirin Regimen Low Dose = **aspirin 81mg**, enteric-coated, doctor-directed cardioprotection | — | Same active ingredient, meaningfully different dose and intended use under the same family brand — see also Ecotrin, which sells both an 81mg and 325mg tablet under its own single brand name for the same reason. Mixing these up (e.g., taking Low Dose thinking it will relieve acute pain, or taking Genuine Aspirin daily thinking it's the cardioprotective dose) is a real, easy mistake. See [[aspirin]]. |
| H2 Receptor Antagonists category | [[famotidine]]-based (Pepcid, Zantac 360°) | **cimetidine**-based (Tagamet HB 200) | — | Different molecules within the same drug class filed side-by-side in this database's category data — cimetidine is a notable CYP450 inhibitor with a real warfarin interaction that famotidine does not share to the same degree. Do not assume interaction profiles transfer across an entire Pharmacy Times category. |

---

## Section C — Duplicate-Dosing Risk: Different Products, Same Hidden Active Ingredient

Unlike Section A (where the products are marketed as equivalent), these are cases where a consumer would not necessarily expect two products to share an active ingredient — the risk is stacking without realizing it.

- **Acetaminophen is the single most important entry here.** Per [[acetaminophen]]: combination-product overlap (e.g., a Tylenol product plus an acetaminophen-containing cold/flu combo, PM sleep aid, or Excedrin-family product taken the same day) is a leading real-world cause of unintentional overdose, contributing to an estimated ~500 US deaths/year and ~50,000 ED admissions/year. Every acetaminophen-containing OTC label carries a "do not use with any other acetaminophen-containing product" warning for this exact reason. Acetaminophen hides inside: plain Tylenol variants, Tylenol PM, Tylenol 8HR Arthritis, Excedrin (all three names in Section A), BC Max, Goody's Powder, and many combination cold/flu products not individually re-verified in this pass.
- **Salicylate stacking.** Aspirin, bismuth subsalicylate (Pepto-Bismol/Kaopectate — Section A), and the Excedrin/BC Powder/Goody's Powder combination products (all aspirin-containing per [[aspirin]]) all deliver the same salicylate load. Someone taking Pepto-Bismol for an upset stomach while also taking aspirin or Excedrin for a headache is compounding salicylate exposure — relevant to both the Reye syndrome risk in children/teens with viral illness and general salicylate-toxicity risk (see [[red-flags]]).
- **NSAID stacking.** Ibuprofen ([[ibuprofen]]) and naproxen ([[naproxen]]) are both NSAIDs; Advil PM (ibuprofen) and Aleve PM (naproxen) are both "PM" combination products that a consumer might take at night while also taking a plain NSAID during the day, unintentionally exceeding the combined NSAID dose and raising GI-bleed/renal/cardiovascular risk without realizing they've doubled the drug class.
- **First-generation-antihistamine/anticholinergic stacking.** Diphenhydramine appears across oral sleep aids (Tylenol PM, Advil PM, Aleve PM, Unisom SleepGels, ZzzQuil) and topical products ([[topical-diphenhydramine]], e.g., anti-itch creams). Using an oral PM product and a topical diphenhydramine cream simultaneously adds to the same anticholinergic burden discussed on [[oral-diphenhydramine-sleep-aid]] (falls/delirium/confusion risk, especially in older adults per the AGS Beers Criteria).
- **Sodium loading in antacid/combination powders.** Original Alka-Seltzer delivers ~567mg sodium per tablet on top of its aspirin content — relevant to anyone also managing sodium intake for heart failure, kidney disease, or hypertension, and easy to miss since Alka-Seltzer is filed under Antacids/Nausea Remedies/Upset Stomach Remedies, none of which signal "contains aspirin" or "high sodium" by category name alone.

---

## How to use this page

This is a synthesis of findings already confirmed elsewhere in this database, not a substitute for reading the actual product label in hand — new brand-family surprises are still being found as brand-by-brand research continues, and this list is not asserted to be exhaustive. When in doubt, check the specific ingredient page (e.g., [[docusate]], [[acetaminophen]], [[famotidine]]) and the specific brand's own `drugs/*.md` page for the most detailed sourcing.

## Related
- [[red-flags]]
- [[pharmacy overview]]
- [[docusate]]
- [[acetaminophen]]
- [[bismuth-subsalicylate]]
- [[famotidine]]

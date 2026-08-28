# Interactions Layer — README

**Type:** Analysis (methodology note)
**Verification Status:** AI-compiled from primary sources, unverified — not yet reviewed by a pharmacist/physician
**Last updated:** 2026-08-28
**Sources:** This page is a methodology note, not a research page — it explains the design of this folder and reports an audit of existing `ingredients/*.md` "Drug Interactions" sections. No new primary research was performed.

---

## Why this folder is not a pairwise interaction matrix

This database has 122 ingredient pages. A complete pairwise interaction matrix would require roughly **122 × 121 / 2 ≈ 7,381 unique ingredient pairs** — each one needing its own independently sourced mechanism, severity, and citation to meet this project's sourcing bar (StatPearls, FDA labels, Cochrane, PubMed). That is not a feasible research task for a project of this scope, and attempting it would almost certainly produce either (a) thousands of thin, unsourced, or fabricated entries, which violates this project's core sourcing rule, or (b) an abandoned, permanently-incomplete grid that looks more authoritative than it is.

**Instead, this folder does two things:**

1. **`high-risk-combinations.md`** curates the specific, high-consequence, real-world-common interaction scenarios that had *already* surfaced organically during the ingredient-by-ingredient research phase — acetaminophen duplicate-dosing, NSAID stacking, the ibuprofen/aspirin timing interaction, MAOI combinations, and similar. These are not new research; they are aggregation of interactions this database's own contributors already found and sourced while building the 122 ingredient pages.
2. **This README** documents how each ingredient page's own "Drug Interactions" section is structured, so that a **pairwise lookup** — "does ingredient X interact with ingredient Y?" — can be done manually and reliably by opening both pages, rather than by trusting a pre-written master grid that cannot realistically stay complete or accurate at this ingredient count.

**In short: this layer is designed for lookup, not pre-computation.** If you need to check a specific pair not covered in `high-risk-combinations.md`, open both ingredients' own pages and read their "Drug Interactions" sections directly — see the audit below for what to expect when you do.

---

## Audit: how consistent is the "Drug Interactions" section across ingredient pages?

A sample of 12 ingredient pages was reviewed for structural consistency: [[ibuprofen]], [[naproxen]], [[aspirin]], [[acetaminophen]], [[loperamide]], [[famotidine]], [[second-generation-antihistamines]], [[dextromethorphan]], [[pseudoephedrine]], [[oral-phenylephrine]], [[guaifenesin]], [[iron]].

**Finding: every sampled page has a "Drug Interactions" section (or, in a small number of cases, interaction content folded into "Key Safety Data" or "Contraindications" instead — see below), and all of them use the same general format: a bulleted list, each bullet leading with the interacting substance or drug class in bold, followed by the mechanism and/or clinical consequence in prose.** For example:

> - **Aspirin (cardioprotective, low-dose):** ibuprofen blocks aspirin's antiplatelet effect if dosed too close together...
> - **MAOIs:** contraindicated — hypertensive crisis risk

**This format is consistent enough to scan quickly and cross-reference by eye**, but it is **not** a structured table with dedicated fields — meaning it does not currently have:
- A standardized **severity rating** (e.g., "contraindicated" vs. "monitor" vs. "minor" appears inconsistently as free text within the prose, not as a consistent tag or field)
- A **per-interaction citation** distinct from the page's overall sourcing — most interaction facts are drawn from the same StatPearls/FDA-label sources already listed in the page header, rather than each bullet carrying its own inline citation
- A machine-parseable structure (no consistent delimiter/table format across all 122 pages) — this matters if this database is ever used to programmatically cross-reference pairs (e.g., for the eventual local-AI training goal described in `pharmacy ai consultant.md`)

**A small number of pages fold interaction-relevant content into other sections instead of a dedicated "Drug Interactions" header** — e.g., [[guaifenesin]] lists its MAOI contraindication under Contraindications rather than a separate Interactions section, and [[iron]] lists its levodopa/levothyroxine/PPI interactions under a "Drug Interactions" header but with less structured detail than the NSAID pages. This means a pairwise lookup should check **Contraindications, Key Safety Data, AND Drug Interactions** on both ingredient pages, not assume all interaction-relevant content is filed under one heading.

**Recommendation for future work on this layer:** if this database is later revised for machine-readability (relevant to the stated local-AI training goal), retrofitting a consistent `| Interacting Substance | Severity | Mechanism | Source |` table onto each ingredient page's Drug Interactions section — as originally suggested for this layer — would be valuable and is a well-scoped, page-by-page task, distinct from (and much more tractable than) writing new pairwise combination pages from scratch.

## Related
- [[high-risk-combinations]]
- [[pharmacy overview]]

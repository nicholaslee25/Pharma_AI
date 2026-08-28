# Pharmacy AI Consultant

**Type:** Project
**Tags:** #project #education #family #ai
**Status:** Active — Phase 2 (Research) and Phase 2b (brand-level research, all 719 brands) both complete; entering RAG deployment planning
**Last updated:** 2026-08-28

---

## Overview

Started as "Pharmacy for Noobs" — an educational resource explaining medications, dosages, interactions, and pharmacy basics in plain language for non-medical people. Grew into something bigger: a full structured drug reference database ([[pharmacy overview]]), organized by category/subcategory/drug, sourced from the Pharmacy Times OTC Guide.

End goal: train a local AI on this data so family can ask it things like pros/cons, use cases, allergies, and symptoms for any OTC drug, at home, without needing a pharmacist on hand.

## Phases

1. **Organize** — done. Mirrors the OTC Guide's category structure, one file per subcategory with ranked brands + % pharmacist recommendation. One page per unique drug, stubbed for research.
2. **Research** — **complete.** The `ingredients/` layer under `projects/pharmacy/ingredients/` (110+ pages, grown from the original 77 as brand research surfaced whole categories with no ingredient page) carries real clinical evidence (study design, PMID/DOI, effect sizes, evidence grade) rather than just a recommendation percentage. Started from two ChatGPT-compiled evidence dossiers; those have since been deleted, along with the citation-index page that tracked their sourcing, now that every page has been rebuilt directly from primary sources (StatPearls, FDA labels via DailyMed, Cochrane, PubMed). All pages carry a **Verification Status** field (AI-compiled from real primary sources, unverified) — the sourcing work is done, but a real pharmacist/physician review pass to flip that field to "verified" is still outstanding and is the one remaining step before this phase's original "zero AI-compiled content, only real cited papers, verified against practitioners" goal is fully met.
2b. **Brand-level research** — **complete, 2026-08-28.** Every one of the 719 unique brand pages under `projects/pharmacy/drugs/` has now been individually researched (brand-specific FDA label where one exists, brand-specific trials where any exist, cross-checked against the shared `ingredients/` evidence page) and carries its own **Verification Status** field. This is the single largest data-quality upgrade to the drugs/ layer since it was first stubbed out in Phase 1 — every brand page now states plainly what is and isn't brand-specifically supported, rather than inheriting an assumed ingredient link. See [[pharmacy overview]] for the full category-by-category log of findings and new ingredient pages this phase produced.
3. **RAG deployment** — once the corpus is real-sourced and verified, wire it to a small local model (3B–8B open-weight) via retrieval, not fine-tuning first. This is deliberate: RAG lets you cite sources, fix errors without retraining, and is auditable — much safer for a health-info tool than baking facts into weights before they're confirmed correct.
4. **Fine-tune** — once the RAG-verified corpus is solid, it becomes the fine-tuning dataset (reshaped into instruction/Q&A pairs). Only training on data that's already been checked against real practitioners, not before.
5. **Deploy** — serve it, first for family, eventually as a shared server for others.

## Original Open Questions (from "Pharmacy for Noobs")

- Format: website, PDF, printed guide, app? → superseded by the local AI plan
- Scope: OTC meds only, or prescription too? — still open; starting OTC-only via the guide, prescription scope TBD
- What specifically confuses mom and dad most? — still need their input
- Audience: just family, or shareable publicly? — still open

## Next Step

Phases 1 (Organize), 2 (Research), and 2b (brand-level research, 719/719 brands) are all done. Next: either a pharmacist/physician verification pass over the ingredient and brand pages, or moving straight into Phase 3 (RAG deployment) planning. Talk to mom and dad about what confuses them most — that should shape what the AI prioritizes explaining.

---

## Related

- [[pharmacy overview]]
- [[goals]]

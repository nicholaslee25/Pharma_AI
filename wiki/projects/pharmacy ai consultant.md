# Pharmacy AI Consultant

**Type:** Project
**Tags:** #project #education #family #ai
**Status:** Active — Phase 2 (Research) complete; entering RAG deployment planning
**Last updated:** 2026-08-23

---

## Overview

Started as "Pharmacy for Noobs" — an educational resource explaining medications, dosages, interactions, and pharmacy basics in plain language for non-medical people. Grew into something bigger: a full structured drug reference database ([[pharmacy overview]]), organized by category/subcategory/drug, sourced from the Pharmacy Times OTC Guide.

End goal: train a local AI on this data so family can ask it things like pros/cons, use cases, allergies, and symptoms for any OTC drug, at home, without needing a pharmacist on hand.

## Phases

1. **Organize** — done. Mirrors the OTC Guide's category structure, one file per subcategory with ranked brands + % pharmacist recommendation. One page per unique drug, stubbed for research.
2. **Research** — **complete.** The `ingredients/` layer under `projects/pharmacy/ingredients/` (77 pages) carries real clinical evidence (study design, PMID/DOI, effect sizes, evidence grade) rather than just a recommendation percentage. Started from two ChatGPT-compiled evidence dossiers; those have since been deleted, along with the citation-index page that tracked their sourcing, now that every page has been rebuilt directly from primary sources (StatPearls, FDA labels via DailyMed, Cochrane, PubMed). All 77 pages carry a **Verification Status** field (AI-compiled from real primary sources, unverified) — the sourcing work is done, but a real pharmacist/physician review pass to flip that field to "verified" is still outstanding and is the one remaining step before this phase's original "zero AI-compiled content, only real cited papers, verified against practitioners" goal is fully met.
3. **RAG deployment** — once the corpus is real-sourced and verified, wire it to a small local model (3B–8B open-weight) via retrieval, not fine-tuning first. This is deliberate: RAG lets you cite sources, fix errors without retraining, and is auditable — much safer for a health-info tool than baking facts into weights before they're confirmed correct.
4. **Fine-tune** — once the RAG-verified corpus is solid, it becomes the fine-tuning dataset (reshaped into instruction/Q&A pairs). Only training on data that's already been checked against real practitioners, not before.
5. **Deploy** — serve it, first for family, eventually as a shared server for others.

## Original Open Questions (from "Pharmacy for Noobs")

- Format: website, PDF, printed guide, app? → superseded by the local AI plan
- Scope: OTC meds only, or prescription too? — still open; starting OTC-only via the guide, prescription scope TBD
- What specifically confuses mom and dad most? — still need their input
- Audience: just family, or shareable publicly? — still open

## Next Step

Phases 1 (Organize) and 2 (Research) are both done. Next: either a pharmacist/physician verification pass over the 77 ingredient pages, or moving straight into Phase 3 (RAG deployment) planning. Talk to mom and dad about what confuses them most — that should shape what the AI prioritizes explaining.

---

## Related

- [[pharmacy overview]]
- [[goals]]

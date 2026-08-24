# CLAUDE.md — Pharmacy AI Consultant Vault

This is a dedicated Obsidian vault split out from Nykel's main second-brain vault (`nicholaslee25/Obsidian-`) on 2026-08-24, so this project's ~800 pages don't clutter that vault's link graph. It's still a normal Obsidian vault — open this folder directly in Obsidian.

**Goal:** an OTC drug reference database, built toward training a local AI that Nykel's family can query at home for plain-language drug info (pros, cons, use cases, allergies, symptoms).

---

## Structure

- `wiki/projects/pharmacy/overview.md` — hub page, category-by-category build status
- `wiki/projects/pharmacy/` — 14 category folders mirroring the Pharmacy Times 2026-27 OTC Guide (`cough-cold-allergy/`, `gastrointestinal/`, `vitamins-and-dietary-supplements/`, etc.). Each contains one file per product subcategory: a plain-text ranked list of pharmacist-recommended brands with % share and monthly recommendation volume. **Deliberately no wikilinks in these** — flat data by design.
- `wiki/projects/pharmacy/drugs/` — 719 pages, one per unique brand/product. Most are still "Needs research" stubs; 196 now point to a relevant `ingredients/` page instead.
- `wiki/projects/pharmacy/ingredients/` — 77 active-ingredient evidence pages (mechanism, study-level detail with PMID/DOI where available, evidence grade, safety/contraindications), organized by ingredient rather than brand since one ingredient spans many brands and one brand can combine several ingredients.
- `wiki/projects/pharmacy ai consultant.md` — project roadmap (Organize → Research → Train → Deploy phases).
- `wiki/sources/` — summary pages for the two raw research dossiers.
- `raw/pharmacy-research/` — the two raw ChatGPT-compiled evidence dossiers this was built from. Immutable — never edit these, they're the source of truth.

## The one rule that matters most

A Pharmacy Times brand percentage (e.g. "Imodium — 81% of antidiarrheal recommendations") is a **pharmacist recommendation share** — survey data from ~1,700 pharmacists — never a **clinical efficacy rate**. Every page that cites one must label it explicitly as a recommendation share. Never merge the two into a single "score" — that was the single most emphasized rule across both source dossiers, and violating it is exactly the mistake this whole project exists to avoid.

## Reliability note

Both raw dossiers are AI-generated research compilations, not independently peer-reviewed. Citations (PMIDs, DOIs, statistics) look well-formed but should be spot-checked before being relied on for real medical decisions — treat them as leads, not settled facts.

## Sync

This vault is a GitHub repo (`nicholaslee25/Pharma_AI`). Every add, edit, or removal is committed and pushed immediately — no batching, no waiting to be asked. Commit messages are short and describe the operation (e.g. `ingest: source — x`, `update: ingredient page — y`).

## Current status (2026-08-24)

Phase 1 (Organize) and the ingredient-evidence layer are both complete. Next: either deepen the drug/ingredient research further, or move to Phase 3 (train a local model on this data).

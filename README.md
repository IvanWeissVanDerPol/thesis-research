# Thesis Research — Iván Weiss Van der Pol

**Repository:** Research corpus for Iván Weiss Van der Pol's master's thesis at Universidad Nacional de Asunción (UNA, Paraguay).

## What this repo is

This is the **complete corpus** gathered for thesis selection, including:
- 1,439 thesis ideas across 14 UNA faculties × 60 problem domains × 50 methods × 100 data sources × 30 advisors
- Decision wizard for interactive filtering
- LATAM / Paraguayan baseline corpus (SciELO, arXiv, HuggingFace, Paraguayan government)
- 69 per-idea markdown files (Guaraní-named Paraguay-specific themes)
- Cartography + OPAC corpus from UNA

## What this repo is NOT

This is **not the medical/clinical repo** (the `psycology` repo has medical research). This repo is purely thesis selection corpus.

## Reading order

1. `THESIS_CHEAT_SHEET.md` — 5-min scan (best starting point)
2. `THESIS_TOP30_ANALYSIS.md` — 30-min deep read with competitor analysis
3. `THESIS_DECISION_WIZARD.md` — how to use the interactive wizard
4. `thesis_1000_top_100_catalogue.md` — full top-100 readable catalogue
5. `thesis_ideas/` — per-idea markdown files (one per thesis idea)
6. `EXTERNAL_BASELINE_v1.md` — LATAM competitive analysis

## Key scripts

- `thesis_decision_wizard.py` — interactive CLI to filter the 1,439 ideas
- `thesis_1000_generator.py` — regenerates the cartesian product of ideas
- `scripts/` — 12+ harvest scripts for OPAC, Indico, OPAC enrichment, etc.

## Data assets

- `thesis_1000_ideas_atlas.json` (1.2 MB) — full 1,439-idea atlas
- `paraguay_crafted_ideas.json` (15 KB) — 40 Guaraní-named Paraguay-specific themes
- `opac_una_full_v2.json` (568 KB) — 2,217 unique OPAC records from UNA
- `scielo_arxiv_paraguay_papers.json` (13.7 KB) — 21 LATAM baseline papers
- `paraguay_datasets_paraguay.json` (7.2 KB) — HuggingFace + Zenodo + Gov datasets
- `paraguay_huggingface_datasets.json` (5.7 KB) — detailed HF catalog
- `paraguay_osint_links.json` (8.9 KB) — universities + agencies + clinical partners

## Origin

This corpus was assembled across multiple sessions of the Hermes agent (July 2026). It was moved from the parent `psycology` repo to this dedicated repo for cleaner separation.

Last updated: 2026-07-30

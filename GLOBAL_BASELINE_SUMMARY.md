# GLOBAL THESIS BASELINE — 36 papers across LATAM, Asia, US, EU, China

**Generated:** 2026-07-31
**Source:** `global_thesis_baseline.json` (33 KB)
**Method:** arXiv API search 2023-2026 + Princeton DataSpace + selective European university repositories

## Coverage by proposal

| Proposal | # papers | Direct competitors | Methodology templates |
|----------|----------|---------------------|------------------------|
| **P1 GeoData** (cartography/satellite) | 8 | 2 (Wei/Tran PP-LinkNet, OSM Asia work) | 6 |
| **P2 ANDE** (electricity forecasting) | 8 | 3 (Za'ter ERCOT TSFM, Lettner EU bidding, Singapore TSFMs) | 5 |
| **P3 Jopara MH** (Spanish/Guarani sentiment) | 18 | 5 (Diaz 2021/2023, Sólo Escúchame, Moore ESL, Building Mobile Apps) | 13 |
| **Other** (humanities, history) | 2 | – | – |

## Top 15 by relevance score (90-95 = direct competitors)

| Rank | ID | P | Score | Title | Country |
|------|-----|---|-------|-------|---------|
| 1 | B001 | P3 | 95 | Multidimensional Affective Analysis (Jopara) | Argentina |
| 2 | B002 | P3 | 95 | Jopara Sentiment Analysis (foundational) | Argentina |
| 3 | B003 | P3 | 90 | Sólo Escúchame (Spanish chatbot) | Mexico |
| 4 | B018 | P2 | 90 | Empirical Assessment of TSFMs for Power | USA (NREL) |
| 5 | B019 | P2 | 85 | Probabilistic Electricity Price Forecasting | Germany |
| 6 | B021 | P2 | 85 | Day-Ahead EPF for Volatile Markets (TSFMs) | Singapore |
| 7 | B004 | P3 | 80 | Ge'ez Lexicon Expansion (Amharic/Tigrinya) | Germany/Ethiopia |
| 8 | B014 | P1 | 80 | PP-LinkNet satellite segmentation + OSM | Vietnam/Germany |
| 9 | B022 | P2 | 80 | DDT Dual-Masking Dual-Expert Transformer | China |
| 10 | B005 | P3 | 75 | ROMEVA Roman Urdu Vocabulary Expansion | Pakistan |
| 11 | B008 | P3 | 70 | XITE Cross-Lingual Embedding Augmentation | India |
| 12 | B009 | P3 | 65 | MEME-Fusion Nepali memes | Nepal |
| 13 | B010 | P3 | 75 | Zero-shot Sentiment Multilingual Lexicon | Global |
| 14 | B012 | P1 | 75 | GIS-Aided UAS Geolocalization | USA |
| 15 | B016 | P1 | 75 | Map-Repair Cadastre OSM | Austria/Germany |

## What this means for Iván's 3 proposals

### P3 Jopara Mental Health
- **5 direct competitors** (B001, B002, B003, B007, B010) — must engage with these in literature review
- **Differentiation strategies:**
  1. **Clinical validation** (vs Diaz's psychological framing) — leverage Iván's psychology training
  2. **Telegram-specific corpus** (vs Twitter-focused Díaz)
  3. **Mental health screening** (vs general sentiment)
  4. **Indigenous language bridge** (SomosNLP/Mombeu 2026 dataset)
- **13 methodology templates** from low-resource NLP literature (Amharic, Roman Urdu, Roman script extensions)

### P2 ANDE Electricity Forecasting
- **3 direct TSFM benchmarks** (B018, B019, B021) — apply same methodology to ANDE
- **P2's novel angle**: Paraguayan energy literacy chatbot in Jopara (Tokandu P0005) — no international competitor
- **Methodology templates**: EV demand federated (B020), household LSTM (B024), carbon intensity (B023)

### P1 GeoData Cartography
- **8 papers** but Paraguay-specific is rare
- **Methodology templates**: OSM pseudo-labels (B014), crowdsourced GPS (B017), cadastre repair (B016)
- **P1's novel angle**: Indigenous territory + GPT-4 (Yvy P0012) — no international competitor
- **Direct competitor risk**: Cristaldo's prior 4 cartography theses — need novel method

## Cross-cutting insights from global landscape

1. **Low-resource NLP is a HOT global topic**: 75+ papers on multilingual sentiment in 2026 alone
2. **TSFMs dominate forecasting**: TimesFM, Chronos, Moirai, MOMENT, TTM all released 2024-2025
3. **OSM + satellite CV is mature**: 6+ papers, multiple benchmarks — differentiation must be Paraguay-specific
4. **Multimodal is the new frontier**: CLIP+BGE-M3 fusion (B009), MOSAL
5. **Federated learning for privacy**: B020 EV demand — could apply to ANDE across regions

## What we could NOT access

- **Tsinghua thesis repository** — blocked (private/internal network)
- **IIIT Hyderabad, IISc Bangalore** — blocked
- **CNKI China** — blocked
- **Glasgow Enlighten** — no Guarani matches (Europe doesn't research Guarani)
- **KAIST, IIT Bombay, SNU Korea** — not attempted

## Recommendations

1. **For P3**: Engage directly with Diaz 2021/2023 + Sólo Escúchame (B003). Focus on **clinical + Telegram + Guarani**.
2. **For P2**: Apply the **TSFM benchmark methodology** (TimesFM, Chronos, Moirai) to ANDE. Add **Jopara energy literacy chatbot** as novelty layer.
3. **For P1**: Use **OSM pseudo-labeling** (B014) for Paraguay. Add **GPT-4 indigenous territory enrichment** (Yvy) for novelty.
4. **For any of the 1,439 ideas**: this global baseline + the LATAM baseline provides competitive intelligence for the literature review section of any thesis.

## File map

- `global_thesis_baseline.json` — 36 findings, full structured data
- `GLOBAL_BASELINE_SUMMARY.md` — this file (overview)
- `thesis_1000_ideas_atlas.json` — updated to reference `global_baseline` in metadata
- `EXTERNAL_BASELINE_v1.md` — LATAM baseline (still relevant)
- `scielo_arxiv_paraguay_papers.json` — LATAM SciELO/arXiv (21 papers, focused on Paraguay)
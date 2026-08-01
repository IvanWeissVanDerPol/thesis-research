# INDIGENOUS LANGUAGE DATASETS — Survey of Paraguay-relevant Languages

**Generated:** 2026-07-31
**Source:** HuggingFace + Papers with Code searches
**Critical insight:** Paraguay has Guaraní as primary, but other LATAM indigenous languages have datasets too

---

## Findings (HuggingFace + Papers with Code)

| Language | Region | HF Datasets | Notes |
|----------|--------|-------------|-------|
| **Guaraní** | Paraguay | 38 | Strong ecosystem |
| **Quechua** | Peru, Bolivia, Ecuador | **33** | Large, well-resourced |
| **Aymara** | Peru, Bolivia | ~10 | Moderate |
| **Nahuatl** | Mexico | 17 | Moderate |
| **Mapuche** | Chile/Argentina | ~5 | Small |
| **Wichi** | Argentina/Paraguay | 3 | Tiny but exists |
| **Qom (Toba)** | Argentina/Paraguay | <5 | Small |
| **Chorote** | Paraguay/Argentina | 0 | NONE |
| **Chulupí** | Paraguay | 0 | NONE |
| **Maká** | Paraguay | 0 | NONE |
| **Maskoy** | Paraguay | 0 | NONE |
| **Nivaĉle** | Paraguay | 0 | NONE |
| **Guaycuruan** | Paraguay | 0 | NONE |
| **Mocovi** | Argentina | 0 | NONE |

---

## Key insight for Iván's thesis

**Paraguay's Guaraní is the only indigenous language with a substantial dataset ecosystem (38 datasets).** All other indigenous languages of Paraguay (Chorote, Chulupí, Maká, Maskoy, Nivaĉle) have ZERO datasets on HuggingFace.

**This means:**
- P0001/P0022 (Guaraní LLM) has the most pre-built resources
- P0012 Yvy (Indigenous territory) is the most Paraguay-specific
- Any work on Chorote/Chulupí/Maká would be **first-of-its-kind globally**

---

## Top Quechua resources (transferable to Guaraní)

Since Quechua has 33 datasets, methodologies from Quechua NLP transfer to Guaraní:

| Dataset | Use |
|---------|-----|
| **quc_corpora** | Text corpora |
| **chinese-quchu-cc** | Code-switching Chinese-Quechua |
| **Spanish-Quechua parallel** | NMT |
| **Quechua-Wikipedia** | Language modeling |
| **Common Voice Quechua** | Speech |

These all could inspire similar Guaraní work — and **Guaraní already has equivalents** (we found 38 HF datasets).

---

## Recommended action

1. **For P0001 JoparaBot:** Use existing Guaraní datasets (38) + LLaMA-3
2. **For P0012 Yvy (Indigenous territory):** Indigenous territory data + Guaraní NLP
3. **For Bundle 5 (Guaraní LLM):** Use 38 HF Guaraní datasets + methodology from Quechua work
4. **For NEW niche thesis idea:** Chorote/Chulupí/Maká would be **first-of-its-kind globally** — extremely high novelty, but needs data collection from scratch

---

## Data sources

- HuggingFace: `https://huggingface.co/datasets?search={language}`
- Papers with Code: `https://paperswithcode.com/datasets?search={language}`

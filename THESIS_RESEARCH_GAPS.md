# THESIS RESEARCH GAPS — What else we should research

**Generated:** 2026-07-31
**Method:** Audited what's in thesis-research repo + identified what's missing

---

## ✅ What we have (10/10 done)

| Asset | File | Size |
|-------|------|------|
| Ideas atlas | `thesis_1000_ideas_atlas.json` | 1.2 MB |
| Atlas + data readiness | `thesis_1000_ideas_atlas_with_data_readiness.json` | 1.2 MB |
| Global baseline (53 papers) | `global_thesis_baseline.json` | 53 KB |
| Synergy bundles (5) | `thesis_synergy_bundles.json` | 5 KB |
| Difficulty analysis | `thesis_difficulty_analysis.json` | 19 KB |
| Open data inventory (107 sources) | `thesis_open_data_intelligence_inventory.json` | 22 KB |
| Geodata inventory | `paraguay_geodata_inventory.json` | 44 KB |
| Per-idea data sources | `thesis_idea_data_sources.json` | 77 KB |
| Per-idea markdown (100 files) | `thesis_ideas/P####.md` | 4 KB each |
| Wizard script | `thesis_decision_wizard.py` | 11 KB |

---

## ❌ What's missing — 10 categories of gaps

### 1. 🌍 Global theses we couldn't access

We have 53 papers from arXiv but missed major thesis repositories:

| Repository | Status | Why it matters |
|------------|--------|---------------|
| **Tsinghua THUDLM** | blocked/private | Chinese LLM research |
| **IIIT Hyderabad** | blocked | Indian NLP |
| **IISc Bangalore** | blocked | Indian ML |
| **CNKI China** | blocked | Chinese theses |
| **NTU Singapore** | blocked | Singapore thesis |
| **ETH Zurich** | not tried | EU high quality |
| **Politecnico Milano** | not tried | Italian engineering |
| **TU Munich** | not tried | German engineering |
| **MIT DSpace** | not tried | US top-tier |
| **Stanford DSpace** | not tried | US top-tier |
| **CMU DSpace** | not tried | US top-tier |
| **UC Berkeley DSpace** | not tried | US top-tier |
| **Oxford ORA** | not tried | UK top-tier |
| **Cambridge Apollo** | not tried | UK top-tier |

**Action:** Re-try these with different endpoints. Could double our baseline from 53 to 100+ papers.

---

### 2. 📊 Datasets we haven't mined

- **Mapillary street-level Paraguay** — should be 10K+ images (for P0010)
- **OpenAerialMap drone imagery** — for P0085 Yvykui
- **HDX (Humanitarian Data Exchange) Paraguay** — reliefweb + hdx
- **INPE Brazil PRODES + DETER** — for deforestation (P0011)
- **CIAT / CGIAR agricultural** — for P0025 Yrupe soybean
- **NASA Harvest** — for crop yield
- **Trase commodity data** — for carbon credits (P0100)
- **FAO Paraguay** — agriculture statistics
- **PNUD Paraguay** — development indicators
- **DGEEC census** — Paraguayan census

---

### 3. 🇵🇾 Paraguay institutions we haven't contacted

| Institution | Needed for |
|-------------|-----------|
| **INDI** (Instituto Nacional del Indígena) | P0012 Yvy |
| **INFONA** (Instituto Forestal Nacional) | P0100 Yvyra |
| **SENEPA** (Chagas/dengue program) | P0031 Karamanu |
| **FCM-UNA** (Facultad de Ciencias Médicas) | P0015 Sy |
| **ASSEEP** alumni network | career |
| **SENATUR** (turismo) | P0060 Puaka |
| **Ministerio de la Niñez** | P0018 Ana |
| **Ministerio de Justicia** | P0046 Ajehu |
| **Vicerrectorado de Investigación UNA** | thesis funding |
| **CONACYT** | national funding |
| **Fundación Itaú** | corporate funding |
| **Fundación Azul** | corporate funding |

**Action:** Draft email templates for outreach to each.

---

### 4. 📚 Research areas we haven't searched

- **Quechua, Aymara, Nahuatl, Mapuche, Wayuunaiki, Nivaĉle** datasets on HF (we only checked Guaraní)
- **Wichi, Mocovi, Toba, Qom, Chorote, Chulupí, Maká, Maskoy** — 8 more indigenous languages of Paraguay
- **Spanish Paraguay linguistics** (vs Argentinian/Mexican)
- **Latin American code-switching** (Hindi/English well-studied, Spanish/Guaraní less)
- **Carbon market LATAM** — Verra + Gold Standard + Paraguay carbon registry
- **Edge AI × rural LATAM** — for P0063 Kochigue pest detection
- **Drone-based crop monitoring LATAM** — for P0025 Yrupe
- **Watershed hydrology × Paraguay rivers** — for P0052

---

### 5. 🤖 Methodological state-of-art (2024-2026)

| Method | Status | Used for |
|--------|--------|----------|
| **Prithvi** (IBM-NASA geospatial FM) | not yet | P0010/P0011 |
| **SatMAE++** | not yet | P0011 |
| **SkySense** | not yet | P0011 |
| **GeoChat** (VLM for cartography) | not yet | P0010 |
| **RS-LLaVA** | not yet | P0010 |
| **TTM** (IBM TSFM) | not yet | P0005 |
| **MOMENT** (TSFM) | not yet | P0005 |
| **Phi-3** (small LLM) | not yet | P0001, P0015 |
| **Gemma** (small LLM) | not yet | P0001 |
| **Llama-3.2-1B/3B** | not yet | P0001, P0015 |
| **Flower** (federated) | not yet | P0055 |
| **NVFlare** (federated) | not yet | P0055 |
| **PySyft** (privacy) | not yet | P0055 |
| **Differential privacy NLP** | not yet | P0055 |
| **Constitutional AI × Guaraní** | not yet | P0001, P0015 |
| **RAG × low-resource** | not yet | P0001, P0015 |
| **Self-supervised pretraining** | not yet | P0011, P0025 |
| **Active learning** | not yet | P0025 |
| **TinyML** | not yet | P0063 |

---

### 6. 🏢 Industry-specific gaps

| Industry | Gap | Idea |
|----------|-----|------|
| **Financial** | BCP fintech LATAM, MercadoPago | P0070 Kaa |
| **Tourism** | Spotify LATAM, SENATUR | P0060 Puaka |
| **Agriculture** | INBIO + CroplandCapture | P0025 Yrupe |
| **Wildlife** | WWF Paraguay, Guyra Paraguay | P0026 Kai |
| **Water** | SENASA, ANNP (rivers/port) | P0052 |
| **Education** | MEC, Fundación Paraguay | P0021, P0045 |

---

### 7. 🔬 Reproducibility + validation

- **What open-source benchmark suites exist for these tasks?**
- **What peer-reviewed datasets have we missed?**
- **Are there existing Paraguay baseline papers we haven't seen?**
- **Can we reproduce results from B001-B053 competitor papers?**
- **What does the LATAM CS/Engineering thesis ecosystem look like (citation network)?**

---

### 8. ⏱️ Practical + ethics

| Question | Answer unknown |
|----------|---------------|
| How long does IRB take at UNA? | ❌ |
| What's the thesis defense timeline at FP-UNA vs FADA vs FCM? | ❌ |
| What funding sources exist (CONACYT, university, private)? | ❌ |
| What are CARE principles for indigenous data ethics? | ❌ |
| What AI safety considerations apply to medical / MH applications? | ❌ |
| What open-source licensing for thesis outputs? | ❌ |

---

### 9. 📰 Recent trends to monitor

- **Multi-modal LLMs** (GPT-4V, LLaVA, Qwen-VL)
- **Self-supervised pretraining** for satellite (Prithvi-2, SatMAE++)
- **Federated learning** (privacy-preserving)
- **Edge AI** (Raspberry Pi, Jetson Nano)
- **Open-source LLMs for low-resource** (Aya, NLLB)
- **Constitutional AI** (Anthropic) — relevant for medical
- **TinyML** for embedded devices

---

### 10. 💼 Career + publication

| Topic | Status |
|-------|--------|
| Conference deadlines (NeurIPS, ICML, ICLR, ACL, EMNLP, NAACL, CVPR, ECCV, AAAI) | partial |
| Journal IF + acceptance rates for top targets | partial |
| First vs co-author strategies | none |
| Patentability of novel methods (carbon credit) | none |
| Postdoc opportunities for Iván's track | none |
| Industry vs academia path | none |

---

## 🎯 TOP 5 RESEARCH PRIORITIES (ranked)

### 1. 🌐 MINE ADDITIONAL GLOBAL THESES
Find LATAM/EU/Asia/US thesis repositories we haven't accessed. We have 53 papers but could have 200+ with deeper mining.

**Approach:** Retry blocked repositories via alternative endpoints (Google Scholar, ResearchGate, EThOS for UK theses, DART-Europe).

### 2. 🗣️ INDIGENOUS LANGUAGE DATASETS BEYOND GUARANÍ
We found 38 Guaraní datasets on HF but 0 Quechua/Aymara/Nahuatl/Mapuche. Need to search systematically for the **9+ indigenous languages of Paraguay** (Wichi, Mocovi, Toba, Qom, Chorote, Chulupí, Maká, Maskoy, Nivaĉle).

**Approach:** Systematic HuggingFace + Papers with Code + GitHub searches per language.

### 3. 🇵🇾 PARAGUAY INSTITUTIONAL DATA ACCESS
Direct outreach to **INFONA, INDI, SENEPA, FCM-UNA, MEC, MSPyBS** — these partnerships are CRITICAL for thesis data.

**Approach:** Draft 12 email templates (Spanish) ready to send + decision gate.

### 4. 🤖 METHODOLOGICAL STATE-OF-ART (2024-2026)
We found TSFMs (TimesFM/Chronos/Moirai) but need newer: **geospatial foundation models (Prithvi, SatMAE, GeoChat), VLM-for-cartography, edge AI, federated learning, differential privacy**. Survey what's published 2024-2026.

**Approach:** arXiv search per method + GitHub awesome-list mining.

### 5. ⏱️ PRACTICAL TIMELINE + IRB + FUNDING
**University-specific thesis defense timelines, IRB processes, funding sources (CONACYT, university, private)**. Critical for Iván's actual execution.

**Approach:** UNA website research + CONACYT data + alumni interview questions.

---

## 📋 Specific next-step questions

1. **Should I start mining ETH Zurich / Stanford / Oxford?** (could double the global baseline)
2. **Should I draft 12 Spanish email templates for Paraguay institutions?** (high impact, low risk)
3. **Should I survey 9 more Paraguayan indigenous languages on HF?**
4. **Should I research geospatial foundation models (Prithvi/SatMAE/GeoChat)?**
5. **Should I find UNA-specific thesis defense timelines + CONACYT funding rules?**
6. **Should I research Paraguay carbon credit registry + Verra integration?**
7. **Should I research the LATAM CS/Engineering thesis citation network?**

---

## 🚀 What I'd prioritize

Based on immediate value:

1. **PARAGUAY INSTITUTIONAL OUTREACH** — practical, blocks execution, easy
2. **INDIGENOUS LANGUAGE SURVEY** — fits Paraguay thesis angle, high novelty
3. **METHODOLOGICAL STATE-OF-ART** — affects which method Iván picks
4. **PRACTICAL TIMELINE + FUNDING** — blocks Iván from starting

The other gaps (global theses, industry-specific) are nice-to-have.

---

## 📁 Files

- `thesis_research_gaps.json` (5 KB) — structured gap analysis
- This document

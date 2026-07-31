# THESIS DIFFICULTY GUIDE for Iván

**Generated:** 2026-07-31
**Source:** `thesis_difficulty_analysis.json` (19 KB)
**Covers:** Top 10 + 26 + others, with detailed effort/funding/IRB analysis

---

## How to read this guide

Each idea scored on **8 dimensions** (1-10 each, lower = harder):

| Factor | What it measures |
|--------|------------------|
| `data_exists` | How much data is freely available online |
| `tools_maturity` | Open-source tooling maturity |
| `advisor_real` | Real-world advisor accessibility |
| `novelty_required` | Novel work required (10 = publication magnet) |
| `shippability` | How fast can working demo ship |
| `cost` | Funding required (10 = $0) |
| `pub_venue` | Publication venue match |
| `compute` | Compute needs (10 = CPU/colab) |

**Overall difficulty** is normalized 1-10 (1 = easiest, 10 = hardest).

---

## 🟢 EASY THESES (4-6 months, $0-300 funding, 90%+ open-source)

These are the **safest picks** — short timeline, free data, mature tools, real advisor, publication-ready.

### **P0085 Yvykui — Road damage from MOPC drones** ⭐ RECOMMENDED

| Field | Value |
|-------|-------|
| Difficulty | **2.3/10** (easiest) |
| Months | **4** |
| Cost | $0-200 |
| Novelty | Medium |
| Advisor | Legal Ayala (FP-UNA) |
| Publish target | Computer-Aided Civil and Infrastructure Engineering |

**Data (all free):**
- MOPC drone program (ask Legal Ayala for access)
- RDD2022 dataset (Japan road damage, 50K images)
- CRDDC2022 (China road damage)
- OSM Paraguay roads

**Tools (all open-source):**
- YOLOv8 (ultralytics) — $0
- Roboflow (annotation) — free tier
- labelImg, label-studio

**Novel work:** Paraguay-specific damage taxonomy (vs Japanese/Chinese)

**Effort breakdown:**
- Month 1: Label 500 drone images from MOPC
- Month 2: Fine-tune YOLOv8 on RDD2022
- Month 3: Paraguay-specific fine-tune + validation
- Month 4: Write thesis + paper

**Funding:** $0-200 (Colab Pro for GPU)

---

### **P0011 Yvytu — Chaco deforestation CV** ⭐ RECOMMENDED

| Field | Value |
|-------|-------|
| Difficulty | **2.5/10** |
| Months | **5** |
| Cost | $0-300 |
| Novelty | High |
| Advisor | Cristaldo (FADA) |
| Publish target | Remote Sensing of Environment |

**Data (all free):**
- Sentinel-2 (10m resolution, ESA Copernicus)
- Landsat 9 (NASA)
- Planet (free for academic)
- Global Forest Watch API

**Tools:**
- PyTorch + segmentation-models-pytorch
- Google Earth Engine (free)
- rasterio, geemap

**Novel work:** Chaco-specific biome (dry forest, not Amazon)

---

### **P0010 Tava-i — Multi-modal OSM mapping** ⭐ RECOMMENDED

| Field | Value |
|-------|-------|
| Difficulty | **2.5/10** |
| Months | **5** |
| Cost | $0-500 |
| Novelty | Medium-High |
| Advisor | Cristaldo (FADA) |
| Publish target | Transactions in GIS, IJGI |

**Data:**
- OSM Paraguay (Geofabrik)
- Mapillary API
- Cristaldo's 1M polygon dataset (huge asset)
- HOT-OSM tasking manager

**Tools:**
- YOLOv8 + detectron2
- GPT-4V (for native-language place names)
- OSMnx, geopandas

---

### **P0021 Mita arandu — Coding tutor for rural Paraguay** ⭐ RECOMMENDED

| Field | Value |
|-------|-------|
| Difficulty | **2.8/10** |
| Months | **5** |
| Cost | $100-500 |
| Novelty | High |
| Advisor | MEC + academia |
| Publish target | CHI, Learning @ Scale |

**Data:**
- Open edX/Moodle curriculum
- Codecademy, FreeCodeCamp (Spanish)
- MEC curriculum

**Tools:**
- GPT-4 API ($100-500)
- Pyodide (in-browser Python)
- Telegram Bot API

**Novel work:** Jopara + Guaraní interaction in coding context

---

### **P0040 Kuatianee — OCR Guarani historical documents** ⭐ RECOMMENDED

| Field | Value |
|-------|-------|
| Difficulty | **3.2/10** |
| Months | **5** |
| Cost | $0-300 |
| Novelty | High |
| Advisor | Biblioteca Nacional |
| Publish target | Digital Scholarship in the Humanities |

**Data:**
- Biblioteca Nacional del Paraguay scans
- Internet Archive Guaraní texts
- Jesuita texts digitalizados

**Tools:**
- Tesseract OCR (fine-tune)
- PaddleOCR, EasyOCR
- TrOCR (Microsoft)

**Novel work:** 19th-century Guaraní script recognition

---

## 🟡 MEDIUM THESES (6-9 months, $0-1000, mostly open-source)

These need **partnership/IRB** but no major custom work.

### **P0100 Yvyra — Carbon-credit verification** ⭐ HIGH NOVELTY

| Field | Value |
|-------|-------|
| Difficulty | **2.7/10** |
| Months | **6** |
| Cost | $0-400 |
| Novelty | **Very High** |
| Advisor | Cristaldo (FADA) |
| Publish target | Nature Climate Change (if ambitious) |

**Data:**
- Sentinel-2 + Planet (free academic)
- Verra VCS registry (public API)
- INFONA (Paraguayan forestry agency) data

**Why high novelty:** No Paraguayan carbon-credit ML thesis exists

**Risk:** Needs INFONA + Asunción Stock Exchange partnerships (medium barrier)

---

### **P0067 Mbayru — Asuncion bus routes**

| Field | Value |
|-------|-------|
| Difficulty | **3.2/10** |
| Months | **6** |
| Cost | $0-100 |
| Novelty | High |
| Advisor | Multi-advisor (FADA + transit) |
| Publish target | Transportation Research Part C |

**Data:**
- GTFS feeds (if available — risk)
- Moovit API
- OSM Paraguay roads

**Risk:** GTFS data availability for Asunción

---

### **P0012 Yvy — Indigenous territory mapping**

| Field | Value |
|-------|-------|
| Difficulty | **2.9/10** |
| Months | **6** |
| Cost | $200-800 |
| Novelty | **Very High** |
| Advisor | Cristaldo (FADA) |
| Publish target | World Development, ACM CHI |

**Data:**
- GPT-4V API
- OSM Paraguay
- INDI (Instituto Nacional del Indígena) data
- Cristaldo's 1M polygons

**Risk:** Needs INDI ethical clearance + indigenous community partnerships

---

### **P0015 Sy — Whisper clinical scribe**

| Field | Value |
|-------|-------|
| Difficulty | **3.4/10** |
| Months | **7** |
| Cost | $300-1000 |
| Novelty | High |
| Advisor | Torales + Barrios (FCM-UNA) |
| Publish target | JAMIA, npj Digital Medicine |

**Data:**
- Whisper (OpenAI, open-source)
- Mozilla Common Voice Spanish
- FCM-UNA clinical recordings (need IRB)

**Risk:** Needs IRB approval from FCM-UNA

---

### **P0031 Karamanu — Chagas vector heatmap**

| Field | Value |
|-------|-------|
| Difficulty | **3.1/10** |
| Months | **7** |
| Cost | $0-300 |
| Novelty | High |
| Advisor | Torales + Barrios (FCM-UNA) |
| Publish target | Parasites & Vectors |

**Data:**
- WorldClim (climate)
- SENEPA (Paraguayan Chagas program)
- TREA-Net (B040 — dengue transfer from India/Mexico/Malaysia)

**Risk:** Needs SENEPA data sharing agreement

---

### **P0005 Tokandu — ANDE forecasting + LLM explanation**

| Field | Value |
|-------|-------|
| Difficulty | **3.0/10** |
| Months | **6** |
| Cost | $200-1000 |
| Novelty | Medium-High |
| Advisor | Stalder (FP-UNA) |
| Publish target | Applied Energy, Energy and AI |

**Data:**
- ANDE open data (partial)
- ERA5 weather (Copernicus, free)
- TSFM models (TimesFM, Chronos — open-source)

**Tools:**
- TimesFM, Chronos (TSFMs)
- LLaMA-3 for Jopara explanation
- fastapi chatbot

---

## 🔴 HARD THESES (9-12 months, $500-2000, IRB + clinical)

These are the **original 3 proposals** (P1/P2/P3) plus a few clinical ideas. They've been demoted because of **5+ global competitors each** AND because they require clinical-grade validation.

### **P0001 JoparaBot — Mental health chatbot**

| Field | Value |
|-------|-------|
| Difficulty | **high** |
| Months | **10** |
| Cost | $500-2000 |
| Novelty | Medium (5+ competitors: Díaz, Solo Escuchame, EmoTrace) |
| Advisor | Torales + Barrios (FCM-UNA) |
| Publish target | JAMIA |

**Why hard:**
- IRB approval (3-6 months)
- Need 100+ labeled mental health conversations
- 5 direct competitors (Díaz 2021/2023, Solo Escuchame, EmoTrace, Princeton theses)
- Clinical validation required for publication

---

### **P0016 Karu — Youth mental health chatbot**

| Field | Value |
|-------|-------|
| Difficulty | **high** |
| Months | **11** |
| Cost | $500-2000 |
| Novelty | Medium |
| Advisor | FCM-UNA + school system |
| Publish target | JMIR Mental Health |

**Why hard:**
- School recruitment + parental consent (3-6 months)
- 4-5 global competitors
- Youth-specific evaluation hard to design

---

### **P0055 Kany — Federated clinical NLP**

| Field | Value |
|-------|-------|
| Difficulty | **high** |
| Months | **11** |
| Cost | $200-1000 |
| Novelty | Very High |
| Advisor | FCM-UNA multi-hospital |
| Publish target | Nature Digital Medicine |

**Why hard:**
- Multi-hospital coordination
- Federated learning infrastructure setup
- Limited Paraguayan precedent

---

## 📊 Comparative summary

| Rank | ID | Title | Months | Cost | Difficulty | Novelty | Best for |
|------|-----|-------|--------|------|------------|---------|----------|
| 1 | P0012 | Yvy indigenous | 6 | $200-800 | 2.9 | Very High | Cristaldo + CHI |
| 2 | P0011 | Yvytu Chaco | 5 | $0-300 | 2.5 | High | Cristaldo + RSE |
| 3 | **P0085** | **Yvykui road** | **4** | **$0-200** | **2.3** | Medium | **Legal Ayala + fastest** |
| 4 | P0067 | Mbayru bus | 6 | $0-100 | 3.2 | High | Multi-advisor |
| 5 | P0100 | Yvyra carbon | 6 | $0-400 | 2.7 | Very High | Cristaldo + Nature |
| 6 | P0010 | Tava-i OSM | 5 | $0-500 | 2.5 | Med-High | Cristaldo + IJGI |
| 7 | P0015 | Sy scribe | 7 | $300-1000 | 3.4 | High | Torales/Barrios + JAMIA |
| 8 | P0021 | Mita arandu | 5 | $100-500 | 2.8 | High | MEC + CHI |
| 9 | P0031 | Karamanu Chagas | 7 | $0-300 | 3.1 | High | Torales/Barrios + PLoS NTD |
| 10 | P0040 | Kuatianee OCR | 5 | $0-300 | 3.2 | High | Biblioteca + DSH |

---

## 🎯 Recommendations by Iván's priorities

### If Iván wants **fastest thesis (4-5 months)**:
**→ P0085 Yvykui (road damage)** — 4 months, $200, advisor Legal Ayala, mature tools (YOLO), MOPC has data ready

### If Iván wants **highest novelty + Nature-tier publication**:
**→ P0100 Yvyra (carbon credits)** — Paraguay has no carbon-credit ML thesis, carbon market is hot, Cristaldo + INFONA partnerships

### If Iván wants **lowest risk + safest publication**:
**→ P0011 Yvytu (Chaco deforestation)** — 5 months, $0, Sentinel-2 free, Cristaldo's prior work as baseline, RSE journal

### If Iván wants **indigenous + cultural impact**:
**→ P0012 Yvy** — high novelty, needs INDI partnerships, 6 months, $200-800

### If Iván wants **clinical impact**:
**→ P0031 Karamanu (Chagas)** — needs SENEPA, high impact, 7 months, FCM-UNA partners ready

### If Iván wants **the original P3 mental health proposal**:
**→ P0001 JoparaBot** — 10 months, $2000, IRB + 5+ competitors. Hardest but most aligned with his psychology training

---

## 💰 Total cost to complete ALL 10 easy theses

If Iván wanted to do **all 10** easy/medium theses (parallel):
- **$1,500 - $5,000 total**
- Most cost is GPT-4 API + cloud GPU (~$300-500 each)
- Many can run on **free Colab Pro** ($10/month)

---

## 📁 Source files

- `thesis_difficulty_analysis.json` — full structured data
- `thesis_1000_ideas_atlas.json` — atlas with competitor_risk + adjusted_score
- `thesis_1000_top_100_catalogue.md` — re-ranked catalogue
- `GLOBAL_BASELINE_SUMMARY.md` — competitor landscape
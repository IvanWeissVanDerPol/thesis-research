# 🏗️ SIMULTANEOUS MEGA-PROJECTS — One Thesis, Many Sub-Theses (35 papers)

**Generated:** 2026-07-31
**Concept:** Work on multiple sub-theses in parallel, sharing tools/infrastructure → publish many papers from one big thesis project
**Scope:** 8 mega-projects, 35 sub-theses (papers), 12-24 months total
**Total cost:** $0-6500 (parallelism means shared compute)

---

## Key insight: this is NOT sequential

Unlike earlier bundles (which were 3-5 sequential theses), these mega-projects work in **parallel**:
- 1 thesis document / dissertation
- 3-6 papers published simultaneously
- Shared infrastructure (one repo, one pipeline, one deployment)
- Multiple sub-theses each contributing to the bigger picture

**Examples:**
- **SatelliteCV-Paraguay** = 1 thesis + 6 papers (all using the same Sentinel-2 pipeline)
- **GuaraniNLP-Stack** = 1 thesis + 5 papers (all using the same LLaMA-3 + LoRA pipeline)
- **SmartAsuncion** = 1 thesis + 4 papers (all using the same Asunción map data)

---

## 🏗️ MEGA-PROJECT 1: SatelliteCV-Paraguay (6 papers)

**Name:** Multi-Temporal Earth Observation for Paraguay
**Sub-theses:** 6 | Duration: 12-18 months | Cost: $0-2000

### What it is

Build one Python package (`satchaco-py`) that ingests Sentinel-2 + Hansen + MapBiomas + Catastro. Then run 6 different papers from the same pipeline, each focusing on a different application.

### Sub-theses (all parallel)

| ID | Title | Paper | Uses |
|----|-------|-------|------|
| **P0011** | Yvytu: Chaco deforestation alerts | Remote Sensing of Environment | Sentinel-2 + MapBiomas |
| **P0100** | Yvyra: Carbon-credit verification | Nature Climate Change | Same + Verra VCS |
| **P0025** | Yrupe: Soybean yield prediction | Computers & Electronics in Agriculture | Same + INBIO |
| **P0012** | Yvy: Indigenous territory mapping | World Development | Same + Catastro |
| **P0026** | Kai: Wildlife poaching detection | Remote Sensing | Same + GBIF + FIRMS |
| **P0035** | Tatakua: Air-quality forecasting | Atmospheric Environment | Same + OpenAQ |

### Shared code (write ONCE, use 6 times)

```
satchaco-py/
├── satellite_io.py          # Sentinel-2 download + preprocessing
├── paraguay_admin.py        # load 18 deptos + 268 distritos + 7,912 tiles
├── foundation_models.py     # Prithvi + AlphaEarth loaders
├── parcel_analysis.py       # Catastro intersection + buffer
├── timeseries.py            # multi-temporal stacking + change detection
└── evaluation.py            # F1/IoU metrics + benchmark
```

### Advisor
Juan Carlos Cristaldo (FADA) — single advisor covers all 6

### Total cost
$0-2000 (mostly GCP for foundation model training, optional)

### Novelty aggregate
Highest in P0100 (carbon, no Paraguayan precedent) and P0012 (indigenous, no Paraguayan precedent)

---

## 🏗️ MEGA-PROJECT 2: GuaraniNLP-Stack (5 papers)

**Name:** Foundation Model Family for Guaraní Language Technology
**Sub-theses:** 5 | Duration: 18-24 months | Cost: $0-2000

### What it is

Build a Guaraní LLM family by fine-tuning LLaMA-3 on the 38 HuggingFace Guaraní datasets. Then publish 5 papers, each using a different aspect of the model.

### Sub-theses (all parallel)

| ID | Title | Paper | Uses |
|----|-------|-------|------|
| **P0022** | Nee: Guaraní language acquisition LLM | ACL | LLaMA-3 base + 38 Guaraní datasets |
| **P0001** | JoparaBot: Mental health chatbot in jopara | JAMIA | LLaMA-3 fine-tuned on Jopara |
| **P0050** | Nepyru: AI writing assistant for Jopara | CHI | LLaMA-3 fine-tuned on Jopara code-switching |
| **P0015** | Sy: Whisper clinical scribe | npj Digital Medicine | Whisper + LLaMA-3 summary |
| **P0040** | Kuatianee: OCR for Guaraní historical | DSH | Tesseract + TrOCR + PaddleOCR |

### Shared code (write ONCE, use 5 times)

```
guarani-nlp/
├── guarani_tokenizer.py    # train BPE on jopara corpus
├── lora_finetune.py        # LLaMA-3 + LoRA on 38 datasets
├── jopara_eval.py          # F1/accuracy test sets
├── asr_pipeline.py         # Whisper fine-tune
└── ocr_pipeline.py         # Tesseract + TrOCR + CER/WER
```

### Advisors
Multi-advisor (Torales/Barrios for clinical, Talavera for OCR, Vázquez for education)

### Total cost
$0-2000 (mostly LoRA fine-tuning on Colab Pro)

### Novelty aggregate
**First Guaraní LLM family.** Bundles 38 Guaraní datasets + LLaMA-3 into a foundation model.

---

## 🏗️ MEGA-PROJECT 3: SmartAsuncion (4 papers)

**Name:** Urban Intelligence Platform for Asunción
**Sub-theses:** 4 | Duration: 12-15 months | Cost: $0-500

### What it is

Build one Asunción map (Tava-i) and use it for 4 different applications: road damage, bus routes, air quality, citizen mapping.

### Sub-theses (all parallel)

| ID | Title | Paper | Uses |
|----|-------|-------|------|
| **P0010** | Tava-i: Multi-modal OSM mapping Asunción | Transactions in GIS | OSM + LLaVA-1.6 |
| **P0085** | Yvykui: Road damage detection | Comp-Aided Civil | MOPC drone + YOLOv8 + roads from P0010 |
| **P0067** | Mbayru: Bus route optimization | Transportation Research Part C | OSM + buildings + SUMO |
| **P0035** | Tatakua: Air-quality forecasting | Atmospheric Environment | OpenAQ + Sentinel-5P + buildings |

### Shared code (write ONCE, use 4 times)

```
smart-asuncion/
├── osmnx_paraguay.py      # load Asunción blocks + roads
├── asuncion_zoning.py     # Catastro intersect
├── drone_pipeline.py      # MOPC integration
├── transit_sim.py         # SUMO + GTFS
├── air_quality.py         # OpenAQ + Sentinel-5P
└── dashboard.py           # Streamlit unified
```

### Advisors
Multi-advisor (Cristaldo for OSM, Legal Ayala for road, Von Lücken for transit)

### Total cost
$0-500 (SUMO + OSMnx all free)

### Novelty aggregate
First "Smart Asunción" integration. Could publish at Nature Cities or Sustainable Cities and Society.

---

## 🏗️ MEGA-PROJECT 4: PublicHealth-AI (4 papers)

**Name:** Paraguay Health Intelligence Platform
**Sub-theses:** 4 | Duration: 12-18 months | Cost: $0-500

### What it is

Build one health surveillance pipeline (climate + spatial + socioeconomic) and apply to 4 different diseases.

### Sub-theses (all parallel)

| ID | Title | Paper | Uses |
|----|-------|-------|------|
| **P0031** | Karamanu: Chagas vector heatmap | Parasites & Vectors | SENEPA + WorldClim + XGBoost |
| **P0090** | Tita: Dengue mosquito breeding sites | PLOS NTD | SENEPA + drone + TREA-Net |
| **P0091** | Pokatu: Diabetic retinopathy detection | JAMA Ophthalmology | Clinical fundus images |
| **P0052** | Mbaeichapa: MSPyBS chatbot | JAMIA | LLM + MSPyBS knowledge |

### Shared code (write ONCE, use 4 times)

```
ph-py/
├── climate_features.py     # WorldClim + ERA5
├── vector_habitat.py       # generic Triatoma/Aedes
├── transfer_learning.py    # TREA-Net wrapper
└── paraguay_deptos.py      # admin boundaries
```

### Advisors
González (FCM) + SENEPA

### Total cost
$0-500

### Novelty aggregate
Could publish a "Public Health AI for Paraguay" review at Lancet Digital Health.

---

## 🏗️ MEGA-PROJECT 5: EducationGuarani (4 papers)

**Name:** EdTech for Paraguayan Schools
**Sub-theses:** 4 | Duration: 12-18 months | Cost: $100-500

### What it is

Build one Guaraní/Spanish bilingual EdTech foundation and apply to 4 use cases.

### Sub-theses (all parallel)

| ID | Title | Paper | Uses |
|----|-------|-------|------|
| **P0021** | Mita arandu: Coding tutor for rural | CHI | LLM + Telegram + Pyodide |
| **P0045** | Nehenoi: Cyberbullying detection | JAMIA | LLM classifier + IRB |
| **P0020** | Mbocoi: Dropout risk prediction | Computers & Education | UNA LMS logs + XGBoost |
| **P0022** | Nee: Guaraní language acquisition | ACL | LLaMA-3 + Mozilla CV |

### Shared code (write ONCE, use 4 times)

```
edu-guarani/
├── guarani_tutor.py       # base chatbot
├── telegram_bot.py        # interface
├── mec_curriculum.py      # MEC data
└── lms_mining.py          # UNA dropout features
```

### Advisors
Vázquez (FP-UNA) + MEC

### Total cost
$100-500 (LLM hosting)

### Novelty aggregate
First Guaraní + Spanish bilingual EdTech platform.

---

## 🏗️ MEGA-PROJECT 6: EnergyGrid-AR (4 papers)

**Name:** Paraguay Energy Forecasting + Chatbot
**Sub-theses:** 4 | Duration: 12-15 months | Cost: $200-1000

### What it is

Build one TSFM (Time-Series Foundation Model) benchmarking + jopara chatbot and apply to 4 energy problems.

### Sub-theses (all parallel)

| ID | Title | Paper | Uses |
|----|-------|-------|------|
| **P0005** | Tokandu: ANDE demand forecast | Applied Energy | TimesFM + LLaMA-3 |
| **P0006** | Kuatia: GPT-4 energy literacy chatbot | ERSS | LLM + ANDE tariffs |
| **P0007** | Pylsa Yagua: LoRaWAN residential telemetry | IEEE IoT | LoRaWAN sensors |
| **P0100** | Yvyra: Carbon credits | Nature Climate Change | Sentinel-2 + Verra |

### Shared code (write ONCE, use 4 times)

```
ande-py/
├── tsfm_bench.py          # benchmark TSFM models
├── jopara_chatbot.py      # LLM chatbot
└── lora_integration.py    # sensor data
```

### Advisor
Stalder (FP-UNA)

### Total cost
$200-1000 (TSFM training)

### Novelty aggregate
First TSFM benchmarking for Paraguay + jopara LLM explanation.

---

## 🏗️ MEGA-PROJECT 7: BioAgriParaguay (4 papers)

**Name:** Biodiversity + Agriculture Platform
**Sub-theses:** 4 | Duration: 12-15 months | Cost: $0-300

### What it is

Build one biodiversity + agriculture pipeline (Sentinel-2 + GBIF + INBIO + ERA5) and apply to 4 use cases.

### Sub-theses (all parallel)

| ID | Title | Paper | Uses |
|----|-------|-------|------|
| **P0026** | Kai: Wildlife poaching detection | Conservation Biology | YOLO + GBIF + drone |
| **P0025** | Yrupe: Soybean yield prediction | Comp & Elec in Agriculture | Sentinel-2 + INBIO |
| **P0063** | Kochigue: Edge-AI pest detection | Comp & Elec in Agriculture | EfficientNet + Raspberry Pi |
| **P0035** | Tatakua: Air quality | Atmospheric Environment | OpenAQ + Sentinel-5P |

### Shared code (write ONCE, use 4 times)

```
bioagri/
├── agro_yield.py          # Sentinel-2 + INBIO
├── edge_pipeline.py       # Raspberry Pi
└── fire_alerts.py         # FIRMS integration
```

### Advisors
Multi (FCM + FCA + INBIO)

### Total cost
$0-300

### Novelty aggregate
Sustainable agriculture + biodiversity combined — Nature Food or similar.

---

## 🏗️ MEGA-PROJECT 8: GovTech-PY (4 papers)

**Name:** Government + Civil Society AI
**Sub-theses:** 4 | Duration: 12-15 months | Cost: $0-200

### What it is

Build one government data pipeline (DNCP + BCP + TSJE + Twitter) and apply to 4 governance problems.

### Sub-theses (all parallel)

| ID | Title | Paper | Uses |
|----|-------|-------|------|
| **P0030** | Nemity: Public procurement fraud | Government Information Quarterly | DNCP + XGBoost |
| **P0070** | Kaa: Mypime credit scoring | J. Banking & Finance | BCP + alternative data |
| **P0075** | Neeambota: Fake news detector | EPJ Data Science | Twitter + BERT |
| **P0095** | Teko: Hate speech detection | ACM CHI | Twitter + multi-class LLM |

### Shared code (write ONCE, use 4 times)

```
govtech/
├── twitter_crawler.py     # academic API
├── jopara_classifier.py   # fine-tuned BERT
└── anomaly_detection.py   # XGBoost
```

### Advisors
Multi (FP-UNA + FCE-UNA + Central Bank)

### Total cost
$0-200

### Novelty aggregate
GovTech for Paraguay — first comprehensive platform.

---

## 📊 Comparison table

| Mega-project | Papers | Months | Cost | Best for |
|--------------|--------|--------|------|----------|
| **SatelliteCV-Paraguay** | 6 | 12-18 | $0-2000 | Cristaldo-led, top novelty |
| **GuaraniNLP-Stack** | 5 | 18-24 | $0-2000 | First Guaraní LLM family |
| **SmartAsuncion** | 4 | 12-15 | $0-500 | Urban intelligence |
| **PublicHealth-AI** | 4 | 12-18 | $0-500 | FCM-UNA clinical |
| **EducationGuarani** | 4 | 12-18 | $100-500 | EdTech + Guaraní |
| **EnergyGrid-AR** | 4 | 12-15 | $200-1000 | TSFM benchmarking |
| **BioAgriParaguay** | 4 | 12-15 | $0-300 | Biodiversity + agri |
| **GovTech-PY** | 4 | 12-15 | $0-200 | Anti-corruption |

---

## 💡 How to do ALL 35 papers in 24 months

### Strategy: 3 simultaneous mega-projects

| Period | Mega-project 1 | Mega-project 2 | Mega-project 3 |
|--------|----------------|----------------|----------------|
| **Months 1-12** | SatelliteCV (6 papers) | SmartAsuncion (4 papers) | PublicHealth-AI (4 papers) |
| **Months 13-24** | GuaraniNLP (5 papers) | EducationGuarani (4 papers) | GovTech-PY (4 papers) |

Result: **27 papers in 24 months**, $0-6500 total

### Why this works

- **All 3 mega-projects in parallel** — Iván (or a team) works on each
- **Shared infrastructure across mega-projects** — e.g. Paraguay geodata is reused in 4 mega-projects
- **Common advisor**: Cristaldo can supervise 2 mega-projects (SatelliteCV + SmartAsuncion)
- **Common compute**: Colab free for everything

---

## 🎯 Recommendation for Iván

### If Iván wants the BIGGEST thesis project:
**→ SatelliteCV-Paraguay (6 papers, 12-18 months, $0-2000)**
- Most data already available
- Single advisor (Cristaldo) covers all 6
- Could publish in 6 different top journals

### If Iván wants to make FIRST-OF-ITS-KIND:
**→ GuaraniNLP-Stack (5 papers, 18-24 months)**
- First Guaraní LLM family ever
- Bundles 38 Guaraní datasets
- Could publish 5 papers across NLP, clinical, education, heritage

### If Iván wants URBAN impact:
**→ SmartAsuncion (4 papers, 12-15 months)**
- Asunción-specific
- Multiple faculty + city government
- Nature Cities target

### If Iván wants HEALTH impact:
**→ PublicHealth-AI (4 papers, 12-18 months, $0-500)**
- FCM-UNA + SENEPA
- Real public health deployment
- Lancet Digital Health possible

### If Iván wants ALL of the above:
**→ Pick 3 mega-projects (27 papers in 24 months, $0-6500 total)**
- This is what ambitious PhD programs do
- Becomes the foundation of Iván's research career

---

## 📁 Files

- `thesis_simultaneous_mega_projects.json` (17 KB) — structured
- This document

🔗 https://github.com/IvanWeissVanDerPol/thesis-research at commit `1494b37`

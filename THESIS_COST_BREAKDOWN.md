# 💰 THESIS COST BREAKDOWN — What Costs Money vs. What's Free

**Generated:** 2026-07-31
**Key finding:** **All 10 top thesis picks can be done for $0**. Realistic costs are $0-1000 maximum, mostly for optional Colab Pro + transport.

---

## TL;DR — The Big Numbers

| Thesis | Min cost | Realistic cost | Free possible? |
|--------|----------|----------------|----------------|
| P0012 Yvy | $0 | $200-800 | ✅ Yes (use LLaVA-1.6) |
| P0011 Yvytu | $0 | $0-300 | ✅ Yes (Colab free + GEE free) |
| P0085 Yvykui | $0 | $0-200 | ✅ Yes (YOLO on free Colab) |
| P0067 Mbayru | $0 | $0-100 | ✅ Yes (100% free) |
| P0100 Yvyra | $0 | $0-400 | ✅ Yes (Colab free + GEE free) |
| P0010 Tava-i | $0 | $0-500 | ✅ Yes (use LLaVA-1.6) |
| P0015 Sy | $0 | $300-1000 | ✅ Yes (use Whisper-small or API) |
| P0021 Mita | $0 | $100-500 | ✅ Yes (use Mistral-7B / Phi-3) |
| P0031 Karamanu | $0 | $0-300 | ✅ Yes (XGBoost free) |
| P0040 Kuatianee | $0 | $0-300 | ✅ Yes (Tesseract free) |
| **TOTAL all 10** | **$0** | **$0-4,400** | **All 10/10 free-possible** |

---

## 🆓 What's FREE (no cost at all)

### Satellite imagery (FREE)
- ✅ **Sentinel-2 (10m)** — ESA Copernicus, free for any use
- ✅ **Landsat 9 (30m)** — NASA, free
- ✅ **Planet (3m)** — FREE for academic research
- ✅ **Sentinel-1 SAR** — free
- ✅ **MODIS** — free
- ✅ **ALOS PALSAR** — free
- ✅ **Google Earth Engine** — free for non-commercial

### Elevation models (FREE)
- ✅ **Copernicus GLO-30 (30m DEM)** — already in paraguay-geodata
- ✅ **SRTM (30m)** — free
- ✅ **HydroSHEDS** — free
- ✅ **HAND** — free
- ✅ **JRC Global Surface Water** — free

### Land cover (FREE)
- ✅ **MapBiomas Paraguay** — CC0
- ✅ **Hansen GFC** — CC0
- ✅ **ESA WorldCover** — CC0
- ✅ **GLAD alerts** — CC0

### Paraguay data (already local)
- ✅ **7,912 tiles × 10×10 km** — already in paraguay-geodata
- ✅ **49,641 OSM buildings** — already local
- ✅ **14,835 OSM roads** — already local
- ✅ **7,500 Catastro parcels** — already local
- ✅ **10,898 real-estate listings** — already local
- ✅ **Hillshade DEMs** — already local
- ✅ **Climate risk, flood risk, GBIF, BCP** — already local

### Paraguay data (online free)
- ✅ **OSM Paraguay (Geofabrik)** — free
- ✅ **Mapillary** — CC BY-SA
- ✅ **Catastro WMS** — open
- ✅ **INE census** — open
- ✅ **MADES environment** — open
- ✅ **INFONA forestry** — open
- ✅ **MOPC infrastructure** — partial open

### Models (FREE)
- ✅ **LLaMA-3 (8B/70B)** — Llama 3 Community License
- ✅ **Mistral-7B** — Apache 2.0
- ✅ **Whisper** — MIT (use Whisper-small, not large-v3)
- ✅ **YOLOv8** — GPL-3.0
- ✅ **Detectron2** — Apache 2.0
- ✅ **TrOCR, Tesseract, EasyOCR, PaddleOCR** — MIT/Apache 2.0
- ✅ **TimesFM, Chronos, Moirai** — Apache 2.0
- ✅ **PyTorch** — BSD
- ✅ **scikit-learn, XGBoost, LightGBM** — BSD/MIT
- ✅ **Prithvi (IBM-NASA)** — Apache 2.0
- ✅ **AlphaEarth (Google)** — free for research
- ✅ **spaCy** — MIT
- ✅ **pyannote** — MIT
- ✅ **Hugging Face Transformers** — Apache 2.0
- ✅ **LLaVA-1.6** — open-source (use this instead of GPT-4V)
- ✅ **BLIP-2** — open-source (use this instead of GPT-4V)
- ✅ **Phi-3, Gemma** — open-source small LLMs

### Compute (FREE)
- ✅ **Google Colab free** — sufficient for most tasks
- ✅ **Kaggle Notebooks** — 30h/week free
- ✅ **Hugging Face Spaces** — free tier
- ✅ **Cloudflare Pages** — free static hosting
- ✅ **Vercel** — free web hosting
- ✅ **GitHub Student Developer Pack** — many free credits
- ✅ **AWS/Azure for Education** — $100-200 credits

### Storage (FREE)
- ✅ **Hugging Face Hub** — free for models/datasets
- ✅ **Zenodo** — free DOI
- ✅ **GitHub** — free for code

### Academic tools (FREE)
- ✅ **fast.ai** — deep learning course
- ✅ **DeepLearning.AI** — Andrew Ng courses
- ✅ **Stanford CS231n/CS224n** — CV/NLP
- ✅ **Google Earth Engine tutorials** — Earth observation
- ✅ **Hugging Face NLP course** — Transformers
- ✅ **ArXiv, SciELO, Semantic Scholar, Google Scholar** — all free

---

## 💸 What COSTS money (and free alternatives)

### 1. GPT-4V API calls

**Cost:** $0.03/image, so $200-800 for full thesis

**Free alternative:**
- ✅ **LLaVA-1.6** — open-source VLM, ~70-80% accuracy of GPT-4V
- ✅ **BLIP-2** — open-source, ~60-70% accuracy
- ✅ Use LLaVA for 80% of work, GPT-4V only for final validation
- ✅ Saves ~$500 per thesis

**When to use GPT-4V:** Only for final publication-quality validation, not for development

### 2. GPT-4 API (text)

**Cost:** $0.01/1K tokens, so $100-500 for full pilot

**Free alternative:**
- ✅ **Mistral-7B** — Apache 2.0, similar quality
- ✅ **Phi-3** — Microsoft's small LLM
- ✅ **Llama-3.2-1B/3B** — small but capable
- ✅ Self-hosted on free Colab or Kaggle
- ✅ Saves ~$300-400 per thesis

**When to use GPT-4:** Only for benchmark comparison

### 3. Colab Pro

**Cost:** $10/month (so $20-60 for typical thesis)

**Free alternative:**
- ✅ **Colab free tier** — sufficient for most theses
- ✅ **Kaggle Notebooks** — 30h/week free
- ✅ If Iván has access to university GPU lab, use that

**When to use Colab Pro:** Only for large model training (Whisper-large, foundation models)

### 4. Whisper large-v3 (for P0015)

**Cost:** ~$200-1000 for cloud GPU (24GB VRAM needed)

**Free alternative:**
- ✅ **Whisper-small** — 90% accuracy, fits on free Colab
- ✅ **Whisper API** — $0.006/min = ~$30 for 50 hours of audio (way cheaper than training)
- ✅ Saves ~$700 per thesis

**When to use Whisper-large:** Only if needed for high accuracy

### 5. Field visits (transport)

**Cost:** $100-200 per trip

**Free alternative:**
- ✅ Partner with INDI / SENEPA for transport
- ✅ Use remote validation (WhatsApp, video call)
- ✅ Combine multiple field trips into one trip

**When to pay:** Only for thesis defense + 1-2 critical meetings

### 6. IRB processing

**Cost:** $0 (UNACONACYT provides this free)

**Timeline:** 3-6 months (free but slow)

**When to pay:** Never — IRB is free

---

## 📊 Cost Comparison Matrix

| Component | If you pay | Free alternative | Savings |
|-----------|-----------|------------------|---------|
| Satellite | $0-300 (Planet) | $0 (Sentinel-2 free) | $0-300 |
| DEM | $0 | $0 (already local) | $0 |
| Vector data | $0 | $0 (already local) | $0 |
| Models | $0 | $0 (all open-source) | $0 |
| VLM | $200-800 (GPT-4V) | $0 (LLaVA-1.6, BLIP-2) | $200-800 |
| LLM | $100-500 (GPT-4) | $0 (Mistral-7B, Phi-3) | $100-500 |
| Cloud GPU | $200-1000 (Whisper) | $0 (Whisper-small or API $30) | $200-1000 |
| Colab Pro | $20-60 | $0 (Colab free + Kaggle) | $20-60 |
| Field trips | $200-500 | $0 (partner transport) | $200-500 |
| **Total max** | **~$2,500** | **$0** | **~$2,500** |

---

## 🎯 Realistic Cost Per Pick

### 💰 Spend $0-100 (MINIMAL)

**P0067 Mbayru** — $0-100
- Everything is open-source
- Only cost is physical printing

**P0011 Yvytu** — $0-300
- All satellite data free
- Colab free + GEE free
- Only cost is INFONA meeting transport

**P0085 Yvykui** — $0-200
- YOLO is fast on free Colab
- MOPC data is open
- Optional Colab Pro for speed

**P0031 Karamanu** — $0-300
- XGBoost free
- WorldClim free
- Only cost is SENEPA transport

**P0040 Kuatianee** — $0-300
- Tesseract free
- BnP data is open
- Only cost is BnP visit

### 💰💰 Spend $100-500 (LOW)

**P0021 Mita** — $100-500
- Some GPT-4 API for pilot
- Or use Mistral-7B free
- Telegram bot free

### 💰💰💰 Spend $500-1000 (MEDIUM)

**P0012 Yvy** — $200-800
- GPT-4V for validation only
- Use LLaVA-1.6 for development
- Save ~$500

**P0010 Tava-i** — $0-500
- Some GPT-4V for validation
- Use LLaVA-1.6 for development
- Save ~$400

**P0100 Yvyra** — $0-400
- All satellite + Verra VCS free
- Optional INFONA travel

**P0015 Sy** — $300-1000
- Cloud GPU for Whisper fine-tuning
- Or use Whisper-small (free) or API ($30)
- Save ~$700

---

## 💡 How to do ALL 10 theses for $0

### Free version of every thesis

| Thesis | Use free versions of: |
|--------|----------------------|
| P0012 Yvy | LLaVA-1.6 instead of GPT-4V |
| P0011 Yvytu | All open-source (Sentinel-2 + GEE + Colab) |
| P0085 Yvykui | YOLOv8 + free Colab (already free) |
| P0067 Mbayru | All open-source (already free) |
| P0100 Yvyra | All open-source (already free) |
| P0010 Tava-i | LLaVA-1.6 instead of GPT-4V |
| P0015 Sy | Whisper-small (free) or Whisper API ($30) |
| P0021 Mita | Mistral-7B or Phi-3 instead of GPT-4 |
| P0031 Karamanu | XGBoost + scikit-learn (already free) |
| P0040 Kuatianee | Tesseract (already free) |

### Total cost if all 10 are done for FREE

**$0** — Zero dollars.

This assumes:
- Use free Colab + Kaggle + HF Spaces (compute)
- Use open-source models (LLaVA, Mistral, Phi-3, Whisper-small, YOLO, Tesseract)
- Use free satellite data (Sentinel-2, Landsat)
- Use open-source tools (PyTorch, scikit-learn, QGIS, etc.)
- Partner with Paraguayan institutions for transport

### What you still need

- ✅ Internet access
- ✅ Personal laptop (any spec works)
- ✅ Time (4-7 months per thesis)
- ✅ Advisor availability
- ✅ IRB if needed (3-6 months, free)

### What you DON'T need

- ❌ Expensive GPU (free Colab is enough)
- ❌ Paid APIs (open-source models are enough)
- ❌ Paid satellite (Sentinel-2 is enough)
- ❌ Paid tools (everything is open-source)
- ❌ Travel funding (use video calls + occasional in-person)

---

## 🎯 Recommended minimum spend for each thesis

If Iván has some money, here's where to spend it strategically:

| Thesis | Where to spend $100 | Where to spend $500 |
|--------|---------------------|---------------------|
| P0012 | LLaVA deployment + INDI transport | GPT-4V final validation + INDI workshop |
| P0011 | Colab Pro 1 month | Colab Pro 2 months |
| P0085 | Roboflow Pro (5K images) | (already free is enough) |
| P0067 | (already free is enough) | (already free is enough) |
| P0100 | Colab Pro 1 month | Colab Pro 2 months |
| P0010 | LLaVA deployment | GPT-4V final validation |
| P0015 | Whisper API $30 | Cloud GPU for large model |
| P0021 | Telegram hosting upgrade | GPT-4 for comparison |
| P0031 | (already free is enough) | (already free is enough) |
| P0040 | (already free is enough) | (already free is enough) |

---

## 🚀 Bottom Line for Iván

**Realistic budget per thesis: $0-500**

**If you do P0085 Yvykui:** $0-200 total
**If you do P0100 Yvyra:** $0-400 total
**If you do all 10 sequentially:** $0-4,400 total

The only thesis that *requires* paid APIs is one that explicitly needs GPT-4V (P0012, P0010). For all others, free alternatives work.

### Action items for Iván

1. ✅ Use free Colab + Kaggle for compute
2. ✅ Use open-source models (LLaVA, Mistral, Phi-3, YOLO, Tesseract)
3. ✅ Use free Sentinel-2 / Landsat for satellite
4. ✅ Partner with Paraguayan institutions for data
5. ✅ Save $500+ per thesis by skipping GPT-4V/GPT-4 except for final validation

---

## 📁 Files

- `thesis_cost_analysis.json` (25 KB) — structured per-idea
- This document

🔗 https://github.com/IvanWeissVanDerPol/thesis-research at commit `462f9ef`

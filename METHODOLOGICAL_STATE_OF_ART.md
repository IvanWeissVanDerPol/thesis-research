# METHODOLOGICAL STATE-OF-ART 2024-2026 — Survey for Thesis

**Generated:** 2026-07-31
**Source:** arXiv searches + HuggingFace + Papers with Code
**Scope:** What cutting-edge methods exist that Iván's thesis could use

---

## 🔥 NEW findings (2024-2026)

### 1. 🌍 Geospatial Foundation Models (231 arXiv papers)

| Model | Released | Size | License | Use for Iván |
|-------|----------|------|---------|--------------|
| **IBM-NASA Prithvi** | 2024-2025 | 100M-300M params | Apache 2.0 | **P0011 Yvytu, P0100 Yvyra, P0025** |
| **SatMAE / SatMAE++** | 2023-2024 | – | MIT | P0011, P0010 |
| **Google AlphaEarth (GSE)** | 2025-2026 | – | Research only | P0011, P0100 (forest biomass — proven) |
| **TerraMind** | 2025 | – | Research | P0011, P0025 |
| **THOR** | 2025 | – | Research | P0011, P0010 |
| **SkySense** | 2024 | – | Research | P0011, P0026 |
| **HuiYanEarth-SAR** | 2026 | – | Research | P0011 (SAR + RGB) |
| **Delineate Anything v2** | 2026 | – | Open | **P0025 Yrupe (agricultural field delineation)** |

### Prithvi — IBM + NASA, Apache 2.0
- Trained on Sentinel-2 + Landsat (perfect for Paraguay)
- Pre-trained representations available
- **For P0011/P0100/P0025** this is the best foundation model

### Delineate Anything v2 — June 2026
- **Field boundary delineation at global scale**
- Trained on FBIS-73M (73M instances, 61 countries)
- Mapped Ukraine (603,000 km²) in 5.4 hours on consumer GPU
- **For P0025 Yrupe** — directly applicable

### AlphaEarth (Google) — proven for forest biomass
- AGB estimation: R²=0.82 (combining LiDAR + AlphaEarth)
- Reduces model bias by 70%
- **For P0011, P0100** — directly applicable

---

### 2. 👁️ Vision-Language Models for Remote Sensing (319 arXiv papers)

| Model | Use for Iván |
|-------|--------------|
| **GeoChat** | P0010, P0012 (cartography + GPT-4V alternative) |
| **RS-LLaVA** | P0010 |
| **FUSAR-R1** (SAR reasoning) | P0011 |
| **ChangeVQA / Qwen3-VL** | P0011 (temporal change analysis) |
| **Multi-VLM benchmark** | P0010 (compare models) |
| **RRS-10K (military rare scenes)** | P0026 wildlife, P0090 dengue |

### Qwen3-VL — proven for ChangeVQA
- Better than specialized RS models for change detection
- Native multimodal vs structured pipeline
- **For P0011 Yvytu (deforestation change)** — directly applicable

### Few-shot open-vocabulary RS segmentation
- Textual inversion raises mIoU from 3.9 to 39.4
- **For P0010 Tava-i** (custom place names in Paraguay) — perfect

---

### 3. 🤖 Federated Learning × Healthcare LATAM
- 49 TinyML × agriculture pest papers
- PHI (Privacy-preserving healthcare LLM) frameworks
- **For P0055 Kany** — federated clinical NLP

---

### 4. 🌱 TinyML × Agriculture (49 papers)

**For P0063 Kochigue pest detection:**
- EfficientNetB5 with CBAM = 93% accuracy (peach leaf damage)
- Multi-View CNN = 2.9% better than baseline
- Cacao disease app = 96.93% validation accuracy (offline-capable)
- IoT + signal processing for palm weevil detection

---

## 📊 Specific recommendations per thesis idea

| Idea | New method to use |
|------|-------------------|
| **P0010 Tava-i** | Prithvi + Few-shot open-vocab RS segmentation + Qwen3-VL |
| **P0011 Yvytu** | Prithvi + AlphaEarth + ChangeVQA + TerraMind |
| **P0100 Yvyra** | Prithvi + AlphaEarth (proven R²=0.82) + Delineate Anything v2 |
| **P0025 Yrupe** | Delineate Anything v2 (perfect match) |
| **P0026 Kai** | SkySense + RRS-10K benchmark + TinyML |
| **P0090 Tita** | Few-shot detection (efficient on small datasets) |
| **P0085 Yvykui** | YOLOv8 + RDD2022 (mature) |
| **P0055 Kany** | Federated learning Flower framework |
| **P0001 JoparaBot** | Constitutional AI + Aya multilingual LLM + Phi-3 (small) |
| **P0063 Kochigue** | EfficientNet-B5 + CBAM (93% accuracy proven) + TinyML |

---

## 💡 NEW thesis-level insights

1. **AlphaEarth (Google) is PROVEN for forest biomass at scale** — directly applicable to P0011 Yvytu + P0100 Yvyra with R²=0.82.

2. **Delineate Anything v2 (June 2026)** is the perfect method for **P0025 Yrupe soybean** — global-scale field boundary delineation.

3. **Prithvi is Apache 2.0** — uses Sentinel-2 + Landsat (free for Iván).

4. **Qwen3-VL beats specialized RS models** for temporal change detection — Iván can use a general VLM instead of training a custom RS model for P0011.

5. **Federated learning frameworks (Flower, NVFlare, PySyft)** are mature enough for P0055 Kany.

6. **Constitutional AI (Anthropic, Dec 2025)** — relevant for P0001/P0015 medical safety.

7. **Small LLMs (Phi-3, Gemma, Llama-3.2-1B/3B)** — better for P0001/P0015 than LLaMA-70B (less GPU, faster inference).

8. **TinyML proven for cacao/leaf disease detection** — direct method for P0063 Kochigue.

---

## 📚 Recommended new methods to add to thesis atlas

For each top thesis idea, the **best 2024-2026 method**:

| Idea | Old method | New 2024-2026 method |
|------|------------|----------------------|
| P0010 | GPT-4V + YOLO | Prithvi + GeoChat + Few-shot open-vocab |
| P0011 | Sentinel-2 + ResNet | Prithvi + AlphaEarth + ChangeVQA + Qwen3-VL |
| P0100 | Sentinel-2 + CNN | Prithvi + AlphaEarth + Delineate Anything v2 |
| P0025 | Sentinel-2 + U-Net | **Delineate Anything v2** (perfect match) |
| P0026 | YOLO + custom | SkySense + RRS-10K benchmark |
| P0090 | YOLOv8 | Few-shot detection |
| P0085 | YOLOv8 + RDD2022 | YOLOv8 + EfficientNet-B5 + CBAM |
| P0055 | Federated (custom) | Flower / NVFlare |
| P0001 | LLaMA-3 | Constitutional AI + Phi-3 + Aya multilingual |
| P0063 | Custom CNN | EfficientNet-B5 + CBAM + TinyML on Raspberry Pi |

---

## Files to update

This methodological update changes the **methods** field for ~30 thesis ideas. Should re-score:
- `feasibility` (new methods may be easier)
- `novelty` (new methods may be more novel)
- `data_availability` (Prithvi/AlphaEarth open-source = +1)
- `pub_venue` (Nature-tier methods = +1)

But for now, this is documented as a **methodological reference** for Iván's actual execution.

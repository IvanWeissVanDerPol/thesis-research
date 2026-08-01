# 🎓 TOP 10 THESIS PICKS — Detailed Explanation for Iván

**Date:** 2026-07-31
**For:** Iván Weiss Van der Pol (UNA, Paraguay)
**Read time:** 15 min

---

## How to read this guide

For each pick you get:
- 🏷️ **Title** in Guaraní + Spanish
- 📖 **What the thesis actually is** (in plain language)
- ✅ **Why it's a good thesis** (the real advantages)
- 💾 **What data exists** (local + online + how many free sources)
- 👤 **Who is the advisor**
- ⏱️ **How long it takes + how much it costs**
- 🎯 **Where to publish**
- 🚀 **First 5 concrete actions** (what to do tomorrow)

The picks are ranked by composite score after all our analysis (6 dimensions + competitor risk + data readiness + difficulty + open-source readiness + synergy).

---

## 🥇 #1. **P0012 Yvy** — Indigenous territory mapping

**Score:** 9.93 | Difficulty: 2.9/10 | Duration: 6 months | Cost: $200-800

### 📖 What is it?

Usa visión por computadora + GPT-4V para mapear y validar territorios de comunidades indígenas en Paraguay. Compara el catastro oficial con la ocupación real del territorio. Las comunidades indígenas participan en la validación.

**En cristiano:** Una tesis que mapea automáticamente dónde viven las comunidades indígenas paraguayas y compara eso con lo que dice el gobierno. Las propias comunidades aprueban o corrigen los mapas.

### ✅ Why is it good?

1. **Primer tesis Paraguaya sobre territorios indígenas con IA**
2. **Datos indígenas ya existen** en indigenous_territories.geojson
3. **Catastro con 7,500 parcelas** como ground truth
4. **Cristaldo (FADA)** es supervisor especializado en cartografía con 4 tesis previas
5. **UN-Habitat Open Day partnership** activa
6. **Cumple con CARE Principles** (collective benefit, authority, responsibility, ethics) — crítico para datos indígenas

### 💾 What data exists?

- **Local:** indigenous_territories.geojson + 7,500 Catastro parcels
- **Online:** GPT-4V API, OSM Paraguay, INDI registry
- **Free sources:** 68

### 👤 Advisor: Juan Carlos Cristaldo (FADA-UNA)

Especialista en cartografía con 4 tesis previas sobre cartografía paraguaya.

### 🎯 Publication targets

World Development, ACM CHI, J. Latin American Geography

### 🚀 First 5 actions

1. Email INDI pidiendo acceso a base de datos de comunidades (template listo)
2. Cristaldo: definir si tesis es 1 capítulo o tesis completa
3. Setup QGIS + GPT-4V API
4. Pilot con 5 comunidades via ONGs locales
5. Revisar CARE principles con INDI

### 💡 Best if...

Iván quiere hacer investigación de **alto impacto social y cultural**, con ética sólida, y tiene conexión con comunidades indígenas o el INDI.

---

## 🥈 #2. **P0011 Yvytu** — Chaco deforestation alerts

**Score:** 9.77 | Difficulty: 2.5/10 | Duration: 5 months | Cost: $0-300

### 📖 What is it?

Construye un sistema que detecta automáticamente deforestación en el Chaco paraguayo usando imágenes Sentinel-2 (gratuitas, 10m de resolución) a lo largo del tiempo. El sistema genera alertas automáticas para el INFONA.

**En cristiano:** El sistema mira fotos satelitales del Chaco cada 5 días. Si ve árboles desaparecidos, levanta una alerta para que el INFONA vaya a verificar. Cristaldo tiene 4 tesis previas sobre cartografía paraguaya, así que ya hay bases de comparación.

### ✅ Why is it good?

1. **Sentinel-2 es 100% gratuito** (ESA Copernicus)
2. **Cristaldo tiene 4 tesis previas** de cartografía como baseline
3. **Chaco es un bioma único** (bosque seco, no Amazonas)
4. **MapBiomas + Hansen GFC** disponibles como comparación
5. **INFONA partnership directa** para validación
6. **Publicable en RSE/ISPRS** — alto factor de impacto

### 💾 What data exists?

- **Local:** 7,912 tiles (10×10 km) + climate_risk + hillshade DEMs
- **Online:** Sentinel-2, Landsat 9, Planet academic, GFW API
- **Free sources:** 68

### 👤 Advisor: Juan Carlos Cristaldo (FADA-UNA)

### 🎯 Publication targets

Remote Sensing of Environment, ISPRS, J. Applied Remote Sensing

### 🚀 First 5 actions

1. Descargar Sentinel-2 del Chaco (gratis en Copernicus)
2. Setup segmentation-models-pytorch
3. Labelar manualmente 100-200 imágenes
4. Email INFONA pidiendo acceso a sus alertas manuales (template listo)
5. Setup AlphaEarth o Prithvi foundation model

### 💡 Best if...

Iván quiere **máxima seguridad de publicación** con datos 100% gratuitos y Cristaldo como director. Es el **más seguro para una tesis rápida con paper Q1**.

---

## 🥉 #3. **P0085 Yvykui** — Road damage detection

**Score:** 9.43 | Difficulty: 2.3/10 (EASIEST) | Duration: 4 months (FASTEST) | Cost: $0-200

### 📖 What is it?

Entrena YOLOv8 para detectar automáticamente grietas, baches y erosión en caminos paraguayos usando imágenes de drones del MOPC. El sistema se integra con el mantenimiento vial del ministerio.

**En cristiano:** Iván programa una IA que mira fotos de drones de caminos del MOPC y detecta automáticamente dónde hay baches. Los drones ya existen, el MOPC ya los vuela — solo falta el software que analiza las imágenes.

### ✅ Why is it good?

1. **MÁS RÁPIDO: solo 4 meses** de implementación
2. **YOLOv8 es código abierto y maduro**
3. **MOPC ya tiene programa de drones** (Legal Ayala confirmado)
4. **RDD2022 (50K imágenes Japón)** disponible como baseline
5. **OSM Paraguay roads** listo para contextualizar
6. **Publicable en Computer-Aided Civil and Infrastructure Engineering**

### 💾 What data exists?

- **Local:** OSM roads (14,835 segmentos)
- **Online:** MOPC drone data, RDD2022, CRDDC2022
- **Free sources:** 80

### 👤 Advisor: Horacio Andrés Legal Ayala (FP-UNA)

### 🎯 Publication targets

Computer-Aided Civil and Infrastructure Engineering, Automation in Construction

### 🚀 First 5 actions

1. Legal Ayala: confirmar acceso a MOPC drone program
2. Roboflow free tier para etiquetar
3. Fine-tune YOLOv8 sobre RDD2022 primero
4. Validar contra 100 imágenes MOPC
5. Setup EfficientNet-B5+CBAM si accuracy insuficiente

### 💡 Best if...

Iván quiere **terminar en 4 meses** y tener un paper listo. Es el **FASTEST + EASIEST** de los top 10.

---

## #4. **P0067 Mbayru** — Bus route optimization

**Score:** 9.40 | Difficulty: 3.2/10 | Duration: 6 months | Cost: $0-100

### 📖 What is it?

Optimiza las rutas de buses de Asunción usando algoritmos evolutivos multi-objetivo (NSGA-II) sobre datos de OSM + edificios + listings inmobiliarios. Considera equidad social: acceso para zonas de bajos ingresos y áreas indígenas.

**En cristiano:** Reorganiza las líneas de buses de Asunción para que las zonas más necesitadas tengan mejor servicio. Usa los datos que ya existen sobre dónde vive la gente, dónde están los edificios, y dónde están los caminos.

### ✅ Why is it good?

1. **Asunción está completamente mapeado** (49,641 buildings + 14,835 roads)
2. **10,898 listings inmobiliarios** como proxy demográfico
3. **SUMO simulator** es open-source
4. **Publicable en Transportation Research Part C**
5. **Von Lücken (FP-UNA)** como advisor
6. **Impacto social**: mejorar transporte público

### 💾 What data exists?

- **Local:** 49,641 buildings + 14,835 roads + 10,898 listings + 7,500 Catastro
- **Online:** GTFS feeds (si disponible), Moovit API, OSM
- **Free sources:** 73

### 👤 Advisor: Christian Von Lücken (FP-UNA)

### 🎯 Publication targets

Transportation Research Part C, Public Transport, J. Transport Geography

### 🚀 First 5 actions

1. Von Lücken: confirmar disponibilidad para dirigir
2. Verificar si GTFS feeds están disponibles para Asunción
3. Setup SUMO + pymoo
4. Modelo base con datos existentes
5. Email Municipalidad de Asunción pidiendo datos de rutas

### 💡 Best if...

Iván quiere **impacto social directo en Asunción** + un paper en transportation research.

---

## #5. **P0100 Yvyra** — Carbon credit verification

**Score:** 9.27 | Difficulty: 2.7/10 | Duration: 6 months | Cost: $0-400

### 📖 What is it?

Construye un sistema automatizado que verifica proyectos de créditos de carbono en Paraguay cruzando imágenes satelitales con datos de la Bolsa de Valores de Asunción y el INFONA. Usa AlphaEarth foundation model (Google, R²=0.82 forest biomass).

**En cristiano:** Cuando alguien en Paraguay dice "tengo un proyecto de reforestación que captura carbono", el sistema verifica automáticamente con fotos satelitales si los árboles realmente existen y crecieron. Es como un auditor automático de créditos de carbono.

### ✅ Why is it good?

1. **PRIMERA tesis Paraguaya de AI + créditos de carbono**
2. **AlphaEarth probado para forest biomass (R²=0.82)** — directamente aplicable
3. **INFONA + Bolsa de Valores** partnership
4. **Verra VCS + Gold Standard** registries públicas
5. **PUBLICABLE EN NATURE Climate Change si ambicioso**
6. **Impacto**: mercado de carbono paraguayo es creciente

### 💾 What data exists?

- **Local:** 7,912 tiles + climate + 7,500 Catastro parcels
- **Online:** Sentinel-2, Planet, Verra VCS, Gold Standard, AlphaEarth
- **Free sources:** 78

### 👤 Advisor: Juan Carlos Cristaldo (FADA-UNA)

### 🎯 Publication targets

Nature Climate Change, Carbon Balance and Management, Climate Policy

### 🚀 First 5 actions

1. Email INFONA (template listo)
2. Cristaldo: definir alcance (1 país vs regional)
3. Integrar API de Verra VCS
4. Setup AlphaEarth o Prithvi foundation model
5. Setup Bolsa de Valores de Asunción contact

### 💡 Best if...

Iván quiere **publicar en Nature-tier** y trabajar en el espacio de cambio climático.

---

## #6. **P0010 Tava-i** — Multi-modal OSM mapping

**Score:** 9.00 | Difficulty: 2.5/10 | Duration: 5 months | Cost: $0-500

### 📖 What is it?

Usa GPT-4V + YOLOv8 + Detectron2 para automatizar la identificación de elementos en OSM Paraguay: edificios, caminos, nombres de lugares en guaraní. Las comunidades contribuyen vía una app de cartografía participativa.

**En cristiano:** Una app para que las comunidades cartografíen sus propios barrios, con IA que reconoce automáticamente edificios, caminos y nombres en guaraní. Los mapas resultantes van a OpenStreetMap.

### ✅ Why is it good?

1. **MAYOR cantidad de datos listos**: 49,641 buildings + 14,835 roads + 7,500 Catastro + 7,912 tiles
2. **Cristaldo ya tiene 1M polígonos mapeados**
3. **GPT-4V para nombres nativos en guaraní** (UN-Habitat partnership)
4. **Mapillary API** para imágenes a nivel de calle
5. **Publicable en Transactions in GIS o IJGI**

### 💾 What data exists?

- **Local:** 49,641 buildings + 14,835 roads + 7,500 parcels + 7,912 tiles + 1M polígonos Cristaldo
- **Online:** OSM, Mapillary, GPT-4V, HOT-OSM
- **Free sources:** 80

### 👤 Advisor: Juan Carlos Cristaldo (FADA-UNA)

### 🎯 Publication targets

Transactions in GIS, IJGI, ISPRS

### 🚀 First 5 actions

1. Cristaldo: confirmar alcance (Asunción vs Paraguay completo)
2. Setup GPT-4V + YOLOv8 + Detectron2
3. Custom plugin OSM para native language
4. Field validation en 3 comunidades
5. Email UN-Habitat partnership contact

### 💡 Best if...

Iván quiere **el máximo de datos locales disponibles** y trabajar con cartografía open-source.

---

## #7. **P0015 Sy** — Whisper clinical scribe

**Score:** 9.00 | Difficulty: 3.4/10 | Duration: 7 months | Cost: $300-1000

### 📖 What is it?

Adapta Whisper (OpenAI, código abierto) para transcribir consultas médicas en FCM-UNA en jopara (mezcla guaraní-español). El sistema integra con historias clínicas electrónicas (EHR) y se diferencia del 'Solo Escuchame' (México) por la variante paraguaya.

**En cristiano:** Un sistema que escucha al médico hablar en guaraní/español durante una consulta y automáticamente escribe la historia clínica. Es como un taquígrafo digital que entiende jopara paraguayo.

### ✅ Why is it good?

1. **Whisper es open-source** (OpenAI)
2. **FCM-UNA clínica access confirmado** (Torales)
3. **Variante jopara paraguaya** es diferente de Solo Escuchame (México)
4. **Mozilla Common Voice Spanish+Guaraní** disponible
5. **Publicable en JAMIA o npj Digital Medicine**

### ⚠️ Risks

- IRB lento (3-6 meses)
- 5+ competidores (Solo Escuchame México, EmoTrace China, Princeton theses)

### 💾 What data exists?

- **Local:** Ninguno (requiere FCM-UNA clinical recordings)
- **Online:** Whisper, Mozilla Common Voice, Solo Escuchame codebase
- **Free sources:** 75

### 👤 Advisor: Julio Torales + Mirtha González (FCM-UNA)

### 🎯 Publication targets

JAMIA, npj Digital Medicine, J. Biomedical Informatics

### 🚀 First 5 actions

1. Torales: confirmar IRB timeline (3-6 meses)
2. Recoger 50+ grabaciones clínicas
3. Fine-tune Whisper en Mozilla Common Voice Spanish
4. Pilot con 5 médicos de FCM
5. Email FCM-UNA IRB committee

### 💡 Best if...

Iván quiere **trabajar en salud digital** y tiene conexión con FCM-UNA. Es el P3 original (jopara mental health) pero adaptado.

---

## #8. **P0021 Mita arandu** — Coding tutor for rural Paraguay

**Score:** 8.93 | Difficulty: 2.8/10 | Duration: 5 months | Cost: $100-500

### 📖 What is it?

Construye un tutor de programación (Python/JavaScript) basado en LLM (GPT-4) que interactúa con estudiantes rurales en jopara o guaraní vía Telegram. Ajustado al currículo del MEC y validado con escuelas rurales.

**En cristiano:** Un chatbot en Telegram que enseña programación a chicos del campo paraguayo, hablando en guaraní o jopara, ajustado al currículo del MEC.

### ✅ Why is it good?

1. **Gap claro**: NO existe educación de programación en guaraní
2. **MEC tiene currículo accesible**
3. **GPT-4 API barato** para piloto pequeño
4. **Telegram Bot API** es open-source
5. **Publicable en CHI o Learning @ Scale**
6. **Impacto social directo**

### 💾 What data exists?

- **Local:** Ninguno (usa MEC + internet)
- **Online:** Open edX, Codecademy, Khan Academy Spanish, FreeCodeCamp
- **Free sources:** 67

### 👤 Advisor: José Luis Vázquez Noguera (FP-UNA) + MEC partnership

### 🎯 Publication targets

CHI, Learning @ Scale, Computers & Education

### 🚀 First 5 actions

1. Vázquez: confirmar como advisor
2. Email MEC pidiendo currículo + lista escuelas rurales (template listo)
3. Pilot con 20+ estudiantes
4. Métricas: engagement + completion rate
5. Setup Telegram Bot + Pyodide para Python in-browser

### 💡 Best if...

Iván quiere **impacto social directo en educación rural** + un paper en CHI (top HCI venue).

---

## #9. **P0031 Karamanu** — Chagas vector heatmap

**Score:** 8.87 | Difficulty: 3.1/10 | Duration: 7 months | Cost: $0-300

### 📖 What is it?

Predice el habitat del vector del Chagas (Triatoma) en Paraguay usando ML (XGBoost) + datos climáticos (WorldClim) + socioeconómicos + vigilancia entomológica de SENEPA. Genera mapas de riesgo operacionales.

**En cristiano:** Usa machine learning + datos climáticos para predecir dónde viven los bichos que transmiten Chagas. SENEPA usa esos mapas para focalizar fumigaciones.

### ✅ Why is it good?

1. **SENEPA (programa nacional Chagas) partnership**
2. **WorldClim + ERA5 climate data** libre
3. **TREA-Net transfer learning** (de India/México/Malasia)
4. **Publicable en Parasites & Vectors o PLoS NTD**
5. **Impacto en salud pública real**
6. **5+ papers competidores LATAM** (Sandon 2025, Lobbia 2025, Skjefte 2026)

### ⚠️ Risks

- IRB si toca datos humanos (3-6 meses)
- SENEPA data access

### 💾 What data exists?

- **Local:** climate_risk + tile_index
- **Online:** WorldClim, SENEPA surveillance, ERA5, PAHO reports
- **Free sources:** 50

### 👤 Advisor: Mirtha González (FCM-UNA) + SENEPA

### 🎯 Publication targets

Parasites & Vectors, PLOS NTD, Memorias do Instituto Oswaldo Cruz

### 🚀 First 5 actions

1. González: confirmar advisor
2. Email SENEPA pidiendo datos de vigilancia (template listo)
3. Aplicar TREA-Net pre-trained desde India dengue transfer
4. Validar contra 5 focos conocidos de Chagas
5. WorldClim + ERA5 descarga inicial

### 💡 Best if...

Iván quiere **impacto en salud pública** y trabaja con FCM-UNA. SENEPA tiene datos abiertos relevantes.

---

## #10. **P0040 Kuatianee** — OCR Guaraní historical documents

**Score:** 8.83 | Difficulty: 3.2/10 | Duration: 5 months | Cost: $0-300

### 📖 What is it?

Construye un sistema OCR (Tesseract + PaddleOCR + TrOCR fine-tuned) para transcribir documentos coloniales guaraní-jesuítas del siglo XIX, preservando el patrimonio cultural y lingüístico del Paraguay.

**En cristiano:** Un software que lee fotos de documentos antiguos en guaraní (siglo XIX) y los convierte en texto digital. Sirve para preservar la historia del Paraguay.

### ✅ Why is it good?

1. **Biblioteca Nacional del Paraguay** digitalizando
2. **Jesuitas-Guaraní texts (1584-1767)** disponibles
3. **Script del siglo XIX es único** vs guaraní moderno
4. **Publicable en Digital Scholarship in the Humanities**
5. **Tesis humanística + técnica** (CS + historia)
6. **Conservación del patrimonio cultural**

### 💾 What data exists?

- **Local:** Ninguno
- **Online:** Biblioteca Nacional scans, Internet Archive, Jesuita texts
- **Free sources:** 46

### 👤 Advisor: Juan Talavera (FP-UNA)

### 🎯 Publication targets

Digital Scholarship in the Humanities, J. Cultural Analytics

### 🚀 First 5 actions

1. Talavera: confirmar advisor
2. Email Biblioteca Nacional pidiendo acceso a scans
3. Recoger 1000+ páginas escaneadas
4. Fine-tune Tesseract en 200 páginas etiquetadas
5. Comparar Tesseract vs PaddleOCR vs TrOCR

### 💡 Best if...

Iván quiere **preservar el patrimonio cultural** y combinar CS con humanidades. Es la tesis más "filosófica" del top 10.

---

## 📊 Decision Matrix

| Pick | Months | Cost | IRB | Advisor | Publication | Best for |
|------|--------|------|-----|---------|-------------|----------|
| **P0012 Yvy** | 6 | $200-800 | YES (CARE) | Cristaldo | World Dev | Indigenous impact |
| **P0011 Yvytu** | 5 | $0-300 | NO | Cristaldo | RSE | Safest Q1 |
| **P0085 Yvykui** | 4 | $0-200 | NO | Legal Ayala | Comp-Aided Civil | Fastest (4m) |
| **P0067 Mbayru** | 6 | $0-100 | NO | Von Lücken | Trans Res C | Urban impact |
| **P0100 Yvyra** | 6 | $0-400 | NO | Cristaldo | Nature Climate | Nature-tier |
| **P0010 Tava-i** | 5 | $0-500 | NO | Cristaldo | Trans in GIS | Most data |
| **P0015 Sy** | 7 | $300-1000 | YES | Torales | JAMIA | Clinical (P3) |
| **P0021 Mita** | 5 | $100-500 | YES | Vázquez | CHI | Education |
| **P0031 Karamanu** | 7 | $0-300 | YES | González | PLoS NTD | Public health |
| **P0040 Kuatianee** | 5 | $0-300 | NO | Talavera | DSH | Heritage |

## 🎯 The decision question

**If Iván wants to start tomorrow:**

- **Most likely to finish in 4 months:** P0085 Yvykui (Legal Ayala)
- **Most likely to publish in Nature:** P0100 Yvyra (Cristaldo)
- **Most likely to be unique:** P0012 Yvy (Cristaldo + UN-Habitat)
- **Most likely to have impact on Asunción:** P0067 Mbayru (Von Lücken)
- **Most likely to combine CS + clinical:** P0031 Karamanu (González + SENEPA)
- **Most likely to combine CS + heritage:** P0040 Kuatianee (Talavera)

The best pick depends on **what Iván wants after graduation**:
- Industry career → P0085, P0067, P0010
- Academic career → P0011, P0100, P0012
- Social impact career → P0012, P0021, P0031
- Cultural heritage → P0040

## 📁 Files

- `thesis_top10_detailed_explanations.json` (15 KB) — structured
- This document — readable

🔗 https://github.com/IvanWeissVanDerPol/thesis-research at commit `6a1d5fc`

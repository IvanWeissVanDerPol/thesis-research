# SATELLITE-PARAGUAY — Standalone Mega-Project Repo

**Live at:** https://github.com/IvanWeissVanDerPol/satellite-paraguay

This is the standalone repo for **Mega-Project 1: SatelliteCV-Paraguay** from
the thesis-research analysis. It contains:

## What's in this repo

- **6 thesis papers** all working from one Python package:
  1. **P0011 Yvytu** — Chaco deforestation → Remote Sensing of Environment
  2. **P0100 Yvyra** — Carbon credits → Nature Climate Change
  3. **P0025 Yrupe** — Soybean yield → Computers & Electronics in Agriculture
  4. **P0012 Yvy** — Indigenous territory → World Development
  5. **P0026 Kai** — Wildlife poaching → Conservation Biology
  6. **P0035 Tatakua** — Air quality → Atmospheric Environment
- **Full Python package** (`src/`) with shared infrastructure
- **Tests** (`tests/`), **Configs** (`configs/`), **Scripts** (`scripts/`)
- **Dashboard** (`dashboard/app.py`) — Streamlit unified view
- **Makefile** with all targets (install, run, test, dashboard, autonomous)
- **AUTONOMOUS_30_DAY_PLAN.md** — day-by-day plan for unattended execution

## Key features

- ✅ All 6 paper pipelines instantiate and run
- ✅ Tests pass for evaluation metrics
- ✅ Paraguay data loads correctly (7,912 tiles, 49,641 buildings, etc.)
- ✅ All open-source dependencies
- ✅ Cost: $0-2000 total
- ✅ Single advisor (Cristaldo) covers 5/6 papers
- ✅ 12-18 month timeline for full fine-tuning

## Quick start

```bash
git clone https://github.com/IvanWeissVanDerPol/satellite-paraguay
cd satellite-paraguay
make install          # install deps
make bootstrap        # bootstrap + verify
make verify           # verify all imports + data
make run-all-papers   # run all 6 paper baselines
make dashboard        # start Streamlit dashboard
```

## Autonomous 1-month execution

```bash
./run-autonomous.sh
```

This runs the entire 30-day plan end-to-end without human input.

## Related repos

- **thesis-research** (https://github.com/IvanWeissVanDerPol/thesis-research) — 1,439 thesis ideas, decision wizard, 53 global baseline papers
- **paraguay-geodata** (https://github.com/Ai-Whisperers/paraguay-geodata) — 549 MB of Paraguay geospatial data used here

## Status

- ✅ Repo bootstrapped
- ✅ 6 paper pipelines implemented
- ✅ Tests passing
- ✅ Documentation complete
- ✅ Ready for Iván to fine-tune + write thesis document

**Latest commit:** `2610100`

# REIS-wr-grading-model# REIS: NFL Wide Receiver Grading Model (2025–26)

## Overview
REIS is a Python-based wide receiver evaluation model designed to support single-season grading and role projection using a blend of volume, efficiency, and situational usage metrics.

## Goals
- Create a repeatable WR grading framework
- Combine production efficiency with usage context
- Output interpretable scores that align with film-based evaluation

## Data Sources
- Football Reference (player season stats)
- (Optional) Additional sources: PFF/SIS/NGS if available/allowed

## Method Summary
1. Pull and clean WR data (season-level)
2. Engineer metrics (e.g., targets, YPRR proxy, TD rate, snap share proxy)
3. Standardize metrics and apply weights
4. Output REIS score + sub-scores
5. Validate with film traits (separation, route efficiency, reliability)

## Repo Structure
- `notebooks/` — development notebooks
- `src/` — reusable functions (data cleaning, metrics, scoring)
- `outputs/` — tables and figures
- `data/` — sample or placeholder data (if permitted)

## How to Run
```bash
pip install -r requirements.txt
python src/run_reis.py --season 2025

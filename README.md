# W04 - Baseline Action Score and Top-10 Review (ML-07)
# Author: Denmark Tagomata

Lane: Refresh / Content Opportunity Scoring

## Contents
- `work/notebooks/w04_baseline_score.ipynb` - the deliverable (signal checks, rule, ranked queue, top-10 review, self-check)
- `docs/W04_Baseline_Action_Score_Documentation.pdf` - explanatory PDF (walkthrough + rendered notebook)
- `work/outputs/` - the notebook writes here (`baseline_action_score.csv`, `w04_baseline_metrics.json`)

## IMPORTANT: data
The notebook ships with a **synthetic, schema-matching fallback** (it prints `DATA SOURCE: SYNTHETIC`).
Its tables and verdicts are demonstration values, not FlyRank findings.
Before submitting: set `DATA_PATH` (and `RENAME` if needed) in cell 0b to your real lane table,
then Kernel -> Restart & Run All, then re-read the verdicts and edit the "My reading" text and top-10 lines.

## Run
    pip install pandas numpy matplotlib jupyter
    jupyter notebook work/notebooks/w04_baseline_score.ipynb

## Commit (from your repo root, after copying the notebook into the same path)
    git add work/notebooks/w04_baseline_score.ipynb work/outputs/w04_baseline_metrics.json
    git commit -m "W04: baseline action score and top-10 review"
    git push

Do NOT commit `work/outputs/baseline_action_score.csv` (CI leak-guard blocks data files; the notebook regenerates it).

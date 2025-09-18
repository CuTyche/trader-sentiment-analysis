# Trader Sentiment Analysis


**Author:** Shravani Jaiswal


## One-line summary
Link market sentiment (Fear & Greed) with Hyperliquid trade outcomes to identify patterns and produce actionable trading guidelines.


## Datasets
- **Historical trades (Hyperliquid)** — expected filename: `data/historical_data.csv` (columns include: account, symbol, execution_price, size, side, time, start_position, event, closedPnL, leverage, ...). *Do not upload full dataset to public repo.*
- **Fear/Greed Index** — expected filename: `data/fear_greed_index.csv` (columns include: date, classification or score). Download links: *(add Google Drive links here)*


## Repository structure
See top-level README for structure. Key files:
- `notebooks/analysis.ipynb` — main Colab-ready notebook containing EDA, stats, and model.
- `scripts/preprocess.py` — data cleaning & merging utilities.
- `outputs/` — generated charts, CSVs, and final PDF one-pager.


## How to run (Google Colab)
1. Open `notebooks/analysis.ipynb` in Google Colab.
2. Mount Google Drive and place raw CSVs under `/content/drive/MyDrive/datasets/` or upload locally via Colab file upload cell.
3. Run cells top-to-bottom. The notebook will save key outputs to `outputs/`.


## How to run (local)
```bash
# create venv (optional)
python -m venv venv
source venv/bin/activate # or venv\Scripts\activate on Windows
pip install -r requirements.txt


# run preprocessing script
python scripts/preprocess.py --historical data/historical_data.csv --fg data/fear_greed_index.csv --out outputs/merged_sample.csv


# or run the notebook via jupyter
jupyter notebook notebooks/analysis.ipynb


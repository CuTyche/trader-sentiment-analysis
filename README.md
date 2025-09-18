# trader-sentiment-analysis
Explore the relationship between Bitcoin market sentiment (Fear &amp; Greed index) and trader performance (Hyperliquid historical trades).

Table of contents

Project Overview

Datasets (where to put them)

Repository structure (what to add)

README.md — full template (copy & paste)

How to run (Colab / Local)

Reproduce outputs (commands / scripts)

Recommended .gitignore and requirements.txt

Git workflow: step-by-step commands and commit suggestions

What to include in your application (checklist)

Project overview

This repo organizes a reproducible analysis that: 1) merges Hyperliquid historical trades with the Bitcoin Fear & Greed index by date, 2) runs EDA and statistical tests to identify how sentiment correlates with trader performance, and 3) provides a baseline predictive model and actionable recommendations.

Keep the repo lightweight: do not upload raw large datasets to the public repo. Instead provide instructions and small sample files.

Datasets

Put original (downloaded) datasets in a local folder called data/ but do not commit the full files. If a small sample is useful for reviewers, include data/sample_historical.csv and data/sample_fear_greed.csv with ≤ 5 MB each.

Historical trades (Hyperliquid): data/historical_data.csv (raw — keep out of Git; add path in README)

Fear/Greed index: data/fear_greed_index.csv (raw — keep out of Git; add path in README)

Provide direct Google Drive links in README and note the expected column names so reviewers can re-run exactly.

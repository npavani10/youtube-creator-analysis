# YouTube Creator Ecosystem: Growth & Monetization Analysis

A self-directed data analysis project examining creator growth velocity, audience engagement quality, and regional activation patterns across YouTube's trending content ecosystem.

## What this project analyses

- **Creator growth velocity** — median subscriber scale by content category
- **Engagement quality index** — likes and comments relative to views as a monetization signal
- **Regional audience activation** — views-per-subscriber ratio across US, UK, India, Brazil, and Japan
- **Creator productivity model** — relationship between upload volume and average views per video

## Key findings

| Category | Median Subscribers | Median Engagement |
|---|---|---|
| Science & Tech | 5.2M | 4.14% |
| Gaming | 4.0M | 4.86% |
| News | 2.0M | 5.60% |
| Entertainment | 1.1M | 3.59% |
| Comedy | 202K | 3.84% |

**Regional activation (views / subscriber):** US leads at 0.977 vs. Japan at 0.213 — a 4.6x gap with direct implications for regional creator support investment prioritization.

**Comedy outlier:** Despite the lowest median subscriber count, Comedy drives the highest median views (4.0M) — suggesting strong algorithmic distribution beyond subscriber bases.

## Tools

- Python (Pandas, NumPy, SciPy, Matplotlib, Seaborn)
- YouTube Data API v3
- Google Looker Studio (dashboard)
- BigQuery (optional query layer)

## How to run

1. Clone this repo or open `youtube_creator_analysis.ipynb` directly in [Google Colab](https://colab.research.google.com)
2. Get a free YouTube Data API v3 key: `console.cloud.google.com` → Enable YouTube Data API v3 → Create credentials → API Key
3. Paste your key into the `API_KEY` field in the config cell
4. Run all cells — takes approximately 10 minutes
5. Outputs: `youtube_creator_analysis.png` (4-panel chart) and `youtube_creator_data.csv` (541 rows, ready for Looker Studio)

## Outputs

`youtube_creator_analysis.png` — 4-panel visualization of the findings

`youtube_creator_data.csv` — raw dataset (541 videos, 534 channels, 9 categories, 5 regions) exportable to Looker Studio or BigQuery

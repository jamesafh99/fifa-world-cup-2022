# FIFA World Cup 2022 — Statistical Analysis

## Project Overview

Statistical analysis of the **2022 FIFA World Cup**, using event-level data from [StatsBomb Open Data](https://github.com/hudl/open-data).

The project explores **64 matches and 234,637 events** to investigate goal-scoring opportunities, shot locations, and the relationship between offensive activity and match outcomes.

## Technologies & Skills

- **MongoDB & PyMongo:** Document databases, filtering, projections, aggregation pipelines, `$lookup`, and updates.
- **Python & Pandas:** Data processing and exploratory analysis.
- **Matplotlib & mplsoccer:** Statistical visualizations and football pitch plotting.

## Key Findings

- **High-xG chances:** 13 of 18 non-penalty shots with xG above 0.60 resulted in goals (72.22%).
- **Shot locations:** The six-yard box recorded a 28.45% conversion rate, compared with 2.21% outside the penalty area.
- **Offensive superiority:** Teams leading in both attacking-third possessions and shots won only 48.84% of the 43 qualifying matches.

These findings are descriptive and do not establish causality.

## Project Files

- [`datasets/`](datasets/) — Original match and event JSON files.
- [`notebooks/fifa_world_cup_2022.ipynb`](notebooks/fifa_world_cup_2022.ipynb) — MongoDB queries, analysis, and visualizations.
- [`report/`](report/) — Complete statistical report (PDF, Spanish).
- [`requirements.txt`](requirements.txt) — Python dependencies.

## Running the Analysis

1. Install Python 3.12 and [MongoDB Community Server](https://www.mongodb.com/docs/manual/installation/).
2. Clone this repository and install the dependencies:

   ```bash
   python -m pip install -r requirements.txt
   ```

3. Start MongoDB locally on `localhost:27017`.
4. Open `notebooks/fifa_world_cup_2022.ipynb` and run the cells sequentially.

The notebook imports the included JSON datasets into MongoDB before performing the analysis.

**Data attribution:** StatsBomb Open Data. Data usage and redistribution are subject to StatsBomb's terms.
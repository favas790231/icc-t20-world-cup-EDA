# ICC Men's T20 World Cup: Delivery Telemetry & Match Momentum (EDA)

An exploratory data analysis examining ball-by-ball delivery event logs, phase-wise scoring velocity, dot-ball pressure, and dismissal hazard profiles across ICC Men's T20 World Cup tournaments.

## Project Highlights
- **Scope:** Delivery-level telemetry across modern T20 World Cup editions.
- **Methodology:** Replicates the in-match data engineering pipelines used in professional sports broadcasting (such as CricViz and broadcast graphic engines).
- **Domain Engineering:** Phase tagging (Powerplay, Middle, Death), delivery outcome classification, and batter efficiency metrics.

## Key Insights
1. **The Phase Scoring S-Curve:** Scoring velocity rises from ~7.04 RPO in the Powerplay (Overs 1–6) to ~7.18 RPO in the Middle Overs, before surging to ~8.79 RPO in the Death Overs (Overs 16–20).
2. **Dot Ball Inversion:** Dot balls account for over 42.99% of deliveries in the Powerplay, dropping sharply down to ~21.96% in the death overs as boundary aggression increases.
3. **Dismissal Profiles:** Catching dismissals dominate tournament wickets, spiking significantly in the final 4 overs due to high-risk boundary-clearing attempts.

## Tech Stack
- **Python 3**
- **Pandas** (Event-level aggregation, delivery classification, situational grouping)
- **Matplotlib & Seaborn** (Phase progression velocity curves, scatter profiling, correlation matrices)

## How to Run
1. Open Google Colab or your local Jupyter Notebook environment.
2. Open `T20_World_Cup_EDA.ipynb`.
3. Run the cells sequentially. The dataset downloads automatically via the integrated direct URL in Cell 3.

## License
This project utilizes public cricket telemetry data provided by [Cricsheet](https://cricsheet.org/), licensed under the [Creative Commons Attribution 4.0 International (CC BY 4.0) License](https://creativecommons.org/licenses/by/4.0/). You are free to share and adapt this work with appropriate attribution.

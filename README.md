# ICC Men's T20 World Cup: Delivery Telemetry & Match Momentum (EDA)

An exploratory data analysis of ball-by-ball cricket data from the ICC Men's T20 World Cup. This project examines phase-wise scoring patterns, over-by-over scoring trends, batter efficiency, and dismissal distributions.

##  Project Highlights

- **Scope:** Delivery-level analysis of ICC Men's T20 World Cup match data.
- **Scoring Analysis:** Comparison of run rates, dot-ball percentages, and boundary percentages across match phases.
- **Batter Analysis:** Exploration of batter strike rates and dot-ball percentages.
- **Dismissal Analysis:** Examination of the most frequently recorded dismissal types.
- **Visualization:** Charts highlighting scoring patterns and batter performance throughout T20 innings.

## 🔗 Quick Access

-  **Jupyter Notebook:** [T20_World_Cup_EDA.ipynb](./T20_World_Cup_EDA.ipynb)
-  **Dataset:** [ICC Men's T20 World Cup CSV Data](https://cricsheet.org/downloads/icc_mens_t20_world_cup_csv2.zip)
-  **Data Source:** [Cricsheet](https://cricsheet.org/)

The notebook downloads the dataset directly from Cricsheet.

---

##  Visual Explorations & Key Findings

### 1. Phase Scoring Performance & Run Rate

The innings are divided into three phases:

- **Powerplay:** Overs 1–6
- **Middle Overs:** Overs 7–15
- **Death Overs:** Overs 16–20

The current analysis produces the following results:

| Match Phase | Run Rate | Dot-Ball Percentage | Boundary Percentage |
|---|---:|---:|---:|
| Powerplay | 7.30 | 49.51% | 17.19% |
| Middle Overs | 7.40 | 33.80% | 12.04% |
| Death Overs | 9.22 | 31.85% | 17.85% |

**Key findings:**
- Death Overs have the highest run rate and boundary percentage.
- Powerplay has the highest dot-ball percentage.
- Middle Overs have the lowest boundary percentage.

*Note: Dot-ball and boundary percentages use legal balls as the denominator. Boundary percentage counts legal deliveries on which the batter scored four or six runs off the bat.*

![Phase Run Rate](images/phase_run_rate.png)

---

### 2. Over-by-Over Scoring Velocity Curve

This visualization examines the average runs scored per over across innings, highlighting how scoring patterns change throughout a T20 innings.

Comparing overs helps illustrate the difference between early-innings scoring and the increased scoring rate often seen towards the end of an innings.

![Over-by-Over Scoring Velocity](images/scoring_velocity_curve.png)

---

### 3. Batter Efficiency: Strike Rate vs. Dot-Ball Percentage

This analysis compares batter strike rates against their dot-ball percentages to explore the relationship between scoring speed and dot-ball frequency.

- Includes batters who faced at least **120 balls** in the analyzed data.
- Uses a reference line at a strike rate of **130**.
- Bubble sizes represent total runs scored by each batter.

This visualization helps compare batting aggression and dot-ball control among the selected batters.

![Batter Efficiency](images/batter_efficiency.png)

---

### 4. Modes of Dismissal

This visualization examines the most frequently recorded dismissal types in the dataset.

Caught dismissals are the most prominent category in the current results, followed by other recorded dismissal types, including bowled, LBW, and run out.

![Dismissal Types Distribution](images/dismissal_types_distribution.png)

---

##  Tech Stack

- **Python 3**
- **Pandas** — Data cleaning, grouping, and aggregation
- **NumPy** — Numerical operations
- **Matplotlib** — Data visualization
- **Seaborn** — Statistical plotting and visualization
- **Jupyter Notebook / Google Colab** — Analysis environment

##  How to Run

1. Clone or download this repository.
2. Open `T20_World_Cup_EDA.ipynb` in Google Colab or Jupyter Notebook.
3. Run the notebook cells sequentially.
4. Ensure an internet connection is available when the dataset-download cell runs.

The dataset is downloaded automatically from Cricsheet, so a separate local dataset file is not required.

##  Limitations

- This project focuses on exploratory data analysis and does not predict match outcomes.
- Batter comparisons include only players who faced at least 120 balls in the analyzed data.
- The analysis focuses on the first two innings and overs 1–20.
- Findings depend on the source data and the cleaning and classification methods used.

##  Data Source & Attribution

The cricket data is sourced from [Cricsheet](https://cricsheet.org/).

Please consult the [Cricsheet website](https://cricsheet.org/) for the applicable data licensing and attribution requirements.

This repository presents an analysis of the source data. The source dataset remains subject to its applicable licensing and attribution terms.

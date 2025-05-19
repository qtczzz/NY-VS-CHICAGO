
# ⚾ Monte Carlo Simulation of MLB Team Performance Using Real Stats

## 📌 Project Overview
This project simulates full 9-inning baseball games between the **Chicago White Sox** and **New York Yankees** using Monte Carlo methods, powered by **real player statistics** from MLB.com. Each player’s outcome probabilities are dynamically retrieved using the MLB API and used to simulate batting performance over thousands of games.

## 🎯 Objectives
- Use real MLB data to estimate scoring probabilities for each batter.
- Simulate thousands of games between the White Sox and Yankees.
- Visualize and analyze scoring distributions and run differentials.
- Estimate win probabilities and average scoring rates per inning.

## 🧩 Methodology
- **Data Retrieval**: Top 9 batters for each team are pulled from the MLB API.
- **Probability Calculation**: Each batter’s hitting stats (H, 2B, 3B, HR, BB, PA) are converted to:
  - `P(single)`, `P(double)`, `P(triple)`, `P(home_run)`, `P(walk)`, `P(out)`
- **Game Simulation**:
  - Full 9-inning games.
  - Batters rotate continuously through their team's lineup.
  - Repeat simulation 10,000 times.
- **Analysis**:
  - Track average runs per inning and game.
  - Plot histograms of scores and differentials.

## 📊 Key Output
- Run distributions per team over 10,000 games
- Run differential histogram (Team A - Team B)
- Calculation of:
  - `Average runs per inning` for each team
  - Win rate and tie rate
  - Standard deviation of scores

## 🗃️ Data Sources
Player data is pulled from:
- [Chicago White Sox Stats](https://www.mlb.com/whitesox/stats)
- [New York Yankees Stats](https://www.mlb.com/yankees/stats)

All stats are accessed via the official [MLB Stats API](https://statsapi.mlb.com).

## 🛠️ Technologies Used
- Python 3.11+
- `pandas`, `requests` – data handling & API
- `random`, `numpy` – Monte Carlo simulation
- `matplotlib` – plots and visualizations
- Jupyter Notebook – interactive development

## 📂 Project Structure

```
/project_folder
│
├── baseball_sim.ipynb           # Final simulation notebook
├── README.md                    # This file
└── mlb_batting_stats.csv (opt)  # Offline input version of batter stats
```

## 📌 Assumptions & Notes
- Only hitting stats are modeled; no pitching or defensive plays included.
- Probabilities are assumed constant (no fatigue or game context).
- Batting order is fixed and cyclic for simplicity.

## 🧠 Potential Extensions
- Add pitching stats or pitcher-vs-batter matchup logic.
- Incorporate team strategies (e.g., stealing, bunting).
- Expand simulation to cover playoff series or entire seasons.
- Include home-field effects.

## 📧 Contact
Created by [Your Name]  
MS in Data Science, Northwestern University  
Email: yourname@u.northwestern.edu

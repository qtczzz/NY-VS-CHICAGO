This is a status log for group 2 about a Baseball Simulator project.

## Team: Group 2

## Time: May 19

teration 1 (2025-05-18)

### Current Task: Search and Visualize Player Stats

Progress:

Implemented a Monte Carlo simulation of 9-inning baseball games between the Chicago White Sox and the New York Yankees.

Real batting stats retrieved from the official MLB Stats API and parsed into outcome probabilities:

P(single), P(double), P(triple), P(home_run), P(walk), P(out)

Simulated 10,000 games with rotating batting lineups for each team.

Visualization of:

Team score distributions

Run differentials (White Sox - Yankees)

Win, loss, and tie percentages



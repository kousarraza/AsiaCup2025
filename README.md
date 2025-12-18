# 🏏 Asia Cup 2025: Comprehensive T20 Dataset & Exploratory Analysis

<p align="center">
  <a href="https://doi.org/10.5281/zenodo.17228056"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.17228056.svg" alt="DOI"></a>
  <a href="https://arxiv.org/abs/2512.XXXX"><img src="https://img.shields.io/badge/arXiv-2512.XXXX-b31b1b.svg" alt="arXiv"></a>
  <a href="https://github.com/kousarraza/AsiaCup2025/blob/main/LICENSE"><img src="https://img.shields.io/badge/License-CC_BY_4.0-lightgrey.svg" alt="License"></a>
  <a href="https://kousarraza.github.io/AsiaCup2025/"><img src="https://img.shields.io/badge/GitHub%20Pages-Live-success.svg" alt="Live Demo"></a>
  <a href="https://github.com/kousarraza/AsiaCup2025/blob/main/notebooks/AsiaCup2025_EDA.ipynb"><img src="https://img.shields.io/badge/Jupyter-Notebook-orange.svg" alt="Notebook"></a>
</p>

<p align="center">
  <strong>A comprehensive dataset and exploratory analysis of the Asia Cup 2025 T20 cricket tournament featuring 19 matches with 61 variables per match.</strong>
</p>

<p align="center">
  <img src="images/19_team_performance_heatmap.png" alt="Team Performance Heatmap" width="800">
  <br>
  <em>Team Performance Heatmap - Comprehensive Comparison of All Teams</em>
</p>

---

## 📊 Live Demo
🔗 **Interactive Web Report:** [https://kousarraza.github.io/AsiaCup2025/](https://kousarraza.github.io/AsiaCup2025/)

---

## 🎯 Overview
This project provides a **comprehensive structured dataset** and **detailed exploratory analysis** of the **Asia Cup 2025 T20 cricket tournament**.  
The dataset covers all 19 matches with 61 carefully curated variables, enabling researchers, analysts, and enthusiasts to perform advanced cricket analytics.

**Key Highlights:**
- 📈 **Comprehensive Coverage:** All matches from group stage to final  
- 🔍 **Detailed Variables:** 61 features including player-level statistics  
- 📊 **Professional Analysis:** 22 visualizations covering all aspects  
- 🔬 **Research Ready:** Formatted for academic research and ML applications  
- 🌐 **Open Access:** Fully open dataset and code under permissive licenses

---

## 📋 Dataset Features

### Match Information
- Match number, series, date, time, venue
- Teams, toss winner, toss decision, match result
- Tournament stage (Group, Super Four, Final)
- Player of the match, match referee, umpires

### Team Performance Metrics
- **Batting:** Runs, wickets, overs, extras (byes, leg byes, wides, no balls)  
- **Bowling:** Wickets taken, economy rates  
- **Powerplay:** Runs scored in powerplay overs  
- **Boundaries:** Fours and sixes hit by each team  
- **Fall of Wickets:** Detailed dismissal sequence  

### Player Statistics
- Top scorer for each team (with runs scored)  
- Top wicket-taker for each team (with wickets taken)  
- Player of the match awards  
- Playing XI for both teams  

### Tournament Structure
- Group stage (Group A & B)  
- Super Four stage (A1 vs A2, B1 vs B2, etc.)  
- Final match analysis  

---

## 🔑 Key Findings

### 🏆 Tournament Highlights
- **Champions:** India defeated Pakistan in the final  
- **Most Successful Team:** India (6 wins, highest win %)  
- **Best Batting Team:** India (most runs, most sixes, highest score)  
- **Best Bowling Team:** Pakistan (most wickets taken)  

### 📊 Statistical Insights
1. **Winning Trends:**  
   - 63% matches won by teams batting second  
   - Average win margin: 32.7 runs / 5.2 wickets  
   - Toss winners won 53% of matches  

2. **Scoring Patterns:**  
   - Average team score: 141.8 runs  
   - Average boundaries per match: 26.4  
   - Powerplay contribution: 32.5% of total runs  

3. **Player Excellence:**  
   - **Kuldeep Yadav:** 3 Player of Match awards  
   - **Pathum Nissanka:** Highest individual score (107*)  
   - **Shaheen Afridi:** Most economical bowler (6.2 economy)  

### 📈 Interesting Trends
- **Boundary Hitting:** Increased by 22% in knockout stages  
- **Toss Strategy:** 68% of toss winners chose to bowl first  
- **Venue Impact:** Dubai matches had 15% higher scoring rates  
- **Close Contests:** 42% matches decided by less than 20 runs/3 wickets  

---

## 🖼️ Visualization Gallery

### Team Performance
<p align="center">
  <img src="images/1_wins_by_team.png" width="45%" alt="Wins by Team">
  <img src="images/3_wins_vs_losses.png" width="45%" alt="Wins vs Losses">
  <br>
  <em>Team performance analysis showing wins distribution</em>
</p>

### Batting Analysis
<p align="center">
  <img src="images/4_total_sixes_by_team.png" width="45%" alt="Sixes by Team">
  <img src="images/5_total_boundaries_by_team.png" width="45%" alt="Boundaries by Team">
  <br>
  <em>Boundary hitting analysis across teams</em>
</p>

### Bowling Analysis
<p align="center">
  <img src="images/7_wickets_by_team.png" width="45%" alt="Wickets by Team">
  <img src="images/8_top_player_of_match.png" width="45%" alt="Player of Match">
  <br>
  <em>Bowling performance and individual awards</em>
</p>

### Tournament Dynamics
<p align="center">
  <img src="images/11_win_type_distribution.png" width="45%" alt="Win Types">
  <img src="images/18_boundaries_trend.png" width="45%" alt="Boundaries Trend">
  <br>
  <em>Match outcome patterns and tournament progression</em>
</p>

**View all 22 visualizations in the [interactive web report](https://kousarraza.github.io/AsiaCup2025/)**

---

## 🚀 Quick Start

### Prerequisites
- Python 3.8 or higher
- Basic understanding of Python and data analysis

### Installation

```bash
# Clone the repository
git clone https://github.com/kousarraza/AsiaCup2025.git
cd AsiaCup2025

# Install required packages
pip install pandas numpy matplotlib seaborn jupyter

# Or install from requirements.txt
pip install -r requirements.txt

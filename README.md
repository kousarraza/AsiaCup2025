# Asia Cup 2025: A Structured T20 Match-Level Dataset and Exploratory Analysis
<p align="center"> <a href="https://kousarraza.github.io/AsiaCup2025"><img src="https://img.shields.io/badge/🌐-Project%20Page-blue" alt="Project Page"></a> <a href="https://arxiv.org/abs/2512.XXXX"><img src="https://img.shields.io/badge/📄-arXiv%3A2512.XXXX-b31b1b" alt="arXiv"></a> <a href="https://doi.org/10.5281/zenodo.17228056"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.17228056.svg" alt="DOI"></a> <a href="https://github.com/kousarraza/AsiaCup2025/blob/main/LICENSE"><img src="https://img.shields.io/badge/📜-License%3A%20CC%20BY%204.0%2FMIT-green" alt="License"></a> <a href="https://github.com/kousarraza/AsiaCup2025/stargazers"><img src="https://img.shields.io/github/stars/kousarraza/AsiaCup2025?style=social&logo=github" alt="GitHub Stars"></a> <a href="https://github.com/kousarraza/AsiaCup2025/network/members"><img src="https://img.shields.io/github/forks/kousarraza/AsiaCup2025?style=social&logo=github" alt="GitHub Forks"></a> <a href="https://github.com/kousarraza/AsiaCup2025/issues"><img src="https://img.shields.io/github/issues/kousarraza/AsiaCup2025" alt="GitHub Issues"></a> </p><p align="center"> <strong>A Complete Dataset and Analysis of the Asia Cup 2025 T20 Cricket Tournament</strong><br> <em>19 Matches • 61 Variables • 22 Visualizations • Open Source</em> </p><p align="center"> <a href="https://github.com/kousarraza">Kousar Raza</a><sup>1*</sup> · <a href="https://github.com/faizanali">Faizan Ali</a><sup>2*</sup> </p><p align="center"> <sup>1</sup>University of Isfahan, Iran · <sup>2</sup>University of Sindh, Jamshoro, Pakistan </p><p align="center"> <a href="https://kousarraza.github.io/AsiaCup2025">🌐 Live Interactive Report</a> · <a href="https://github.com/kousarraza/AsiaCup2025/archive/refs/heads/main.zip">📦 Download Dataset</a> · <a href="#citation">📝 Cite This Work</a> · <a href="#contact">📧 Contact</a> </p>


## Overview

This repository presents a comprehensive, structured dataset and detailed exploratory analysis of the Asia Cup 2025 T20 cricket tournament. The tournament featured 19 high-intensity matches between Asia's top cricket nations, providing rich data for sports analytics research.

**Directional Textual Inversion (DTI)** addresses this by:
- **Decoupling magnitude and direction**: Fixing embedding magnitude to an in-distribution scale
- **Spherical optimization**: Optimizing only the direction on the unit hypersphere via Riemannian SGD
- **vMF prior**: Using a von Mises-Fisher prior for semantic coherence


# 🏏 Asia Cup 2025: Comprehensive T20 Dataset & Exploratory Analysis

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.17228056.svg)](https://doi.org/10.5281/zenodo.17228056)
[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)
[![arXiv](https://img.shields.io/badge/arXiv-2512.XXXX-b31b1b.svg)](https://arxiv.org/abs/2512.XXXX)
[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Live-success.svg)](https://kousarraza.github.io/AsiaCup2025/)
[![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://github.com/kousarraza/AsiaCup2025/blob/main/notebooks/AsiaCup2025_EDA.ipynb)

**A comprehensive dataset and exploratory analysis of the Asia Cup 2025 T20 cricket tournament featuring 19 matches with 61 variables per match.**

<p align="center">
  <img src="images/19_team_performance_heatmap.png" alt="Team Performance Heatmap" width="800">
  <br>
  <em>Team Performance Heatmap - Comprehensive Comparison of All Teams</em>
</p>

## 📊 Live Demo

🔗 **Interactive Web Report:** [https://kousarraza.github.io/AsiaCup2025/](https://kousarraza.github.io/AsiaCup2025/)

## 📖 Table of Contents

- [Overview](#-overview)
- [Dataset Features](#-dataset-features)
- [Key Findings](#-key-findings)
- [Visualization Gallery](#-visualization-gallery)
- [Quick Start](#-quick-start)
- [Repository Structure](#-repository-structure)
- [Usage Examples](#-usage-examples)
- [Methodology](#-methodology)
- [Applications](#-applications)
- [Contributing](#-contributing)
- [Citation](#-citation)
- [License](#-license)
- [Contact](#-contact)
- [Acknowledgments](#-acknowledgments)

## 🎯 Overview

This project provides a **comprehensive structured dataset** and **detailed exploratory analysis** of the **Asia Cup 2025 T20 cricket tournament**. The dataset covers all 19 matches with 61 carefully curated variables, enabling researchers, analysts, and enthusiasts to perform advanced cricket analytics.

### Why This Project?

- **📈 Comprehensive Coverage:** All matches from group stage to final
- **🔍 Detailed Variables:** 61 features including player-level statistics
- **📊 Professional Analysis:** 22 different visualizations covering all aspects
- **🔬 Research Ready:** Formatted for academic research and ML applications
- **🌐 Open Access:** Fully open dataset and code under permissive licenses

## 📋 Dataset Features

### Match Information
- Match number, series, date, time, venue
- Teams, toss winner, toss decision, match result
- Tournament stage (Group, Super Four, Final)
- Player of the match, match referee, umpires

### Team Performance Metrics
- **Batting:** Total runs, wickets, overs, extras (byes, leg byes, wides, no balls)
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

## 🔑 Key Findings

### 🏆 Tournament Highlights
- **Champions:** India won the tournament defeating Pakistan in the final
- **Most Successful Team:** India (6 wins, highest win percentage)
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

DTI achieves superior text fidelity and subject preservation on **SDXL** and **SANA**.

<p align="center">
  <img src="docs/assets/teaser.png" alt="DTI Results" width="100%">
</p>

## Installation

**Requirements:** Python 3.9+ · PyTorch 2.0+ · CUDA GPU

```bash
git clone https://github.com/kunheek/dti
cd dti
pip install -e .
```

<details>
<summary>Using uv (recommended for faster setup)</summary>

```bash
uv venv python=3.12
source .venv/bin/activate
pip install -e .
```
</details>

## Quick Start

### Train DTI on SDXL

```bash
python exps/ours_sdxl.py -g 0
```

This runs DTI on all DreamBooth subjects. To train on a specific subject:

```bash
python exps/ours_sdxl.py -g 0 --instances dog
```

<details>
<summary>Full training command</summary>

```bash
accelerate launch --mixed_precision=bf16 --num_processes=1 \
  scripts/train_sdxl.py \
  --pretrained_model_name_or_path "stabilityai/stable-diffusion-xl-base-1.0" \
  --train_data_dir data/dreambooth/dog \
  --output_dir output/dti-sdxl/dog \
  --placeholder_token "<dog>" \
  --initializer_token dog \
  --resolution 768 \
  --train_batch_size 4 \
  --max_train_steps 400 \
  --learning_rate 0.01 \
  --token_scale mean \
  --kappa 1e-4 \
  --decompose_scale true
```
</details>

### Train on SANA

```bash
python exps/ours_sana.py -g 0 -m sana1.5_1.6b
```

### Evaluate

```bash
python scripts/evaluate.py -e output/dti-sdxl
```

## Training Options

| Parameter | Description | Default |
|-----------|-------------|---------|
| `-g` | GPU ID | `0` |
| `--instances` | Subject names | all |
| `--max_train_steps` | Training iterations | `400` |
| `--kappa` | vMF prior strength | `1e-4` |
| `--learning_rate` | Learning rate | `0.01` |
| `--token_scale` | Magnitude scale (`mean`, `max`, or float) | `mean` |

### Baselines

```bash
# Standard Textual Inversion
python exps/ti_sdxl.py -g 0

# DCO + DTI
python exps/ours_dco_sdxl.py -g 0
```

## Data Format

```
data/
├── dreambooth.json
└── dreambooth/
    └── subject_name/
        ├── 00.jpg
        ├── 01.jpg
        └── ...
```

JSON format:
```json
{
  "subject_name": {
    "path": "data/dreambooth/subject_name",
    "class": "dog",
    "initialization": "dog"
  }
}
```

Download DreamBooth dataset:
```bash
python scripts/download_datasets.py
```

## Project Structure

```
dti/
├── src/dti/       # Core implementation
├── scripts/       # Training & evaluation scripts
├── exps/          # Experiment launchers
└── data/          # Datasets and configs
```

## Citation

```bibtex
@article{kim2025directional,
  title={Directional Textual Inversion for Personalized Text-to-Image Generation},
  author={Kim, Kunhee and Park, NaHyeon and Hong, Kibeom and Shim, Hyunjung},
  journal={arXiv preprint arXiv:2512.13672},
  year={2025}
}
```

## License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.

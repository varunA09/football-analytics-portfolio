# ⚽ Euro 2024 Football Analytics — Shot Map, xG Analysis \& Pass Map

![Python](https://img.shields.io/badge/Python-3.10-blue?style=flat-square&logo=python)
![StatsBomb](https://img.shields.io/badge/Data-StatsBomb%20Open%20Data-red?style=flat-square)
![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)

A football analytics project built using **StatsBomb's free open data**, analysing team and player performance across the **UEFA Euro 2024** tournament. The project produces three professional-grade visualisations: a shot map, an xG leaderboard, and a progressive pass map.

> \*\*Data source:\*\* StatsBomb Open Data — \[statsbomb.com](https://statsbomb.com)  
> \*StatsBomb logo and branding used in accordance with their open data user agreement.\*

\---

## 📊 What This Project Covers

|Analysis|Description|
|-|-|
|**Shot Map**|Visualises every shot taken by a team across the tournament, sized by xG value and coloured by outcome|
|**xG Leaderboard**|Ranks the top 10 players by total Expected Goals (xG) accumulated and compares against actual goals scored|
|**Progressive Pass Map**|Maps all completed passes that progressed the ball from outside the final third into the final third|

\---

## 🧠 Key Concepts

### Expected Goals (xG)

Expected Goals (xG) is a probability metric assigned to every shot, ranging from 0 to 1. It estimates the likelihood of a shot resulting in a goal based on factors such as distance from goal, shot angle, body part used, and the type of assist. A shot with xG = 0.35 historically results in a goal 35% of the time.

xG is the most widely used metric in modern football analytics and underpins player evaluation, team performance assessment, and tactical reporting across professional clubs, broadcasters, and betting companies.

### Progressive Passes

A progressive pass is a completed pass that moves the ball significantly closer to the opponent's goal — in this project defined as a pass that starts outside the final third (x < 80 on the StatsBomb 120×80 pitch coordinate system) and ends inside it (x ≥ 80). These passes are a key indicator of a team's ability to break defensive lines and create attacking opportunities.

\---

## 🛠️ Tools \& Libraries

|Tool|Purpose|
|-|-|
|`Python 3.10`|Core programming language|
|`statsbombpy`|StatsBomb's official Python library for accessing free open data|
|`pandas`|Data manipulation and aggregation|
|`matplotlib`|Base charting and figure rendering|
|`mplsoccer`|Football pitch drawing and sports-specific visualisations|

\---

## 📁 Project Structure

```
football-analytics-portfolio/
│
├── euro2024\_analysis.ipynb     # Main Jupyter notebook with all analysis and charts
├── spain\_shot\_map.png          # Shot map visualisation
├── euro2024\_xg\_leaderboard.png # xG vs goals bar chart
├── spain\_progressive\_passes.png# Progressive pass map
└── README.md                   # This file
```

\---

## 🚀 How to Run This Project

### 1\. Clone the repository

```bash
git clone https://github.com/YOUR\_USERNAME/football-analytics-portfolio.git
cd football-analytics-portfolio
```

### 2\. Create a Python 3.10 environment

```bash
conda create -n football-analytics python=3.10
conda activate football-analytics
```

### 3\. Install dependencies

```bash
pip install "numpy<2" pandas statsbombpy mplsoccer matplotlib notebook
```

### 4\. Launch Jupyter Notebook

```bash
jupyter notebook
```

Open `euro2024\_analysis.ipynb`, ensure the kernel is set to `Python (football-analytics)`, and run all cells.

> \*\*Note:\*\* The `statsbombpy` library pulls data directly from StatsBomb's GitHub repository — no API key or account is required for open data access.

\---

## 📈 Key Findings

### Shot Map (Spain)

Spain's shot distribution across Euro 2024 revealed a strong concentration of high-xG chances in central positions close to goal, reflecting their possession-based, progressive style of play. The majority of low-xG shots originated from outside the box, while their goals came predominantly from high-probability central positions.

### xG Leaderboard

The comparison between accumulated xG and actual goals scored highlights both clinical finishers (players who outperformed their xG) and those who underperformed relative to the chances they created — a key distinction in player evaluation used by professional clubs.

### Progressive Pass Map (Spain)

Spain's progressive passing volume was among the highest in the tournament, with passes distributed across the width of the pitch into the final third — consistent with their high-press, positional play philosophy under their tactical system.

\---

## 📌 Data Attribution

This project uses **StatsBomb Open Data**, made freely available for public research and analysis.

* Repository: [github.com/statsbomb/open-data](https://github.com/statsbomb/open-data)
* Python library: [github.com/statsbomb/statsbombpy](https://github.com/statsbomb/statsbombpy)
* User Agreement: [statsbomb.com/resource-centre](https://www.statsbomb.com/resource-centre)

If you use or build upon this work, please also credit StatsBomb as the original data source.

\---

## 👤 About

**Varun Narayanan Kutty** — Data Analyst with an MSc in Big Data (University of Stirling) and experience in SQL, Python, Power BI, and Apache Spark. Currently building a sports analytics portfolio with a focus on football.

Connect on LinkedIn - https://www.linkedin.com/in/varunadiyodi/


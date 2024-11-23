# Position-Driven-Clustering-of-Basketball-Players
An interpretable clustering framework using Bayesian Networks to group basketball players by position based on performance metrics. Combines domain knowledge and Gaussian Mixture Models for insightful team analysis. Includes a user interface for real-time queries.
# Bayesian Network-driven Clustering of Basketball Players

A novel approach to clustering basketball players using Bayesian Networks and Gaussian Mixture Models, developed at Ahmedabad University's School of Engineering and Applied Science.

## 📊 Project Overview

This project introduces an interpretable, data-driven approach to clustering basketball players using Bayesian Networks. Unlike traditional "black box" clustering methods, our framework provides transparent insights into how player characteristics influence cluster assignments, making it particularly valuable for team strategy development and player analysis.

### Key Features

- *Interpretable Results*: Clear visualization of feature dependencies through Bayesian Networks
- *Position-based Clustering*: Specialized analysis for all five basketball positions (C, PF, SF, PG, SG)
- *Efficient Processing*: Handles high-dimensional data while maintaining computational efficiency
- *Domain Knowledge Integration*: Incorporates expert basketball knowledge in the clustering process
- *Real-time Query Interface*: User interface for immediate access to player analysis

## 🔍 Methodology

### Data Processing
- Dataset: NBA statistics from 2016-2024 seasons
- 30 features per player, averaged across seasons
- Categorical encoding using quartile divisions (0-3)

### Technical Implementation

1. *Bayesian Network Construction*
   - Hill Climbing Search algorithm with BIC scoring
   - Domain knowledge integration for edge fixation
   - Variable elimination for position inference

2. *Clustering Implementation*
   - Gaussian Mixture Model (GMM) for final clustering
   - Similarity matrix derived from Bayesian Network
   - 9 distinct player clusters

### Player Clusters

| Cluster Number | Type | Description |
|----------------|------|-------------|
| 1 | High Scorers | Excellent scoring ability, high shooting accuracy |
| 2 | Defensive Specialists | Strong defensive skills, excels in blocking and rebounding |
| 3 | 3-Point Shooters | Skilled at 3-point shooting, effective at long-range shots |
| 4 | Playmakers | Great passing skills, ability to assist and make plays |
| 5 | Rebounders | Strong rebound ability, good positioning |
| 6 | Efficient Shooters | High shooting efficiency, consistent scoring |
| 7 | Low Turnovers | Low turnover rate, maintains control under pressure |
| 8 | Aggressive Defenders | Aggressive in defense, high pressure on opponents |
| 9 | All-Rounders | Versatile skills in scoring, defense, and passing |

## 📈 Results

### Model Performance Comparison

| Model | Accuracy | F1 Score |
|-------|----------|-----------|
| SOM Clustering | 0.8653 | 0.8652 |
| KMeans Clustering | 0.8653 | 0.8652 |
| Bayesian Network Clustering | 0.827 | 0.823 |

### Position-Specific Key Features

- *Point Guard & Shooting Guard*: 
  - Free throws
  - Free throw attempts
  - 3 Pointers

- *Power Forward & Small Forward*: 
  - Blocks
  - 2 Pointers
  - 2 Pointer Attempts
  - Effective Field goals

- *Center*: 
  - Total rebounds
  - Blocks
  - 2 Pointers
  - 2 Pointer Attempts
  - Effective Field goals

## 🛠 Implementation

### Requirements
- Python 3.x
- Required libraries (requirements.txt to be provided)
- SQLite database for user interface

### Features
- Real-time player analysis
- Interactive user interface
- Position inference system
- Cluster analysis visualization
## 📚 References

1. Babaee Khobdeh, S., et al. (2021). Clustering of basketball players using self-organizing map neural networks.
2. D'Urso, P., et al. (2023). A Bayesian network to analyse basketball players' performances: A multivariate copula-based approach.
3. Liu, Z., et al. (2012). Empirical evaluation of scoring functions for Bayesian network model selection.

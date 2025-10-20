# Final Project
**Gayoung Kim**  
Final project for Python Programming II (90-819), Fall 2025

## Project Title
**Legislative Activity and Turnover in the U.S. House: Exploring Predecessor-Successor Patterns in Congressional Bills**

## Research Question
Do successors' legislative activities relate to their predecessors' patterns? Do these relationships differ when successors are from the same party (versus party flips) or when successors have existing family ties within Congress?

## Overview
The U.S. House of Representatives experiences regular turnover while maintaining a stable organizational structure (fixed seats and districts). This study explores whether predecessor behavior predicts successor behavior during the 117th→118th Congress (2021-2025).

## Repository Structure
```
.
├── 01-data-acquisition.qmd    # Download and parse raw data
├── 02-data-cleaning.qmd       # Create turnover pairs dataset
├── 03-eda.qmd                 # Exploratory visualizations
├── 04-analysis.qmd            # Regression models and tests
└── 05-summary.qmd             # Overview and key findings
├── data/
│   ├── raw/                       # Original data sources
│   ├── temp/                      # Intermediate files
└── └── processed/                 # Analysis-ready datasets
```

## Data Sources
1. **U.S. Congressional Bills** (117th-118th Congress): GovInfo API bulk data
2. **Bioguide Profiles**: Congressional biographical records and relationships
3. **Legislators List**: Historical roster from unitedstates/congress-legislators
4. **Legislative Effectiveness Scores**: Volden & Wiseman (CEL)

## Methods
- **Sample**: House turnover pairs from 117th→118th Congress transition
- **Variables**: Bills sponsored/cosponsored, party continuity, newcomer status, dynasty succession
- **Analysis**: Descriptive statistics, correlation analysis, OLS regression with controls


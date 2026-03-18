# AI & Labor Market: Automation vs Augmentation Analysis

[![Python](https://img.shields.io/badge/Python-3.10-blue)](https://python.org)
[![Dataset](https://img.shields.io/badge/Data-Anthropic%20Economic%20Index-orange)](https://huggingface.co/datasets/Anthropic/EconomicIndex)
[![License](https://img.shields.io/badge/License-MIT-green)](LICENSE)

## Overview
This project analyzes **666 occupations** from the Anthropic Economic Index 
to understand how AI automation risk relates to education level and salary.

**Key question:** Does higher education protect workers from AI automation?

## Key Findings
| Finding | Result |
|---------|--------|
| Salary vs automation correlation | r = −0.517 (moderate negative) |
| Salary gap (safe vs at-risk jobs) | +76% ($72K vs $41K/yr) |
| Most vulnerable sector | Office & Administrative Support (83.9% avg risk) |
| Safest sector | Community & Social Service (4.4% avg risk) |
| Education effect (Zone 1→5) | Risk drops from ~75% to ~15% |

## Visualizations

### Salary vs Automation Risk
<img width="1926" height="1176" alt="fig4_salary_vs_automation" src="https://github.com/user-attachments/assets/bebe02c3-c0a1-4122-be76-e2640c6e4836" />

### Education Level vs Automation Risk
<img width="2061" height="921" alt="fig8_jobzone_analysis" src="https://github.com/user-attachments/assets/cbb625f8-70dd-4bc4-bb4d-2b1c8d020e02" />

### Double Protection Effect
<img width="1472" height="1026" alt="fig10_double_protection" src="https://github.com/user-attachments/assets/66a239da-db0c-4e3d-b24a-6de6de6570e4" />

## Project Structure
```
ai-labor-market-analysis/
├── 01_data_exploration.ipynb        # EDA: distributions, missing values, top-risk jobs
├── 02_automation_analysis.ipynb     # Salary vs automation risk, sector bubble chart
├── 03_education_vs_automation.ipynb # JobZone analysis, "double protection" effect
├── images/                          # Visual assets: charts and plots 
├── wage_data.csv                    # Anthropic Economic Index dataset (Feb 2025)
└── README.md
```

## Tech Stack
- **Python** — Pandas, NumPy, Matplotlib, Seaborn
- **Environment** — Google Colab / Jupyter Notebook
- **Data source** — [Anthropic Economic Index](https://huggingface.co/datasets/Anthropic/EconomicIndex)
  (Hugging Face, February 2025 release, CC-BY license)

## How to Run
```bash
git clone https://github.com/DarynaAkkus/ai-labor-market-analysis
cd ai-labor-market-analysis
pip install -r requirements.txt
jupyter notebook
```
Or open directly in Google Colab:  
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/DarynaAkkus/ai-labor-market-analysis/blob/main/01_data_exploration.ipynb)

## Research Context
This analysis was developed as part of an academic conference paper:  
*"Sztuczna inteligencja a rynek pracy: automatyzacja czy augmentacja?"*  
2026

## Author
**Daryna Akkus**  

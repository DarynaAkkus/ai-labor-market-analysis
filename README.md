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
├── 📂 data/
│   ├── wage_data.csv                    # Occupation-level automation & salary data
│   ├── onet_task_mappings.csv           # Work tasks delegated to AI (O*NET)
│   ├── automation_vs_augmentation.csv   # AI interaction type breakdown
├── 📂 images/                           # All generated visualizations (14 charts)
├── 01_data_exploration.ipynb            # EDA: distributions, top-risk jobs
├── 02_automation_analysis.ipynb         # Salary vs automation risk
├── 03_education_vs_automation.ipynb     # Education "double protection" effect
├── 04_tasks_and_interactions.ipynb      # Task delegation + interaction patterns
├── .gitignore
├── requirements.txt
└── README.md
```


## Tech Stack
- **Python** — Pandas, NumPy, Matplotlib, Seaborn
- **Environment** — Google Colab / Jupyter Notebook
## Data Sources
| File | Description | Used in |
|------|-------------|---------|
| `wage_data.csv` | 873 occupations with salary & automation scores | Notebooks 1–3 |
| `onet_task_mappings.csv` | Work tasks mapped to AI usage frequency | Notebook 4 |
| `automation_vs_augmentation.csv` | AI interaction type distribution | Notebook 4 |


**Source:** [Anthropic Economic Index](https://huggingface.co/datasets/Anthropic/EconomicIndex), Hugging Face (Feb 2025, CC-BY license)

## How to Run
```bash
git clone https://github.com/DarynaAkkus/ai-labor-market-analysis
cd ai-labor-market-analysis
pip install -r requirements.txt
jupyter notebook
```

## Research Context
This analysis was developed as part of an academic conference paper:  
*"Sztuczna inteligencja a rynek pracy: automatyzacja czy augmentacja?"*  
2026

## Author
**Daryna Akkus**  

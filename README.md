# Early Warning System - OULAD

Predicts student risk (High/Medium/Low) within the first 28 days of a course
using the Open University Learning Analytics Dataset.

## Team
| Member | Roll No | Contribution |
|---|---|---|
| Akshara SR | 2024BCS0333 | Feature engineering, leakage controls |
| Akshaya S | 2024BEC0057 | Model training, evaluation, threshold tuning |
| Azra Hanan | 2024BCD0069 | Explainability and intervention rules |
| Benvin Vinu | 2024BCS0233 | Documentation, analyses, plots |

## Setup
1. Download OULAD dataset and extract CSVs into `data/` (see `data/README.md`)
2. Install dependencies: `pip install -r requirements.txt`
3. Open `notebooks/OULAD_Early_Warning_System.ipynb` and run all cells

## Results
- Random Forest chosen by 5-fold CV (macro-F1 0.551)
- Test accuracy 0.602, ROC-AUC 0.746
- High-Risk recall 87% with tuned threshold (0.26)

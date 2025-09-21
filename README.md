# SAT Score Trends (2018–2024)

This project analyzes SAT Suite of Assessments score distributions from 2018 through 2024 using publicly available College Board annual reports.

## Project Overview
The goal is to extract, clean, and analyze SAT score distribution data over multiple years to identify trends in overall performance and differences between the Evidence-Based Reading & Writing (ERW) and Math sections for male and female test takers.

## Data
- Source: [College Board Annual Reports](https://reports.collegeboard.org/sat-suite-program-results/data-archive)
- Format: PDF tables (pages 5–7, depending on report)
- Years: 2018–2024

## Methodology
1. **Data Extraction**  
   - Used `camelot` to parse tables from PDF reports.
2. **Data Cleaning**  
   - Standardized column names.
   - Added "Year" and "Section" fields.
   - Removed extraneous rows and restructured score ranges.
3. **Analysis**  
   - Compared score distributions across years.
   - Visualized ERW vs Math performance.
   - Tracked overall score trends.


## Repository Structure
```
├── data/              # Raw PDFs or download instructions
├── notebooks/         # Jupyter notebook(s)
│   └── SAT_Trends.ipynb
├── results/           # Cleaned CSVs or exported plots
└── README.md
```

## Requirements
- Python 3.9+
- `pandas`, `matplotlib`, `seaborn`, `camelot`

Install dependencies:
```bash
pip install pandas matplotlib seaborn camelot-py[cv]
```

## How to Run
1. Download the SAT reports and place them in `data/`.
2. Open the notebook in Jupyter.
3. Run all cells to reproduce the analysis.

## Author
Makenna Roberts
Master’s Student in Applied Statistics & Data Science  

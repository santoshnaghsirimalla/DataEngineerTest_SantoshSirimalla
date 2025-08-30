# Data Engineer Test – Supermarket Analytics and Reinforcement Learning

## Overview
This repository contains the submission for the **Data Engineer Test**. The project demonstrates supermarket analytics with supervised machine learning and a reinforcement learning experiment.

The work is divided into two tasks:

- **Task 01: Supervised Learning on Supermarket Data**  
  Data cleaning, feature engineering, exploratory analysis, and three machine learning models addressing:  
  1. Basket revenue forecasting (regression)  
  2. Predicting whether a customer will return within 30 days (classification)  
  3. Identifying high-performing supermarkets (classification)  

- **Task 02: Reinforcement Learning Maze Agent**  
  A Q-learning agent that learns to navigate a 10×10 maze using epsilon-greedy exploration and optimal policy convergence.

All results are included in executed Jupyter notebooks and summarized in the final report.

---

## Repository Structure
```
.
├── README.md                                # Instructions for review and reproduction
├── Santosh_DataEngineerTest_Report.pdf      # Final report (methodology, results, recommendations)
├── Santosh_BRD_Supermarkettest_Task1.ipynb  # Task 01: Supermarket analytics (supervised ML)
├── Santosh_DataEngineerTest_RL_Task2.ipynb  # Task 02: Reinforcement learning maze
└── data/
    └── .gitkeep                             # Placeholder; datasets are not included
```

---

## Instructions for Review (No Setup Required)
- Open **`Santosh_DataEngineerTest_Report.pdf`** for the complete documentation.  
- Open the executed notebooks (`.ipynb`) directly on GitHub to view code, outputs, and results.  
- No cloning or setup is required for reviewing.  

---

## Instructions for Running (Optional Reproduction)

### 1. Clone the repository
```bash
git clone https://github.com/santoshnaghsirimalla/DataEngineerTest_SantoshSirimalla.git
cd DataEngineerTest_SantoshSirimalla
```

### 2. Python environment
Use **Python 3.8 or above**. Install dependencies:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

### 3. Data placement
The following CSV files are required for Task 01:
- `items.csv`  
- `sales.csv`  
- `promotion.csv`  
- `supermarkets.csv`  

These datasets are not included in the repository due to size constraints.  

To run the notebooks:  
1. Place the four CSV files inside the existing `/data/` folder.  
2. Ensure the filenames match exactly.  

The notebooks are already configured to load from this folder:
```python
base_path = "data/"
sales = pd.read_csv(base_path + "sales.csv")
promotion = pd.read_csv(base_path + "promotion.csv")
items = pd.read_csv(base_path + "items.csv")
supermarkets = pd.read_csv(base_path + "supermarkets.csv")
```

### 4. Run notebooks
```bash
jupyter notebook
```



---

## Deliverables
- **Final Report:** `Santosh_DataEngineerTest_Report.pdf` – documentation of methodology, results, and recommendations.  
- **Task 01 Notebook:** `Santosh_BRD_Supermarkettest_Task1.ipynb` – supervised ML models on supermarket data (basket revenue, customer returns, high-performing stores).  
- **Task 02 Notebook:** `Santosh_DataEngineerTest_RL_Task2.ipynb` – reinforcement learning maze experiment.  
- **Repository:** Organized and reproducible, with clear guidance for both reviewers and users.  


---

## Notes
- Reviewers can read the report and executed notebooks directly on GitHub without any setup.  
- Cloning the repository and adding data in `/data` is required only for re-execution.  
- The `/data` folder is already included with a `.gitkeep` file to preserve structure.  

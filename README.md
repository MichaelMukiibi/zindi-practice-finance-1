# 1. Project Overview

This project aims to predict loan defaults for the Africa Credit Challenge using a classification approach. The solution is built using open-source Python libraries and follows a standard machine learning pipeline from data loading to submission generation.

# 2. Folder Structure & Data Setup

To run this solution, ensure your directory is organized as follows:

```Plaintext
.
├── data/
│   ├── Train.csv                # Training data with targets
│   ├── Test.csv                 # Test data for predictions
│   ├── economic_indicators.csv   # Supplementary external data
│   └── SampleSubmission.csv     # Reference for submission format
├── notebooks/
│   └── Starter_Notebook_.ipynb  # Primary execution notebook
├── requirements.txt             # Environment dependencies
└── README.md                    # README
```

# 3. Environment & Dependencies
The solution requires a Python 3.10+ environment.

- **Required Libraries:** ```pandas```, ```numpy```, ```matplotlib```, ```seaborn```, ```scikit-learn```.
- **Setup:** You can recreate the environment using the provided ```requirements.txt```

```bash
pip install -r requirements.txt
```

# 4. Hardware Requirements

The code was developed and tested on the following specifications:

- **Machine**: HP ProBook 440 G10
- **Processor**: 13th Gen Intel Core i7
- **RAM**: 16 GB
- **OS**: Arch Linux

# 5. Execution Order

To reproduce the results, run the notebook in the following sequence:

1. **Starter_Notebook_.ipynb**: Execute all cells from top to bottom. This handles data loading, basic preprocessing, model training (Logistic Regression), and generation of the final ```submission.csv```.

**Expected Run Time:** Approximately X-Y minutes on the specified hardware. (TBD)

# 6. Feature Explanations

The following key features are used from the dataset:

- **Total_Amount:** The total loan amount initially disbursed.
- **Total_Amount_to_Repay:** Total amount expected including interest and fees.
- **duration:** Length of the loan term in days.
- **New_versus_Repeat:** Categorical indicator of customer loan history.
- **Lender_portion_Funded:** Percentage of the loan funded by the lender.

# 7. Reproducibility Note

A fixed ```random_state=42``` (or similar) is used in all stochastic processes (e.g., ```train_test_split``` and model initialization) to ensure the leaderboard score remains consistent across runs.




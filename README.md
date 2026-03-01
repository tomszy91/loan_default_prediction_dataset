# loan_default_prediction

[![Python](https://img.shields.io/badge/Python-3.12-blue.svg)](https://www.python.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

Analysis of a dataset containing 255,347 unique loan records. The project focuses on exploratory data analysis (EDA) of data with a high degree of balance in categorical features and on identifying patterns leading to default status, which affects 11.6% of the population in the dataset.

## Research Questions

* **What percentage of loan applications end in default? How does this vary between marital status, education, and employment type?**
* **What is the average loan amount? How does it differ between self-employed vs. employed vs. unemployed?**
* **Do people with higher incomes get higher loans?**
* **Profile of a typical "defaulted" vs. "non-defaulted" borrower. What distinguishes them?**
* **Which combination of characteristics (income + loan amount + credit score + DTI) poses the highest risk of default?**

## Key Insights

* **Scale and class balance**: The dataset includes 255,347 borrowers, of whom 29,712 (11.6%) have defaulted on their loans.
* **Categorical homogeneity**: All major categorical features, such as education (Bachelor's, High School, Master's, PhD) and employment type, are distributed almost perfectly evenly, each with approximately 63,000 records.
* **Age structure**: The data covers individuals aged 18 to 69, and the distribution for each specific age is flat, with approximately 4,800 to 5,000 observations per year.
* **Financial goals**: Loans are divided into five equal categories (Auto, Business, Education, Home, Medical), each of which includes approximately 51,000 applications.
* **Key financial metrics**: The average income in the dataset is $82,491, with an average loan amount of $127,578 and an average DTI ratio of 0.25.

## Technical Stack

* **Python 3.12+**
* **pandas** – Data manipulation and cleaning
* **numpy** – Numerical computing
* **matplotlib** – Data visualization
* **seaborn** – Advanced statistical graphics
* **openpyxl** – Excel file integration
* **jupyter** – Analytical environment

## Project Structure

```bash
online_retail_dataset/
├── data/
│   └── Loan_default.csv
├── loan_default_prediction.ipynb
├── requirements.txt
├── README.md
└── LICENSE
```

## Usage

1. Clone the repository:

    ```bash
    git clone https://github.com/tomszy91/loan_default_prediction_dataset.git
    cd loan_default_prediction_dataset
    ```

2. Install the required dependencies:

    ```bash
    pip install -r requirements.txt
    ```

3. Launch the analysis:

    ```bash
    jupyter notebook loan_default_prediction.ipynb
    ```

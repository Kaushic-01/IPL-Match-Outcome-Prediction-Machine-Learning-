# 🏏 IPL Player Performance Prediction using Machine Learning

## 📝 Overview

This repository contains a Machine Learning project focused on analyzing and predicting the performance of **both batsmen and bowlers** in the Indian Premier League (IPL).

The core of the project is a Jupyter Notebook (`Machine Learning Project on IPl DataSet.ipynb`) that leverages historical IPL data to train predictive models. The primary goal is to forecast key **batting and bowling** metrics, offering a data-driven approach to player analysis and potential match-up strategy.

-----

## ✨ Key Features

  * **Data Preprocessing:** Cleaning and transforming raw IPL match data into a structured format suitable for machine learning.
  * **Predictive Modeling:** Utilizing advanced ML algorithms, including **Linear Regression** and **Random Forest Regressor** (in addition to **XGBoost**) for robust prediction.
  * **Batting Metric Prediction:** Forecasting crucial performance indicators:
      * Total **Runs** scored.
      * **Balls** faced, **Fours**, and **Sixes** hit (in the precision forecasting model).
  * **Bowler Metric Prediction:** Forecasting crucial performance indicators:
      * Total **Wickets** taken.
      * **Economy Rate** (Runs conceded per over).
      * Total **Overs** bowled in a match/period.
  * **Tiered Analysis:** Displaying predicted performance with a tiered structure for easy comparison and strategic grouping.

-----

## 🛠️ Technologies & Libraries

The project is built using Python and requires the following key libraries:

  * **Python 3.x**
  * **Jupyter Notebook** (or JupyterLab)
  * `pandas`
  * `numpy`
  * `scikit-learn`
  * `xgboost`
  * `matplotlib` / `seaborn` (for visualization, if included)

-----

## 🚀 Getting Started

Follow these steps to set up and run the project locally.

### Prerequisites

You should have Python and `pip` installed on your system.

### 1\. Clone the Repository

```bash
git clone <your-repository-url>
cd <your-repository-name>
```

### 2\. Install Dependencies

It is recommended to use a virtual environment.

```bash
# Create a virtual environment
python -m venv venv
source venv/bin/activate  # On Windows, use: venv\Scripts\activate

# Install required packages
pip install pandas numpy scikit-learn xgboost jupyter
```

### 3\. Dataset

The project requires the historical IPL dataset.

  * **Source:** *[Placeholder: Provide a link to the dataset you used, e.g., Kaggle or a specific source.]*
  * **File Naming:** Ensure your raw data files are placed in a designated folder (e.g., `data/`) and named according to how they are referenced in the notebook (`IPL match/Ball by Ball 1.csv` and `IPL match/IPL matches 1.csv`).

### 4\. Run the Analysis

Launch the Jupyter Notebook environment and open the project file.

```bash
jupyter notebook
```

Open the `Machine Learning Project on IPl DataSet.ipynb` file and execute the cells sequentially to perform the data loading, model training, and prediction analysis.

-----

## 📊 Example Output (Snippet)

The final output provides clear, predicted scorecards for both batsman and bowler performance.

**Predicted Total Runs for Batters (Example: Type 1 Model - Linear Regression):**

```
Predicted Total Runs for Active Batters in the Next Season:
         batter predicted_runs_next_season
        V Kohli 570
     RD Gaikwad 458
        R Parag 451
      TM Head 447
     SV Samson 421
...
```

*(The prediction for V Kohli's total runs in the next season is 570 runs).*

**Bowler Tiered Analysis (Example: Type 2 Model - Random Forest Regressor):**

```
--- Tier: Elite Predictors ---
(Expected Performance: 3.5 Wickets, 5.80 Econ, 4.0 overs)

         bowler  predicted_wickets  predicted_runs_conceded  predicted_economy_rate  predicted_overs_bowled
      J Bumrah                4.0                     22.0                    5.50                     4.0
      R Khan                  3.0                     23.2                    5.80                     4.0
...
```

*(The output displays tiered performance predictions, including Wickets, Economy Rate, Runs Conceded, and Overs Bowled).*

-----

## 🤝 Contribution

Feel free to open issues or submit pull requests to enhance the prediction model or improve the analysis.

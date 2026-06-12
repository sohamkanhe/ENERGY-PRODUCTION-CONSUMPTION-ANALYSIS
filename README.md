# Energy Production & Consumption Analysis

This project provides a comprehensive analysis of renewable energy production sites in the United States, focusing on Hydro, Solar, and Wind energy. It explores geographic distributions, capacity trends, and developable areas, employing advanced decision-making algorithms and machine learning models to rank and classify energy sites.

The analysis is implemented in both **Python** and **R**, allowing for a comparative look at the data through different programming ecosystems.

## Project Overview

The analysis is contained in two primary notebooks:
*   **Python**: `Energy_Production_Consumption_Analysis.ipynb`
*   **R**: `Energy_Production_Consumption_Analysis.Rmd`

The project performs the following key tasks:

1.  **Data Preprocessing**: Cleaning and integrating disparate datasets for hydro, solar, and wind energy.
2.  **Exploratory Data Analysis (EDA)**: Visualizing site locations across the US, analyzing capacity distributions, and identifying correlations between developable area and energy output.
3.  **Data Balancing**: Utilizing upsampling techniques (in Python) to handle class imbalances for more robust modeling.
4.  **Site Ranking (MCDM)**: Implementing Multi-Criteria Decision Making (MCDM) algorithms to rank the potential and efficiency of different sites:
    *   **TOPSIS** (Technique for Order of Preference by Similarity to Ideal Solution)
    *   **MOORA** (Multi-Objective Optimization on the basis of Ratio Analysis)
5.  **Classification Modeling**: Training and evaluating machine learning models to classify energy sources based on site characteristics:
    *   Logistic Regression, Decision Trees, Random Forest, SVM, KNN, and LSTM.
6.  **Time Series Forecasting**: Predicting future energy consumption using ARIMA models.

## Dataset Description

The analysis uses several datasets located in the `data/` directory:

*   `US_Geo_Hydro.csv`: Data on hydroelectric sites.
*   `US_Solar.csv`: Data on solar energy sites and developable areas.
*   `US_Wind.csv`: Information on wind energy production sites.
*   `US_Prod_and_Cons.xlsx`: Broader statistics on energy production and consumption trends.

## Installation & Setup

### Python Environment
To run the Python analysis locally:
1.  **Install dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

### R Environment
To run the R analysis locally:
1.  **Install R and RStudio**.
2.  **Install required packages**:
    Open R/RStudio and run:
    ```R
    install.packages(c("tidyverse", "readxl", "caret", "randomForest", "e1071", "forecast", "xgboost", "corrplot"))
    ```

## Usage

### Running the Python Notebook
1.  Launch Jupyter Notebook:
    ```bash
    jupyter notebook
    ```
2.  Open `Energy_Production_Consumption_Analysis.ipynb` and run the cells.

### Running the R Notebook
1.  Open `Energy_Production_Consumption_Analysis.Rmd` in RStudio.
2.  Click "Knit" or run the individual code chunks.

## Technologies Used

*   **Languages**: Python, R
*   **Python Stack**: Pandas, NumPy, Scikit-learn, TensorFlow, Matplotlib, Seaborn
*   **R Stack**: tidyverse (ggplot2, dplyr), caret, randomForest, forecast, readxl
*   **Models**: TOPSIS, MOORA, Random Forest, ARIMA, LSTM, XGBoost

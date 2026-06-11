# Energy Production & Consumption Analysis

This project provides a comprehensive analysis of renewable energy production sites in the United States, focusing on Hydro, Solar, and Wind energy. It explores geographic distributions, capacity trends, and developable areas, employing advanced decision-making algorithms and machine learning models to rank and classify energy sites.

## Project Overview

The core of this analysis is contained in the Jupyter Notebook `Energy_Production_Consumption_Analysis.ipynb`. The project performs the following key tasks:

1.  **Data Preprocessing**: Cleaning and integrating disparate datasets for hydro, solar, and wind energy.
2.  **Exploratory Data Analysis (EDA)**: Visualizing site locations across the US, analyzing capacity distributions, and identifying correlations between developable area and energy output.
3.  **Data Balancing**: Utilizing upsampling techniques to handle class imbalances for more robust modeling.
4.  **Site Ranking (MCDM)**: Implementing Multi-Criteria Decision Making (MCDM) algorithms to rank the potential and efficiency of different sites:
    *   **TOPSIS** (Technique for Order of Preference by Similarity to Ideal Solution)
    *   **MOORA** (Multi-Objective Optimization on the basis of Ratio Analysis)
    *   **Hybrid AHP-TOPSIS** and **AHP-MOORA** (Integrating Analytic Hierarchy Process for weight derivation).
5.  **Classification Modeling**: Training and evaluating multiple machine learning models to classify energy sources based on site characteristics (latitude, longitude, area, elevation, etc.):
    *   Logistic Regression
    *   Decision Tree Classifier
    *   Random Forest Classifier
    *   Support Vector Machine (SVM)
    *   K-Nearest Neighbors (KNN)
    *   Long Short-Term Memory (LSTM) Neural Networks

## Dataset Description

The analysis uses several datasets located in the `data/` directory:

*   `US_Geo_Hydro.csv`: Data on hydroelectric sites, including geographic coordinates and capacity.
*   `US_Solar.csv`: Extensive data on solar energy sites and developable areas.
*   `US_Wind.csv`: Detailed information on wind energy production sites.
*   `US_Prod_and_Cons.xlsx`: Broader statistics on energy production and consumption.

## Installation

To run the analysis locally, ensure you have Python installed. It is recommended to use a virtual environment.

1.  **Clone the repository**:
    ```bash
    git clone https://github.com/sohamkanhe/ENERGY-PRODUCTION-CONSUMPTION-ANALYSIS.git
    cd energy-production-consumption-analysis
    ```

2.  **Install dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

## Usage

1.  Launch Jupyter Notebook or JupyterLab:
    ```bash
    jupyter notebook
    ```
2.  Open `Energy_Production_Consumption_Analysis.ipynb`.
3.  Run the cells sequentially to reproduce the analysis, visualizations, and model evaluations.

## Key Findings

*   **Geographic Concentration**: Hydro energy sites are more geographically concentrated near water bodies, while solar and wind sites show a broader distribution across the US.
*   **Capacity Correlations**: A strong linear relationship exists between coverage area and capacity for solar sites, which is less pronounced for hydro and wind.
*   **Model Performance**: Classification models, particularly Random Forest and Decision Trees, achieved high accuracy in predicting energy types based on geographic and physical site attributes.

## Technologies Used

*   **Languages**: Python
*   **Data Analysis**: Pandas, NumPy, SciPy
*   **Visualization**: Matplotlib, Seaborn, Plotly
*   **Machine Learning**: Scikit-learn, XGBoost, TensorFlow/Keras
*   **Decision Making**: Custom implementations of AHP, TOPSIS, and MOORA.

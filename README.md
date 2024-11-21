# Air Quality in Europe: A Data-Driven Analysis of Energy and Pollution Trends

This project is a comprehensive data science investigation into the relationship between energy consumption patterns, socioeconomic factors, and air quality across European countries. Using advanced data analysis techniques and machine learning models, this project provides actionable insights to aid environmental policy formulation and public health initiatives.

## Project Overview

With Europe's ambitious climate goals and varied energy consumption behaviors, understanding the interplay between energy sources, air quality, and public health is critical. This project examines how renewable energy usage, GDP, population, and geographical factors influence air quality. Additionally, predictive models are developed to forecast PM10 air pollution levels.

## Objectives

- **Data Analysis:** Identify trends and correlations between energy sources and air quality.
- **Feature Engineering:** Derive meaningful variables from raw data.
- **Machine Learning:** Predict PM10 air pollution levels using Random Forest and other algorithms.
- **Insights for Policy:** Provide data-driven recommendations for sustainable energy policies.

## Project Workflow

1. **Data Collection**
   - Web scraping using Selenium and MechanicalSoup.
   - API calls to OpenWeatherMap for weather data.
   - Data sourced from reputable platforms such as EEA and Wikipedia.

2. **Data Preprocessing**
   - Cleaning datasets with Python (Pandas, NumPy).
   - Handling missing values and anomalies.
   - Transforming raw data into analysis-ready formats.

3. **Exploratory Data Analysis (EDA)**
   - Visualizing trends in air pollution and renewable energy usage.
   - Correlation analysis between variables like GDP, population, and pollutant levels.

4. **Feature Engineering**
   - Creating derived variables to enhance predictive modeling.
   - Normalizing and aligning datasets for compatibility.

5. **Modeling**
   - Training a Random Forest regression model for PM10 prediction.
   - Cross-validation to assess model robustness.
   - Hyperparameter tuning for optimization.

6. **Evaluation and Insights**
   - Model performance measured by R² and MSE.
   - Insights into feature importance (e.g., O₃ and NO₂ levels).

## Key Files and Structure

### Jupyter Notebooks
- **`1.scraping_airquality_data.ipynb`**  
  Scrapes air quality metrics like PM10, NO₂, and O₃ from EEA.
- **`1.scraping_renewable_energy_data.ipynb`**  
  Gathers renewable energy consumption data.
- **`2.airquality_data_impurity_simulation.ipynb`**  
  Simulates and handles data imperfections for robustness testing.
- **`2.cleaning_renewable_energy_data.ipynb`**  
  Cleans renewable energy data.
- **`3.cleaning_airquality_data.ipynb`**  
  Processes air quality data for analysis.
- **`4.merged_data.ipynb`**  
  Combines datasets and performs EDA.
- **`Mariadb_studentA.ipynb`**  
  Loads cleaned data into MariaDB for centralized storage.

### Documentation
- **`Report_Group16_Hazime-Zayour_Batschelet_Devdas.docx`**  
  Detailed report covering project motivation, methods, and findings.

## Technologies Used

- **Programming:** Python
- **Libraries:** Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn
- **Machine Learning:** Random Forest
- **Database:** MariaDB
- **Web Scraping:** Selenium, MechanicalSoup
- **Cloud Tools:** OneDrive, GitHub

## Results

### Modeling Performance
- **Best Model:** Random Forest
  - R²: 0.91
  - Mean Squared Error (MSE): 1.54
- **Feature Importance:**
  - Top predictors: O₃ levels, NO₂ levels, GDP, renewable energy usage.

### Key Insights
- Strong correlation between renewable energy consumption and reduced air pollutants.
- Economic growth (GDP) influences air quality but varies by country and energy mix.
- Weather factors (temperature, wind speed) play a secondary role in air pollution levels.


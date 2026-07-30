# IBM Data Science Capstone: SpaceX Falcon 9 First Stage Landing Prediction

## Project Overview

This project was completed as the capstone for the IBM Data Science Professional Certificate. The objective is to predict whether the **SpaceX Falcon 9 first stage will successfully land** using historical launch data. Since successful landings allow SpaceX to reuse rocket boosters, accurately predicting landing outcomes can provide insights into launch costs and mission success.

The project follows the complete data science workflow, including data collection, data wrangling, exploratory data analysis, interactive visualizations, and machine learning.

---

## Business Problem

SpaceX has significantly reduced launch costs through reusable rocket technology. A successful Falcon 9 first-stage landing enables booster reuse, making launches more cost-effective.

The goal of this project is to develop a machine learning model capable of predicting whether the first stage will successfully land based on characteristics of previous launches.

---

## Project Workflow

### 1. Data Collection

Data was collected from multiple sources:

* SpaceX REST API
* Wikipedia Falcon 9 launch records (web scraping)

Collected information includes:

* Flight number
* Launch date
* Booster version
* Payload mass
* Orbit type
* Launch site
* Landing outcome
* Core reuse information
* Geographic coordinates

---

### 2. Data Wrangling

The collected data was cleaned and transformed before analysis.

Key preprocessing steps included:

* Removing launches with multiple boosters (Falcon Heavy)
* Removing launches with multiple payloads
* Handling missing values
* Converting dates into a standardized format
* Extracting relevant information from nested API responses
* Creating a structured Pandas DataFrame

---

### 3. Exploratory Data Analysis (EDA)

Exploratory analysis was performed using SQL queries and Python visualizations to identify relationships between launch characteristics and landing success.

Variables explored include:

* Flight number
* Payload mass
* Orbit type
* Launch site
* Launch success rate
* Year of launch

Visualizations were created using:

* Matplotlib
* Plotly Express

---

### 4. Interactive Visual Analytics

Interactive dashboards were created to better understand launch trends.

Tools used:

* Plotly Dash
* Folium

These dashboards allow users to explore:

* Launch success by site
* Payload mass distributions
* Launch locations
* Interactive maps of launch sites

---

### 5. Machine Learning

Several classification algorithms were trained to predict Falcon 9 landing success.

Models evaluated:

* Logistic Regression
* Support Vector Machine (SVM)
* Decision Tree Classifier
* K-Nearest Neighbors (KNN)

Model performance was optimized using GridSearchCV with cross-validation.

---

## Results

The analysis found that several launch characteristics influence landing success, including:

* Launch site
* Payload mass
* Orbit type
* Flight history

The machine learning models achieved approximately **83% prediction accuracy**, demonstrating that historical launch data contains meaningful predictive information.

---

## Technologies Used

* Python
* Pandas
* NumPy
* Requests
* BeautifulSoup
* SQL
* Matplotlib
* Plotly
* Dash
* Folium
* Scikit-learn
* Jupyter Notebook

---

## Repository Structure

```text
IBM-Data-Science-Cert/
│
├── Data Collection API Lab
├── Web Scraping Lab
├── Data Wrangling
├── Exploratory Data Analysis (SQL)
├── Exploratory Data Visualization
├── Interactive Visual Analytics (Folium)
├── Plotly Dash Dashboard
├── Machine Learning Prediction
├── Presentation.pdf
└── README.md
```

---

## How to Run

1. Clone this repository.
2. Install the required Python libraries.
3. Open the Jupyter notebooks.
4. Run the notebooks sequentially from data collection through machine learning.
5. Launch the Plotly Dash application to explore the interactive dashboard.

---

## Author

**Kymani B.**

Completed as part of the **IBM Data Science Professional Certificate**.


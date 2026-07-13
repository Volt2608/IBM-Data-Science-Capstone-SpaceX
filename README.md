# 🚀 SpaceX Falcon 9 First Stage Landing Prediction

> **IBM Data Science Professional Certificate – Applied Data Science Capstone Project**

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-ML-yellow?logo=scikit-learn)
![Plotly](https://img.shields.io/badge/Plotly-Dashboard-blueviolet)
![Folium](https://img.shields.io/badge/Folium-Interactive%20Maps-green)

---

# 📖 Table of Contents

- [Project Overview](#project-overview)
- [Business Problem](#business-problem)
- [Project Objectives](#project-objectives)
- [Project Workflow](#project-workflow)
- [Repository Structure](#repository-structure)
- [Project Methodology](#project-methodology)
- [Technologies Used](#technologies-used)
- [Machine Learning Models](#machine-learning-models)
- [Results](#results)
- [Key Findings](#key-findings)
- [Installation](#installation)
- [Future Improvements](#future-improvements)
- [References](#references)
- [Author](#author)
- [Acknowledgements](#acknowledgements)

---

# 📌 Project Overview

SpaceX has transformed the commercial space industry by developing reusable rockets. The ability to recover and reuse the Falcon 9 first-stage booster significantly reduces launch costs and improves operational efficiency.

This project analyzes historical Falcon 9 launch data to identify the factors influencing first-stage landing success and develops machine learning models capable of predicting landing outcomes.

The project follows the complete data science lifecycle, including data collection, data preparation, exploratory analysis, interactive visualization, and predictive modeling.

---

# 🎯 Business Problem

The cost of launching a Falcon 9 rocket is substantially lower than many competing launch providers because the first-stage booster can be recovered and reused.

Predicting whether a Falcon 9 first stage will successfully land enables more accurate launch cost estimation and supports data-driven decision-making for future missions.

---

# 🎯 Project Objectives

The objectives of this project are to:

- Collect Falcon 9 launch data from multiple sources.
- Prepare and clean the collected datasets.
- Perform exploratory data analysis using SQL and Python visualizations.
- Build interactive maps and dashboards for launch analysis.
- Train multiple machine learning classification models.
- Compare model performance and identify the best-performing classifier.

---

# 🔄 Project Workflow

```text
SpaceX API
      │
      ▼
Wikipedia Web Scraping
      │
      ▼
Data Wrangling
      │
      ▼
Exploratory Data Analysis
      │
      ├──────── SQL Analysis
      │
      └──────── Python Visualizations
      │
      ▼
Interactive Folium Maps
      │
      ▼
Plotly Dash Dashboard
      │
      ▼
Predictive Analysis
      │
      ▼
Model Evaluation
      │
      ▼
Best Classification Model
```

---

# 📂 Repository Structure

```text
IBM-Data-Science-Capstone-SpaceX/

│
├── notebooks/
│   ├── Data Collection API.ipynb
│   ├── Web Scraping.ipynb
│   ├── Data Wrangling.ipynb
│   ├── EDA with SQL.ipynb
│   ├── EDA with Visualization.ipynb
│   ├── Folium Interactive Map.ipynb
│   ├── Plotly Dashboard.ipynb
│   └── Predictive Analysis.ipynb
│
├── dashboard/
│   └── spacex_dash_app.py
│
├── data/
│   ├── dataset_part_1.csv
│   ├── dataset_part_2.csv
│   ├── dataset_part_3.csv
│   ├── spacex_launch_dash.csv
│   └── spacex_web_scraped.csv
│
├── presentation/
│   ├── Data Science Capstone Project Report.pdf
│   └── Data Science Capstone Project Report.pptx
│
│
├── README.md
```

*(Update the folder names if they differ in your repository.)*

---

# ⚙️ Project Methodology

## 1️⃣ Data Collection

Launch data was collected from two different sources:

### SpaceX REST API

- Retrieved Falcon 9 launch records.
- Extracted booster version, payload, launch site and core information.
- Converted the retrieved data into a structured dataset.

### Web Scraping

Launch history was extracted from Wikipedia using:

- Requests
- BeautifulSoup

The extracted launch records were converted into a Pandas DataFrame for further analysis.

---

## 2️⃣ Data Wrangling

The collected datasets were cleaned and prepared for analysis.

Tasks included:

- Handling missing values
- Exploring mission features
- Examining launch sites
- Creating the binary Landing Class target variable
- Exporting the processed dataset

---

## 3️⃣ Exploratory Data Analysis

EDA was performed using SQL queries and Python visualizations.

### SQL Analysis

SQL queries were used to:

- Retrieve unique launch sites
- Calculate payload statistics
- Analyze mission outcomes
- Identify booster versions
- Explore landing outcomes
- Summarize Falcon 9 mission performance

### Data Visualization

Python visualizations included:

- Flight Number vs Launch Site
- Payload Mass vs Launch Site
- Success Rate vs Orbit Type
- Flight Number vs Orbit Type
- Payload Mass vs Orbit Type
- Launch Success Yearly Trend

---

## 4️⃣ Interactive Visual Analytics

### Folium Maps

Interactive maps were developed to visualize:

- Launch site locations
- Launch outcomes
- Geographic proximity to coastlines
- Nearby highways
- Railways
- Cities

### Plotly Dash Dashboard

The interactive dashboard enables users to:

- Select launch sites
- Filter payload ranges
- View launch success distribution
- Explore payload vs landing success
- Compare booster performance interactively

---

## 5️⃣ Predictive Analysis

Four supervised machine learning models were developed:

- Logistic Regression
- Support Vector Machine (SVM)
- Decision Tree
- K-Nearest Neighbors (KNN)

All models were optimized using **GridSearchCV** before evaluation.

---

# 🛠 Technologies Used

## Programming Language

- Python

## Data Processing

- Pandas
- NumPy

## Data Visualization

- Matplotlib
- Plotly

## Interactive Analytics

- Plotly Dash
- Folium

## Web Scraping

- Requests
- BeautifulSoup

## Machine Learning

- Scikit-learn
- GridSearchCV

## Database

- SQLite

## Development Environment

- Jupyter Notebook
- IBM Skills Network Labs
- Visual Studio Code

---

# 🤖 Machine Learning Models

| Model | Accuracy |
|----------------------|---------:|
| Decision Tree | **88.89%** |
| Logistic Regression | **83.33%** |
| Support Vector Machine | **61.11%** |
| K-Nearest Neighbors | **50.00%** |

The **Decision Tree classifier** achieved the highest classification accuracy and was selected as the final predictive model.

---

# 📊 Results

The project successfully demonstrated the complete end-to-end data science workflow.

Major outcomes include:

- Successful collection of Falcon 9 launch data from multiple sources.
- Development of cleaned datasets suitable for analysis.
- Interactive SQL analysis and visual analytics.
- Creation of interactive Folium maps and Plotly Dash dashboards.
- Training and evaluation of multiple classification models.
- Selection of the Decision Tree classifier as the best-performing predictive model.

---

# 🔍 Key Findings

- Launch Site influences first-stage landing success.
- Payload Mass is associated with landing outcomes.
- Orbit Type affects landing performance.
- Falcon 9 landing success improved steadily over time.
- Interactive analytics provided additional insights into launch performance.
- Decision Tree produced the highest predictive accuracy among the evaluated models.

---

## ⚙️ Installation & Set Up

Clone the repository:

```bash
git clone https://github.com/Volt2608/IBM-Data-Science-Capstone-SpaceX.git
```

Navigate to the project directory:

```bash
cd IBM-Data-Science-Capstone-SpaceX
```

Install the required Python libraries:

```bash
pip install pandas numpy matplotlib plotly dash folium requests beautifulsoup4 scikit-learn jupyter ipython-sql sqlalchemy
```

Alternatively, install each package individually:

```text
pandas>=2.0.0
numpy>=1.24.0
matplotlib>=3.7.0
plotly>=5.15.0
dash>=2.14.0
folium>=0.14.0
requests>=2.31.0
beautifulsoup4>=4.12.0
scikit-learn>=1.3.0
jupyter>=1.0.0
ipython-sql>=0.5.0
sqlalchemy>=2.0.0
```

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Run the notebooks sequentially from **Data Collection** through **Predictive Analysis**.

---

# 🚀 Future Improvements

Possible future enhancements include:

- Training additional ensemble models such as Random Forest and XGBoost.
- Incorporating real-time launch data from the SpaceX API.
- Deploying the prediction model as a web application.
- Improving dashboard functionality with additional filtering options.
- Exploring deep learning approaches for landing prediction.

---

# 📚 References

- IBM Data Science Professional Certificate
- SpaceX REST API
- Wikipedia – Falcon 9 Launch History
- Scikit-learn Documentation
- Plotly Documentation
- Folium Documentation
- BeautifulSoup Documentation

---

# 👩‍💻 Author

**Jyotika Bhatia**

IBM Data Science Professional Certificate

GitHub: https://github.com/Volt2608


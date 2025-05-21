# 🚀 IBM Data Science Capstone Project – SpaceX Launch Analysis

---

## 📌 Overview

This capstone project is the final requirement of the IBM Data Science Professional Certificate. It focuses on analyzing SpaceX launch data to extract business insights and build predictive models to determine the success of rocket launches.

The project includes:

* Data collection via SpaceX API and web scraping
* Data wrangling and transformation
* Exploratory Data Analysis (EDA) using Python and SQL
* Interactive geospatial visualization with Folium
* Interactive dashboard development using Plotly Dash
* Machine learning classification models to predict launch outcomes

---

## 🎯 Objective

* Identify the key factors influencing SpaceX launch success
* Build and evaluate classification models to predict mission success
* Develop interactive visual tools for stakeholders to explore data insights

---

## 🛠️ Tools & Technologies

* **Python:** Pandas, NumPy, Scikit-learn, BeautifulSoup, Requests
* **SQL:** For structured querying and EDA
* **Dash & Plotly:** Interactive dashboards
* **Folium:** Geospatial mapping
* **Jupyter Notebook:** Development environment
* **IBM Skills Network Labs:** Hosting and deployment

---

## 📂 Project Structure

```
├── notebooks/
│   └── Capstone-Project.ipynb       # Main notebook
├── assets/
│   └── visualizations/              # Maps, charts, dashboards
├── spacex_launch_dash.csv          # Cleaned dataset
├── README.md                        # Project documentation
```

---

## 🔍 Methodology

### 🧾 Data Collection

* Fetched SpaceX launch data via their REST API (`/launches`, `/rockets`, `/missions`)
* Parsed JSON data into Pandas DataFrames
* Conducted additional scraping using BeautifulSoup to enhance the dataset

### 🧹 Data Wrangling

* Handled missing values and duplicates
* Renamed columns, formatted types (e.g., datetime), and normalized fields
* Performed feature engineering for model improvement

### 📊 Exploratory Data Analysis (EDA)

* Used SQL queries and visualizations (histograms, box plots, heatmaps)
* Analyzed success rates across orbit types, payload weights, and sites
* Identified trends over time and across mission types

### 🌍 Interactive Visual Analytics

* **Folium Map:** Visualized launch sites, payload mass, and outcomes
* **Plotly Dash App:** Included:

  * Pie charts (success/failure)
  * Scatter plots (payload vs. success)
  * Filters (site selector, payload slider)

### 🤖 Predictive Modeling

* Models used:

  * Logistic Regression
  * Decision Tree
  * Support Vector Machine (SVM – best performer with RBF kernel)
  * K-Nearest Neighbors
* Evaluation metrics:

  * Accuracy, Precision, Recall, F1-score
* Hyperparameter tuning using `GridSearchCV` with 10-fold cross-validation

---

## 📈 Results

* **Best Model:** SVM with RBF kernel achieved highest accuracy
* **Top Influencing Factors:**

  * Launch site
  * Payload mass
  * Orbit type
* **Insights:**

  * Launch sites like CCAFS SLC-40 and KSC LC-39A showed higher success rates
  * Heavier payloads tend to succeed more at experienced launch sites
  * Success rates improved steadily year over year

---

## 📊 Interactive Components

* **Folium Map:**

  * Geolocated launch sites with outcome markers
  * Payload trajectory and infrastructure proximity
* **Plotly Dash Dashboard:**

  * Filter by site and payload
  * Pie chart (Success distribution)
  * Scatter plots and sliders for in-depth analysis

---

## 🧪 Evaluation Metrics

| Metric    | Value |
| --------- | ----- |
| Accuracy  | 83.3% |
| Precision | 0.80  |
| Recall    | 1.00  |
| F1-Score  | 0.89  |

Confusion Matrix showed excellent recall and high precision with only 3 false positives.

---

## 📚 Appendix

**Dataset:** `spacex_launch_dash.csv`
**Key Features:**

* Launch Site
* Payload Mass (kg)
* Booster Version Category
* Class (0 = Fail, 1 = Success)

**Python Libraries Used:**

* `pandas`, `numpy`, `plotly`, `dash`, `sklearn`, `folium`, `requests`, `beautifulsoup4`

---
## 📄 Final Report (PDF)
You can view the full capstone report here:  
[📥 Download/View PDF Report](https://drive.google.com/file/d/19FmUwLZZlRdsJuNS5-cOYnYJYBWLJwM9/view?usp=drive_link)

# 🧠 COVID-19 Data Analysis & World Happiness Correlation

![Python](https://img.shields.io/badge/Python-3.11-blue?logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-1.6.2-blue?logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-1.26.1-orange?logo=numpy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3.8.1-red?logo=matplotlib&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-0.13.3-blueviolet?logo=seaborn&logoColor=white)

This project analyzes the global spread of COVID-19 and explores its relationship with socio-economic indicators from the **World Happiness Report**.  
The goal is to uncover patterns in infection rates across countries and determine whether happiness-related factors (like GDP, health, and social support) had any impact on pandemic outcomes.

---

## 📌 Project Overview

During the COVID-19 pandemic, countries showed varied infection patterns due to differences in healthcare systems, preparedness, and socio-economic conditions.  
This project performs a **data-driven analysis** to understand these variations and correlate them with global happiness indicators.

---

## 🎯 Objectives

- Analyze the progression and spread of COVID-19 globally.
- Compute and compare **maximum infection rates** across countries.
- Merge and correlate COVID-19 data with **World Happiness Report metrics**.
- Visualize key relationships to identify patterns or anomalies.

---

## 🧰 Tech Stack

**Languages & Tools:**  
- Python  
- Jupyter Notebook  

**Libraries:**  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  

---

## 🧩 Datasets Used

1. **COVID-19 Confirmed Cases Dataset**  
   - Contains date-wise cumulative confirmed cases for each country.  
   - Preprocessing: Removed unnecessary columns like `Lat` and `Long`.

2. **World Happiness Report**  
   - Contains indicators like GDP per capita, Health expectancy, Freedom, and Social Support.  
   - Preprocessing: Removed redundant columns such as `Generosity`, `Corruption`, and `Score`.

---

## ⚙️ Approach

### 1. Data Cleaning & Preparation
- Loaded both datasets and handled missing or irrelevant columns.  
- Aggregated COVID-19 data by **country** for easier analysis.  
- Calculated **daily new cases** using `.diff()`.  
- Extracted the **maximum infection rate** for each country.

### 2. Data Integration
- Renamed inconsistent columns for alignment.  
- Merged both datasets on the *Country* field to enable correlation analysis.

### 3. Exploratory Data Analysis (EDA)
- Plotted cumulative cases and infection trends for major countries like **India, China, Spain, Brazil, and the U.S.**  
- Visualized daily infection spikes using Matplotlib.  
- Created comparative plots to observe differences in spread patterns.

### 4. Correlation Analysis
- Used Seaborn regression plots and heatmaps to explore relationships between:  
  - GDP per Capita vs Max Infection Rate  
  - Health Expectancy vs Max Infection Rate  
  - Social Support vs Max Infection Rate  

- Observation: Happiness or economic indicators didn’t strongly correlate with infection rates.

---

## 📊 Key Insights

- China’s infection rate curve flattened earlier than most countries.  
- The U.S. and Spain recorded the highest peak infection rates.  
- Higher GDP or happiness scores **did not guarantee** lower infection rates.  
- Non-economic factors like healthcare readiness, early lockdowns, and public awareness played crucial roles.

---

## 🧠 Conclusion

This analysis demonstrates how **data integration from multiple domains** (health + socio-economic) can provide valuable perspectives.  
While the World Happiness metrics showed little direct correlation with infection rates, they revealed broader insights into societal resilience during crises.

---

## 🧩 Skills Demonstrated

- Data Cleaning & Transformation  
- Exploratory Data Analysis (EDA)  
- Statistical Correlation  
- Data Visualization & Storytelling  
- Python-based Analytical Workflow

---

## 📈 Visual Outputs (Examples)

- Line plots of cumulative COVID-19 cases by country  
- Daily infection rate trends  
- Scatter plots and regression lines showing happiness vs infection metrics  
- Heatmaps for variable correlation

---

## 📜 Author

**👨‍💻 Chinmay Shukla**  
B.Tech Student | Data Analyst | Web & UI/UX Designer  
📍 Passionate about transforming data into meaningful insights  

---

## 🔗 Repository Structure

COVID19-Happiness-Analysis/
│
├── data/
│ ├── covid19_confirmed.csv
│ └── world_happiness.csv
│
├── notebooks/
│ └── covid_happiness_analysis.ipynb
│
├── outputs/
│ └── plots/
│
├── README.md
└── requirements.txt

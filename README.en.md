🇬🇧 English | readme en français 👉 [🇫🇷 Français](README.md) 
# 📊 Education Systems Data Analysis

Project carried out as part of the **Data Engineer training – OpenClassrooms**.

The objective of this project is to analyze global education data in order to identify countries with the highest potential for expanding an academy internationally.

---

# 🎯 Project Objective

Identify the most promising countries for establishing an academy by analyzing:

* economic indicators  
* educational indicators  
* demographic data  

A **weighted scoring method** was developed to rank countries based on their potential.

---

# 🧹 Data Cleaning

Several data preparation steps were carried out:

* loading and exploring datasets  
* removing columns with more than **90% missing values**  
* checking and removing duplicates  
* computing descriptive statistics  
* selecting the **15 years with the fewest missing values**  
* selecting the **15 most relevant indicators**  

Countries with too many missing values were also removed to ensure a usable dataset.

---

# 📊 Indicator Analysis

Each selected indicator was analyzed individually:

* statistical analysis using `describe()`  
* distribution visualization  
* interpretation of results  

This step helped better understand relationships between variables and identify the most relevant indicators for the analysis.

---

# 🔎 Removing Redundant Indicators

A correlation analysis was performed to identify highly correlated indicators.

When two indicators had a correlation above **0.9**, one of them was removed to avoid redundancy and simplify the analysis model.

Some gender-based indicators (male / female) were also removed due to high correlation with overall indicators.

---

# 🧠 Scoring Method

A scoring algorithm called **Academy Score** was developed to rank countries.

Each country receives a score based on several indicators:

| Indicator                     | Weight |
| ----------------------------- | ------ |
| GDP per capita                | 8      |
| Number of students            | 3      |
| Total GDP                     | 3      |
| Total population              | 1      |

This score provides an **objective ranking of countries with the highest market potential**.

---

# 📈 Results

The analysis allows comparison of countries across several dimensions:

* economic wealth  
* size of the education market  
* economic stability  
* population size  

The final score highlights countries with the **highest potential for international expansion**.

---

# ⚠️ Limitations

* data aggregated at the national level  
* absence of qualitative factors (regulation, competition, culture)  
* some data may be outdated  

This project therefore represents **an initial exploratory analysis** to identify potential markets.

---

# 🛠️ Technologies Used

* Python  
* Pandas  
* NumPy  
* Matplotlib  
* Seaborn  
* Scikit-learn  
* Jupyter Notebook  

Project dependencies are defined in the `pyproject.toml` file.

---

# 📂 Repository Content

education_data_analysis.ipynb → full data analysis  
project_presentation.pptx → project presentation  
pyproject.toml → reproducible environment  

---

# 👨‍💻 Author

YAD95  
OpenClassrooms Project – Education Systems Data Analysis

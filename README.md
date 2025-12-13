# Machine-Learning-Driven Business Success

**Author:** Rizwan Ahasan Pathan  
**Affiliation:** M.S. in Applied Data Science, University of Southern California (USC)  
**Project Type:** End-to-End Data Engineering & Machine Learning Project  
**Geographic Scope:** Los Angeles City (119 ZIP Codes)  
**Primary Focus:** Applied Machine Learning, Data Engineering, Decision Analytics


---

## Overview

This project demonstrates an **end-to-end machine learning–driven analytics pipeline** designed to examine how data and technology influence business success in a real-world context. Using the **restaurant industry** as a practical case study, the system integrates heterogeneous data sources, engineers meaningful features, and applies statistical analysis and machine learning models to uncover actionable insights.

Rather than relying on a single signal (such as online ratings), the project combines **regulatory quality indicators**, **customer engagement metrics**, and **neighborhood-level contextual data** to build a more comprehensive, data-driven view of performance and opportunity. The outcome is a **reproducible, production-style pipeline** that illustrates how machine learning and data engineering can effectively support informed business decision-making.


---

## Project Objectives

- Integrate multiple real-world data sources into a unified analytical model  
- Analyze relationships between operational quality signals and customer behavior  
- Engineer composite performance and opportunity metrics  
- Identify high-potential geographic regions using clustering and ranking methods  
- Predict business success using supervised machine learning models  
- Translate model outputs into interpretable, decision-oriented insights  


---

## Data Sources

### 1. Regulatory Inspection Data (Scraped)
- **Source:** Los Angeles County Department of Public Health  
- **Collection Method:** Selenium + BeautifulSoup  
- **Records:** 8,441  
- **Key Features:** Inspection score, grade, inspection date, address, ZIP code  

### 2. Business Metadata (API)
- **Source:** Yelp Fusion API  
- **Records:** 20,917 businesses  
- **Key Features:** Rating, review count, price level, categories, location, business status  

### 3. Demographic & Economic Indicators (Scraped + API)
- **Sources:** UnitedStatesZipCodes.org, U.S. Census API  
- **Coverage:** 182 ZIP codes (119 within Los Angeles City)  
- **Key Features:** Population, population density, median income, employment rate, median home value  

### 4. Geographic Reference Table
- **Purpose:** ZIP-level normalization, city filtering, and relational consistency across datasets  
 

---


## Technical Architecture

- **Programming Language:** Python 3.9+  
- **Database:** SQLite (normalized relational schema with foreign keys)  
- **Data Collection:** Selenium, BeautifulSoup, REST APIs  
- **Data Processing & Modeling:** Pandas, NumPy, scikit-learn  

### Machine Learning Techniques
- Feature engineering and normalization  
- Clustering using K-Means  
- Classification using Random Forest  
- Feature importance analysis  

### Visualization
- Matplotlib  
- Seaborn  

### Execution Environment
- Jupyter Notebook  

A unified SQL view, **`Combined_Restaurant_View`**, serves as the single source of truth for all downstream analytics and machine learning workflows.


---


## Machine Learning & Analytics Components

- **Composite Success Index** to quantify overall business performance  
- **Opportunity Scoring Model** to rank and compare geographic regions  
- **Correlation and clustering analysis** to uncover underlying structural patterns  
- **Supervised learning model** to predict high-performing businesses  
- **Model explainability** through feature importance and visual diagnostics  

Together, these components demonstrate how machine learning models can be operationalized to provide practical, real-world analytical decision support.

---

## Requirements

- Python 3.9 or later  
- All project dependencies are defined in `requirements.txt`

### Installation
bash
pip install -r requirements.txt

---

## Installation

```bash
pip install -r requirements.txt

---

## Reproducibility & Extensibility

- Modular scripts enable independent execution of each stage of the data pipeline  
- Relational database design supports straightforward schema extension  
- Analytical workflows can be adapted to domains beyond the restaurant industry  
- Machine learning models are designed to be interpretable and reproducible  

---

## References

- [Python Documentation](https://docs.python.org/3/)
- [scikit-learn Documentation](https://scikit-learn.org/stable/)
- [Pandas Documentation](https://pandas.pydata.org/docs/)
- [SQLite Documentation](https://sqlite.org/docs.html)
- [SQLite Query Planner](https://sqlite.org/queryplanner.html)
- [U.S. Census API](https://www.census.gov/data/developers/data-sets.html)
- [Yelp Fusion API](https://www.yelp.com/developers/documentation/v3)
- [Selenium Documentation](https://www.selenium.dev/documentation/)
- [BeautifulSoup Documentation](https://www.crummy.com/software/BeautifulSoup/bs4/doc/)
- [Matplotlib Documentation](https://matplotlib.org/stable/)
- [Seaborn Documentation](https://seaborn.pydata.org/)

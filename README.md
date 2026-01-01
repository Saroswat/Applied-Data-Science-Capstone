# SpaceX Falcon 9 First-Stage Landing Prediction  
### *IBM Data Science Capstone Project*



##  **Project Overview**

This project investigates whether the **successful landing of SpaceX Falcon 9 first stages** can be predicted using **publicly available data and machine learning techniques**.

First-stage reusability is a critical factor in reducing launch costs. By predicting landing success, this project demonstrates how **data-driven decision-making** can support **mission planning and cost estimation** in the aerospace industry.

The project follows a **complete end-to-end data science lifecycle**, from raw data collection to predictive modeling and interactive visualization.



##  **Objectives**

- Collect SpaceX launch data from multiple public sources  
- Clean, preprocess, and engineer meaningful features  
- Perform exploratory and statistical analysis using Python and SQL  
- Build interactive visual analytics for deeper insight discovery  
- Train and evaluate machine learning models to predict landing success  

---

🗂️ Project Structure

The repository is organized to reflect each stage of the data science pipeline, from data collection to deployment and presentation.

📁 notebooks/
	•	01_data_collection_api.ipynb
Data collection using the SpaceX REST API
	•	02_web_scraping.ipynb
Web scraping Falcon 9 launch data from Wikipedia
	•	03_data_wrangling.ipynb
Data cleaning, preprocessing, and feature engineering
	•	04_eda_visualization.ipynb
Exploratory Data Analysis using Matplotlib and Seaborn
	•	05_eda_sql.ipynb
Exploratory Data Analysis using SQL queries
	•	06_interactive_map_folium.ipynb
Geospatial analysis and proximity visualization using Folium
	•	07_machine_learning_prediction.ipynb
Predictive modeling, hyperparameter tuning, and evaluation

⸻

📁 dashboard/
	•	spacex_dash_app.py
Interactive dashboard built using Plotly Dash

⸻

📁 data/
	•	spacex_launch_data.csv
SpaceX launch data collected from the REST API
	•	spacex_web_scraped.csv
Launch data collected via web scraping
	•	dataset_part_3.csv
Final processed dataset used for machine learning

⸻

📁 presentation/
	•	SpaceX_Capstone_Presentation.pdf
Final project presentation submitted for peer review

⸻

📄 README.md
	•	Project documentation and overview

⸻

✅ Notes
	•	Each notebook corresponds to a specific stage of the project
	•	The structure supports reproducibility and peer evaluation
	•	Dash application and presentation files are separated for clarity

│   └── SpaceX_Capstone_Presentation.pdf
│
└── README.md





---

## 📊 **Data Sources**

### 🔹 SpaceX REST API
- Launch details
- Payload information
- Booster and landing outcomes

### 🔹 Wikipedia (Web Scraping)
- Falcon 9 launch history tables
- Parsed using **BeautifulSoup**

---

## 🧪 **Methodology**

### **1️⃣ Data Collection**
- Retrieved structured data using the **SpaceX REST API**
- Scraped additional launch records from **Wikipedia**
- Converted JSON and HTML tables into Pandas DataFrames

---

### **2️⃣ Data Wrangling & Preprocessing**
Performed using **Pandas** and **NumPy**:
- Removed irrelevant and redundant columns  
- Handled missing values (e.g., payload mass imputation)  
- Identified numerical vs categorical variables  
- Applied **One-Hot Encoding**  
- Normalized and standardized numerical features  

---

### **3️⃣ Exploratory Data Analysis (EDA)**
- Visual analysis using **Matplotlib** and **Seaborn**
- Aggregations and filtering using **SQL**
- Identified key factors influencing landing success

---

### **4️⃣ Interactive Visual Analytics**
- **Folium** for geospatial analysis of launch sites and proximities  
- **Plotly Dash** for an interactive dashboard with dropdowns and sliders  

---

### **5️⃣ Predictive Analysis**
- Train-test split applied to the dataset  
- Models trained and tuned using **GridSearchCV**:
  - Logistic Regression  
  - Support Vector Machine (SVM)  
  - Decision Tree  
  - K-Nearest Neighbors (KNN)  

---

## 🤖 **Machine Learning Results**

| Model | Accuracy |
|------|---------|
| Logistic Regression | **0.8333** |
| Support Vector Machine | **0.8333** |
| **Decision Tree** | **⭐ 0.8889 (Best)** |
| K-Nearest Neighbors | **0.8333** |

✅ **Best Performing Model:** **Decision Tree Classifier**  
- Highest accuracy  
- Interpretable decision logic  
- Suitable for operational deployment  

---

## 🗺️ **Key Insights**

- **Launch site, payload mass, orbit type, and launch maturity** are the strongest predictors of landing success  
- Landing success rates have **improved significantly over time**  
- Coastal launch sites with strong transport infrastructure are strategically chosen  
- Machine learning models can reliably approximate landing outcomes  

---

## 📈 **Dashboards & Visualizations**

- Interactive **Plotly Dash** dashboard for dynamic analysis  
- **Folium maps** for spatial reasoning and proximity analysis  
- Enables real-time exploration of:
  - Launch sites  
  - Payload ranges  
  - Landing outcomes  

---

## 🧾 **Final Deliverables**

- ✔ Completed Jupyter notebooks  
- ✔ Interactive dashboard application  
- ✔ Final presentation (PDF)  
- ✔ Fully reproducible GitHub repository  

---

## 🔮 **Future Work**

- Incorporate environmental and weather data  
- Apply ensemble models (Random Forest, Gradient Boosting)  
- Introduce time-aware or sequential models  
- Add explainability techniques (e.g., SHAP values)  

---

## 👤 **Author**

**Saroswat Roy**  
*MSc Artificial Intelligence (NLP)*  
📍 London, United Kingdom  

---

## 📜 **License**

This project is created for **educational purposes** as part of the  
**IBM Data Science Capstone**.

---

⭐ *If you found this project insightful, feel free to explore the notebooks or fork the repository.*

# 🚗 Fuel Consumption & CO₂ Emissions — Exploratory Data Analysis

## 📊 Project Overview

This project presents an **Exploratory Data Analysis (EDA)** of vehicle fuel consumption and CO₂ emissions using **Python**.

The analysis focuses on understanding relationships between **vehicle specifications, fuel consumption, fuel types, fuel efficiency, and CO₂ emissions**. Various data analysis and visualization techniques are used to identify patterns, distributions, and relationships within the dataset.

The project was developed using **Pandas, NumPy, Matplotlib, and Seaborn** in a Jupyter Notebook environment.

---

## 🎯 Objectives

The main objectives of this project are:

* Understand the structure and characteristics of the vehicle dataset.
* Perform initial data inspection and data-quality checks.
* Analyze different vehicle manufacturers and models.
* Examine the distribution of fuel types.
* Study engine size and number of cylinders.
* Analyze city, highway, and combined fuel consumption.
* Investigate fuel efficiency using combined MPG.
* Explore CO₂ emission patterns.
* Identify relationships between vehicle specifications, fuel consumption, and CO₂ emissions.
* Visualize important patterns using statistical graphs and charts.

---

## 📁 Dataset

The dataset contains information about vehicles, their technical specifications, fuel consumption, and CO₂ emissions.

### Dataset Size

* **Rows:** 1,067
* **Columns:** 13
* **Model Year:** 2014

### Dataset Features

| Column                     | Description                      |
| -------------------------- | -------------------------------- |
| `MODELYEAR`                | Vehicle model year               |
| `MAKE`                     | Vehicle manufacturer             |
| `MODEL`                    | Vehicle model                    |
| `VEHICLECLASS`             | Vehicle category/class           |
| `ENGINESIZE`               | Engine size                      |
| `CYLINDERS`                | Number of engine cylinders       |
| `TRANSMISSION`             | Transmission type                |
| `FUELTYPE`                 | Fuel type                        |
| `FUELCONSUMPTION_CITY`     | Fuel consumption in city driving |
| `FUELCONSUMPTION_HWY`      | Fuel consumption on highways     |
| `FUELCONSUMPTION_COMB`     | Combined fuel consumption        |
| `FUELCONSUMPTION_COMB_MPG` | Combined fuel efficiency in MPG  |
| `CO2EMISSIONS`             | CO₂ emissions                    |

The notebook confirms that all 13 columns contain 1,067 non-null records.

---

## 🛠️ Technologies & Libraries

The following technologies were used:

* 🐍 **Python**
* 🧮 **NumPy**
* 🐼 **Pandas**
* 📈 **Matplotlib**
* 📊 **Seaborn**
* 📓 **Jupyter Notebook**

---

## 🔍 EDA Process

### 1. Data Loading

The dataset was loaded into a Pandas DataFrame for analysis.

### 2. Data Understanding

The dataset structure was examined using:

* `head()`
* `tail()`
* `shape`
* `columns`
* `info()`
* `describe()`

The dataset contains both **numerical and categorical variables**.

### 3. Data Quality Checking

Missing-value analysis was performed across all columns.

**Result:** No missing values were found in the dataset.

Duplicate records were also checked.

**Result:** `0` duplicate rows were identified.

---

## 📊 Statistical Analysis

The numerical analysis provides the following key values:

| Metric               |   Mean | Minimum | Maximum |
| -------------------- | -----: | ------: | ------: |
| Engine Size          |   3.35 |     1.0 |     8.4 |
| Cylinders            |   5.79 |       3 |      12 |
| City Consumption     |  13.30 |     4.6 |    30.2 |
| Highway Consumption  |   9.47 |     4.9 |    20.5 |
| Combined Consumption |  11.58 |     4.7 |    25.8 |
| Combined MPG         |  26.44 |      11 |      60 |
| CO₂ Emissions        | 256.23 |     108 |     488 |

These statistics show considerable variation in engine specifications, fuel consumption, fuel efficiency, and CO₂ emissions across the vehicles.

---

## ⛽ Fuel Type Analysis

The dataset contains four fuel types:

* `X` — 514 vehicles
* `Z` — 434 vehicles
* `E` — 92 vehicles
* `D` — 27 vehicles

Fuel type `X` is the most frequently represented category in the dataset.

A count plot was also created to visualize the distribution of vehicles across fuel types.

---

## 🏭 Manufacturer Analysis

The analysis examined the most frequently represented vehicle manufacturers.

The top manufacturers by number of records include:

| Manufacturer  | Records |
| ------------- | ------: |
| FORD          |      90 |
| CHEVROLET     |      86 |
| BMW           |      64 |
| MERCEDES-BENZ |      59 |
| GMC           |      49 |
| AUDI          |      49 |
| TOYOTA        |      49 |
| PORSCHE       |      44 |
| VOLKSWAGEN    |      42 |
| DODGE         |      39 |

The analysis helps identify which manufacturers contribute the largest number of vehicles to the dataset.

---

## 📈 Correlation Analysis

A correlation matrix and heatmap were used to examine relationships between numerical variables.

Important correlations observed in the analysis include:

* **Engine Size ↔ CO₂ Emissions:** `0.874`
* **Cylinders ↔ CO₂ Emissions:** `0.850`
* **City Fuel Consumption ↔ CO₂ Emissions:** `0.898`
* **Highway Fuel Consumption ↔ CO₂ Emissions:** `0.862`
* **Combined Fuel Consumption ↔ CO₂ Emissions:** `0.892`
* **Combined MPG ↔ CO₂ Emissions:** `-0.906`

The analysis indicates strong relationships between fuel consumption, engine characteristics, fuel efficiency, and CO₂ emissions within this dataset.

---

## 💡 Key Insights

### 🔹 Dataset

* The dataset contains **1,067 vehicle records** and **13 variables**.
* All records contain complete values.
* No duplicate records were identified.

### 🔹 Fuel Consumption

* Average combined fuel consumption is approximately **11.58**.
* Average city fuel consumption is approximately **13.30**.
* Average highway fuel consumption is approximately **9.47**.

### 🔹 Fuel Efficiency

* Average combined fuel efficiency is approximately **26.44 MPG**.
* Combined MPG has a strong negative relationship with CO₂ emissions.

### 🔹 Engine Characteristics

* Average engine size is approximately **3.35**.
* The dataset includes vehicles ranging from **3 to 12 cylinders**.
* Engine size and cylinder count show strong positive relationships.

### 🔹 CO₂ Emissions

* Average CO₂ emissions are approximately **256.23**.
* CO₂ emissions range from **108 to 488**.
* Higher fuel consumption measures show strong positive relationships with CO₂ emissions.

---

## 📊 Visualizations

The project includes visualizations such as:

* ⛽ Fuel Type Distribution
* 🏭 Vehicle Manufacturer Distribution
* 📊 Fuel Consumption Analysis
* 📈 Vehicle and Engine Analysis
* 🔥 Correlation Heatmap
* 📉 CO₂ Emission Relationships

These visualizations make it easier to identify patterns and relationships within the dataset.

---

## 📂 Project Structure

```text
Fuel-Consumption-EDA/
│
├── FuelConsumption.ipynb
├── FuelConsumption.csv
└── README.md
```

---

## 🚀 How to Run the Project

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/Fuel-Consumption-EDA.git
```

### 2. Navigate to the Project Folder

```bash
cd Fuel-Consumption-EDA
```

### 3. Install Required Libraries

```bash
pip install numpy pandas matplotlib seaborn jupyter
```

### 4. Launch Jupyter Notebook

```bash
jupyter notebook
```

### 5. Open

```text
FuelConsumption.ipynb
```

Run the notebook cells sequentially to reproduce the analysis.

---

## 📌 Project Highlights

| Category                | Details                           |
| ----------------------- | --------------------------------- |
| 📊 Analysis Type        | Exploratory Data Analysis         |
| 🚗 Domain               | Automobile / Vehicle Analytics    |
| 📁 Dataset Size         | 1,067 rows × 13 columns           |
| 🐍 Language             | Python                            |
| 🧹 Data Cleaning        | Missing values & duplicate checks |
| 📈 Visualization        | Matplotlib & Seaborn              |
| 📊 Statistical Analysis | Pandas                            |
| 🔥 Correlation Analysis | Correlation Matrix & Heatmap      |
| 🌱 Environmental Metric | CO₂ Emissions                     |

---

## 🎓 Learning Outcomes

Through this project, the following skills were practiced:

* Data loading and exploration
* DataFrame manipulation using Pandas
* Numerical analysis using NumPy
* Data-quality validation
* Statistical analysis
* Categorical data analysis
* Data visualization
* Correlation analysis
* Insight generation from datasets
* Exploratory Data Analysis workflow

---

## 🔮 Future Improvements

Possible extensions of this project include:

* Building a machine-learning model to predict CO₂ emissions.
* Comparing fuel efficiency across vehicle classes.
* Performing detailed manufacturer-level comparisons.
* Applying feature engineering to improve predictive analysis.
* Creating an interactive dashboard using Power BI, Tableau, or Plotly.
* Developing a predictive model for fuel consumption.

---

## 📌 Conclusion

This project demonstrates how **Exploratory Data Analysis** can be used to understand vehicle fuel consumption and CO₂ emission patterns.

The analysis combines data-quality checks, descriptive statistics, categorical analysis, visualization, and correlation analysis to provide a structured understanding of the dataset. The results highlight strong relationships between fuel consumption, engine characteristics, fuel efficiency, and CO₂ emissions within the analyzed vehicle data.

---

## 👨‍💻 Author

**RAJAN KUMAR GUPTA**

📊 Aspiring Data Analyst | Python | SQL | Data Visualization | Exploratory Data Analysis

---

## ⭐ Support

If you find this project useful, consider giving the repository a ⭐ on GitHub.

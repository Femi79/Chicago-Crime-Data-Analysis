# Chicago Crime Data Analysis

## 📌 Project Overview

This project performs exploratory data analysis (EDA) on the Chicago Crime Dataset using Python and Pandas. The analysis focuses on cleaning the dataset, extracting useful time-based features, identifying crime trends, determining the most common crime types, analyzing crime locations, and examining how crime frequency changes over the years.

---

## 📂 Dataset

The dataset used is:

- **chicago2.csv**

It contains crime records with information such as:

- Date of occurrence
- Crime type
- Crime description
- Location
- Arrest status
- Community area
- District
- Year
- Geographic coordinates

---

## 🛠 Technologies Used

- Python 3
- Pandas
- NumPy
- Jupyter Notebook

---

## 📊 Project Tasks

### Question 1 — Data Cleaning

Performed initial preprocessing by:

- Loading the dataset
- Removing unnecessary columns:
  - `Unnamed: 0`
  - `Case Number`
  - `Latitude`
  - `Longitude`

This simplifies the dataset and removes redundant information.

---

### Question 2 — Feature Engineering

Converted the `Date` column into datetime format.

Extracted new features:

- **Month**
- **Day**
- **Season**

Season was determined using the month:

| Months | Season |
|---------|--------|
| Dec – Feb | Winter |
| Mar – May | Spring |
| Jun – Aug | Summer |
| Sep – Nov | Fall |

---

### Question 3 — Crime Trend Analysis

Grouped the dataset by:

- Month
- Day
- Season
- Crime Description

Then determined:

#### Highest Crime Periods

| Category | Result |
|----------|--------|
| Month | **July (7)** |
| Day | **3rd day of the month** |
| Season | **Spring** |

#### Crime Frequency

Most common crime:

- **SIMPLE**
- **124 occurrences**

Least common crime:

- **AGG CRIM SEX ABUSE FAM MEMBER**
- **1 occurrence**

---

### Question 4 — Crime Locations

Identified locations with the highest number of reported crimes.

Top locations:

| Location | Frequency |
|----------|-----------|
| Street | 255 |
| Residence | 169 |
| Apartment | 123 |
| Sidewalk | 87 |
| Other | 35 |

---

### Question 5 — Crime Frequency by Year

Grouped crime descriptions by year to analyze yearly trends.

### Observation

Crime frequency changes across different years, indicating that crime patterns vary over time depending on the type of crime.

---

## 📈 Key Findings

- July recorded the highest number of crime reports.
- The 3rd day of the month had the most reported crimes.
- Spring experienced the highest overall crime frequency.
- The most common crime description was **SIMPLE**.
- Streets were the most frequent crime locations.
- Crime occurrence varied from year to year.

---

## 🚀 How to Run

1. Clone this repository.

```bash
git clone https://github.com/yourusername/chicago-crime-analysis.git
```

2. Install dependencies.

```bash
pip install pandas numpy
```

3. Place `chicago2.csv` inside the project directory.

4. Open the notebook.

```bash
jupyter notebook
```

5. Run all cells.

---

## 📁 Project Structure

```
Chicago-Crime-Analysis/
│
├── chicago2.csv
├── Chicago_Crime_Analysis.ipynb
├── README.md
└── requirements.txt
```

---

## Future Improvements

- Add data visualizations using Matplotlib and Seaborn.
- Build interactive dashboards with Plotly or Power BI.
- Perform predictive crime analysis using machine learning.
- Create heatmaps of crime hotspots.
- Analyze crime trends by district and community area.

---

## Author

**Abdulmalik Ojo**

Data Analytics Project using Python and Pandas.

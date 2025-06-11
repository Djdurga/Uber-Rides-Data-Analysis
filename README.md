# Uber Rides Data Analysis using Python

This repository contains an in-depth exploratory data analysis (EDA) of Uber rides using a dataset that includes ride details like start/end times, ride purpose, category (Business or Personal), distance traveled, and city locations. The analysis was performed using Python's powerful data handling and visualization libraries.

## 📊 Project Description

This project is focused on uncovering patterns and insights from a historical dataset of Uber rides. The dataset includes detailed trip records, including:

* Timestamps for start and end of trips
* Distance in miles
* Trip purpose (Meeting, Customer Visit, Errand, etc.)
* Ride category (Business or Personal)
* Origin and destination cities

The goal of this project is to:

* Clean and preprocess the dataset
* Explore how Uber rides vary based on purpose, day of the week, and category
* Visualize distributions and frequencies of various ride metrics
* Identify frequent travel routes and patterns

The insights gained can be useful for personal travel optimization, business expense tracking, and understanding user behavior in ride-sharing applications.

---

## 🔎 Key Objectives

* Convert and parse datetime fields to proper formats
* Handle missing or null values in the dataset
* Extract new features like trip duration, weekday, and month
* Generate visualizations for trip purposes, distances, ride categories, and routes
* Understand business vs personal ride distribution

---

## 🔧 Technologies Used

* **Python**
* **Pandas** – Data manipulation
* **NumPy** – Numerical processing
* **Matplotlib** & **Seaborn** – Data visualization
* **Jupyter Notebook** – Interactive analysis

---

## 💡 Insights from EDA

### 🚗 Trip Purpose Analysis

* Most trips are business-related.
* Common purposes include `Meeting`, `Meal/Entertain`, `Errand/Supplies`, and `Customer Visit`.
* A noticeable portion of trips had no recorded purpose (marked as "Unknown").

### 🕛 Temporal Patterns

* Rides are most frequent on **weekdays**, especially on **Wednesdays and Thursdays**.
* Most rides occurred in **January** and **March**.

### ⚖️ Distance & Duration

* The majority of rides are **short-distance** (under 10 miles).
* A few outliers travel 60+ miles.
* Average trip duration is under 30 minutes.

### 🚤 Ride Category

* **Business trips** make up the majority of the dataset.
* **Personal trips** are less common, suggesting the dataset may be from an employee expense log.

### 📍 Common Routes

* Most frequent routes are within the same city (e.g., `Fort Pierce → Fort Pierce`).
* Some long-distance trips between cities such as `Fort Pierce → West Palm Beach`.

---

## 📂 Dataset Features

| Column Name | Description                                |
| ----------- | ------------------------------------------ |
| START\_DATE | Date and time when the trip started        |
| END\_DATE   | Date and time when the trip ended          |
| CATEGORY    | Business or Personal                       |
| START       | Starting city of the ride                  |
| STOP        | Destination city of the ride               |
| MILES       | Distance traveled in miles                 |
| PURPOSE     | Reason for the trip (meeting, visit, etc.) |

---

## 🔀 Data Cleaning Steps

* Converted `START_DATE` and `END_DATE` to datetime objects using `pd.to_datetime()`
* Created a new `DURATION` column in minutes
* Handled missing values in the `PURPOSE` column by filling with `'Unknown'`
* Generated new columns like `WEEKDAY`, `MONTH`, and `ROUTE` for deeper insights

---

## 🖋️ Visualizations

* **Trip Purpose Count Plot**: Showcased most common trip purposes
* **Distance Histogram**: Displayed how far most rides travel
* **Trips by Weekday & Month**: Highlighted when people ride the most
* **Category Comparison**: Compared Business vs Personal rides
* **Top Routes**: Showed the most traveled routes in the dataset

---

## 📁 Folder Structure

```
Uber-Rides-EDA/
├── UberDataset.csv
├── Uber_EDA.ipynb
└── README.md
```

---

## ✨ How to Run

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/Uber-Rides-EDA.git
   cd Uber-Rides-EDA
   ```

2. Install dependencies:

   ```bash
   pip install pandas matplotlib seaborn
   ```

3. Run the notebook:

   ```bash
   jupyter notebook Uber_EDA.ipynb
   ```

---

## 👩‍💼 Author

**Durga Rani**
M.Tech Data Science & AI (2024–2026)


---

## 💌 Contributions & Feedback

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change or improve.

If you found this project helpful, feel free to give it a star ⭐!

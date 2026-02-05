# 🚖 NYC Taxi Trip Analysis: Cash vs. Card Hypothesis

![Python](https://img.shields.io/badge/Python-3.8%2B-blue) ![Library](https://img.shields.io/badge/Library-Pandas%20|%20SciPy-orange) ![Status](https://img.shields.io/badge/Status-Completed-green)

## 📋 Project Overview
This project analyzes a dataset of NYC Yellow Taxi trips to investigate payment behaviors and trip characteristics. The core focus was to test the relationship between **payment methods** (Card vs. Cash) and **trip fare/distance**, providing data-driven insights into passenger spending habits.

## 🔍 Key Insights (The Findings)
Through rigorous statistical testing and data segmentation, the following patterns emerged:

* **The "Card" Premium:** Customers paying with **Credit Cards** tend to have significantly higher average fares and longer trip distances compared to Cash users.
* **Payment Preference:** Credit Card is the dominant payment method, accounting for a larger share of transaction volume than Cash.
* **Trip Distance Dynamics:** There is a strong positive correlation between trip distance and fare amount, confirming the linear pricing structure of the taxi system.
* **Passenger Count:** Most trips involve single passengers, with larger groups (5+ passengers) being rare outliers.

## 🛠️ Technical Approach

### 1. Data Cleaning & Preprocessing
* **Filtering:** Removed invalid transactions, such as negative fare amounts and trips with 0 distance, to ensure data integrity.
* **Type Conversion:** optimized memory usage by converting datetime columns (`tpep_pickup_datetime`, `tpep_dropoff_datetime`) for accurate duration calculations.
* **Outlier Handling:** Identified and segmented high-value outliers to prevent skewed averages.

### 2. Statistical Analysis (Hypothesis Testing)
* **T-Test Implementation:** Conducted a T-test to statistically verify if the difference in average fare between Card and Cash users was significant.
* **Result:** The p-value was effectively **0.0**, rejecting the Null Hypothesis. This statistically proves that payment method *does* influence transaction value—Card users spend more.

## 🚀 How to Run
1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/yourusername/NYC-Taxi-Analysis.git](https://github.com/yourusername/NYC-Taxi-Analysis.git)
    ```
2.  **Install dependencies:**
    ```bash
    pip install pandas numpy scipy matplotlib
    ```
3.  **Run the Notebook:**
    Open `taxi.ipynb` to view the code and statistical outputs.


**Developer:** Dweep Shishodia
**Role:** Data Science Undergraduate @ IIT Madras

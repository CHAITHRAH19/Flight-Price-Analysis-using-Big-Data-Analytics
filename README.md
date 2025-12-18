# Flight Price Analysis using Big Data Analytics ✈️📊

## Project Overview

This project demonstrates the use of **Big Data technologies** to analyze airline flight pricing patterns at scale. Using **Apache Hadoop (HDFS)** and **PySpark**, the project processes large flight datasets to extract actionable insights such as average fare by airline, most frequent flight routes, and price distribution over time.

The project highlights how distributed storage and parallel processing can be leveraged for **data-driven decision-making in the aviation industry**.

---

## Objectives

* Store large flight datasets using **HDFS**
* Perform distributed data processing using **PySpark**
* Analyze airline pricing trends and route frequencies
* Apply MapReduce-style transformations for scalability
* Generate analytical outputs for strategic insights

---

## Technologies Used

* **Apache Hadoop (HDFS & YARN)**
* **Apache Spark (PySpark)**
* **Docker** (containerized Hadoop & Spark cluster)
* **Jupyter Notebook**
* **Python**
* **CSV Dataset (Flight Pricing Data)**

---

## Dataset

* **Type:** Flight pricing and route data
* **Format:** CSV
* **Size:** Large-scale dataset suitable for distributed processing
* **Key Attributes:**

  * Airline name
  * Total fare
  * Flight date
  * Origin and destination airports
  * Route frequency

---

## System Architecture

* Hadoop cluster deployed using **Docker**
* HDFS for distributed storage
* Spark Master & Worker nodes for parallel computation
* PySpark connected to HDFS for data processing
* Jupyter Notebook for interactive analysis

---

## Key Analyses Performed

### 1. Average Fare by Airline

* Calculates the mean flight price for each airline
* Helps identify pricing strategies across carriers

### 2. Most Frequent Flight Routes

* Identifies routes with the highest number of flights
* Useful for demand and route optimization analysis

### 3. Price Distribution by Date

* Computes average fare and flight count per day
* Reveals temporal price trends and demand patterns

---

## Output Data (Stored in HDFS)

```
/flightresults/
│── average_price_by_airline.csv
│── most_frequent_routes.csv
│── price_distribution_by_date.csv
```

---

## How to Run the Project

1. **Start Hadoop & Spark Cluster**

   ```bash
   docker-compose up -d
   ```

2. **Upload Dataset to HDFS**

   ```bash
   hdfs dfs -put flightdataset.csv /flightdata/
   ```

3. **Launch Jupyter Notebook**

   * Access via `http://localhost:8888`
   * Run PySpark notebooks for analysis

4. **View Results**

   * Output CSV files stored in HDFS
   * Can be downloaded for further analysis

---

## Key Insights

* Airline pricing varies significantly across carriers
* Certain routes dominate flight frequency
* Fare trends fluctuate based on travel dates
* Big Data tools enable efficient large-scale analytics

---

## Future Enhancements

* Predictive pricing using Machine Learning
* Real-time data ingestion
* Advanced route profitability analysis
* Integration with live airline APIs

---

⭐ *If you find this project useful, feel free to star the repository!*

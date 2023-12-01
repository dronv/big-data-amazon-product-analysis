# Amazon Product Analysis

## Overview

This repository contains a PySpark and Dash application for analyzing and visualizing data from an Amazon product dataset. The analysis covers various aspects such as discounts, prices, ratings, and popularity. The results are presented in an interactive Dash dashboard.

## Prerequisites

- Apache Spark
- Hadoop Distributed File System (HDFS)
- Python libraries: `pyspark`, `dash`, `dash-bootstrap-components`, `matplotlib`, `plotly`

## Running the Application

### PySpark and Dash Setup

1. **Spark Session Setup:**
   - Make sure Apache Spark is installed and properly configured.
   - Open your browser and go to http://localhost:8080 to view the Spark master web interface.

2. **Install Required Python Libraries:**
   ```bash
   pip install pyspark dash dash-bootstrap-components matplotlib plotly

## Connecting Master and Worker Clusters
<img width="918" alt="localhost_spark_connected_workers" src="https://github.com/dronv/big-data-amazon-product-analysis/assets/41694884/737c0789-213b-46bf-9a26-42499e0f0d58">

### Windows Machine
  #### 1. Master Cluster
  ```bash
  spark-class org.apache.spark.deploy.master.Master
  ```
  #### 2. Worker Cluster
  ```bash
  spark-class org.apache.spark.deploy.worker.Worker spark://your-master-node:port
  ```

### Linux Machine
  #### 1. Master Cluster
  ```bash
  ./sbin/start-master.sh
  ```
  #### 2. Worker Cluster
  ```bash
  ./sbin/start-worker.sh spark://your-master-node:port
  ```
## HDFS Setup
  ### Windows Machine
  #### 1. Start DFS services:
  ```bash
  start-dfs
  ```
  #### 2. Start yarn services:
  ```bash
  start-yarn
  ```
  ### Linux Machine
  #### 1. Start DFS services:
  ```bash
  ./sbin/start-dfs.sh
  ```
  #### 2. Start yarn services:
  ```bash
  ./sbin/start-yarn.sh
  ```

### Access HDFS Web Interface:
Open your browser and go to http://localhost:9870 to view the HDFS web interface.

## Dashboard
  Access the Dash Dashboard:
  
  Open your browser and go to http://localhost:8050.
  Navigate through different sections:
  
  ~ Discount Analysis
  ~ Price Analysis
  ~ Ratings Analysis
  ~ Popularity Analysis

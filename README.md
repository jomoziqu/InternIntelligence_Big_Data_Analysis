# NYC Taxi Trip Data Analysis with PySpark

## Overview
This project analyzes NYC Taxi Trip Record Data using PySpark to uncover patterns in passenger behavior, fare economics, and geospatial demand hotspots. The analysis includes temporal trends, machine learning (trip duration prediction), and comparisons between weekdays/weekends.

---

## Dataset
**Source**: [NYC TLC Trip Record Data](https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page)  
**Files Used**:  
- `yellow_tripdata_2019-01.csv` (main trip data)  
- `taxi_zone_lookup.csv` (geospatial zone metadata)  

**Columns of Interest**:  
- Temporal: `tpep_pickup_datetime`, `tpep_dropoff_datetime`  
- Fare: `total_amount`, `fare_amount`, `tip_amount`, `tolls_amount`  
- Trip Details: `passenger_count`, `trip_distance`, `PULocationID` (pickup zone)  

---

## Setup

### Prerequisites
- **Apache Spark**: Install via [Spark Documentation](https://spark.apache.org/docs/latest/)  
- **Python Libraries**:  
  ```bash
  pip install pyspark pandas matplotlib seaborn

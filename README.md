# Capstone Project: Predicting NYC Taxi Fare

## 🚖 Project Overview
This project develops a predictive model for NYC taxi fares using trip records. By analyzing factors like trip distance, passenger count, and pickup/dropoff locations, it improves fare estimation and optimizes pricing strategies.

---

## Data Dictionary

### Dataset 1 (Model Building)
- `VendorID`: Taxi vendor identifier
- `tpep_pickup_datetime`: Trip start timestamp
- `tpep_dropoff_datetime`: Trip end timestamp
- `passenger_count`: Number of passengers
- `trip_distance`: Distance of the trip in miles
- `RatecodeID`: Trip rate code
- `store_and_fwd_flag`: Data storage and forwarding flag
- `PULocationID`: Pickup location zone ID
- `DOLocationID`: Dropoff location zone ID
- `payment_type`: Payment method used
- `fare_amount`: Base fare amount
- `extra`: Additional charges
- `mta_tax`: Mandatory MTA tax
- `tip_amount`: Tip amount
- `tolls_amount`: Toll charges
- `improvement_surcharge`: NYC transportation improvement surcharge
- `total_amount`: Total fare amount
- `congestion_surcharge`: Congestion surcharge

### Dataset 2 (Mapping and Analysis)
- `key`: Unique trip identifier
- `fare_amount`: Total fare (USD)
- `pickup_datetime`: Trip start time
- `pickup_longitude`, `pickup_latitude`: Pickup location
- `dropoff_longitude`, `dropoff_latitude`: Dropoff location
- `passenger_count`: Number of passengers

---

## Methodology
1. **Data Cleaning**:
   - Removed outliers (e.g., negative fares or zero passenger counts).
   - Standardized datetime and location data.

2. **Feature Engineering**:
   - Calculated trip distance (haversine).
   - Extracted time-based features (hour, day of the week).

3. **Modeling**:
   - Baseline: Linear Regression
   - Advanced: Random Forest, Gradient Boosting

4. **Evaluation**:
   - Metrics: RMSE, MAE, R²
   - Cross-validation for robustness.

---

## Interactive Visualization
1. **Interactive Map**:
   - Visualizes pickup and dropoff locations in separate layers.
   - Highlights high-demand areas like Midtown Manhattan and Financial District using polygons.
   - Includes landmarks such as JFK Airport, Times Square, and Central Park.

   
2. **Predictive Modeling**：
- Developed two predictive models:
  1. **Linear Regression**:
     - RMSE: 6.98, R²: 0.71.
     - Simple, interpretable, and effective for this dataset.
  2. **Random Forest Regression**:
     - RMSE: 7.71, R²: 0.65.
     - Handles non-linear patterns but underperformed due to limited features and hyperparameter tuning.

- Model Comparison:
  - Linear Regression outperformed Random Forest in accuracy and simplicity.
  - Random Forest could benefit from further tuning and inclusion of location-based features (e.g., geospatial clustering of zones).
    
---

## Results
- **Key Factors**:
  - Trip distance and time of day are the most significant predictors of taxi fares.
- **Model Insights**:
  - Advanced models outperform baseline models in fare prediction accuracy.
- **Visual Discoveries**:
  - High-demand areas and airport routes consistently show higher fare trends.
  - Heatmaps reveal concentrated taxi activity in Manhattan and at major airports.
- **Practical Application**:
  - The model provides actionable insights for pricing strategies and trip cost estimations.

---

## Acknowledgments
- The dataset is sourced from [Kaggle's NYC Taxi Fare Data Exploration](https://www.kaggle.com/code/breemen/nyc-taxi-fare-data-exploration/notebook).
- Geospatial data and map visualizations are powered by [OpenStreetMap](https://www.openstreetmap.org/export#map=9/40.711/-73.659).


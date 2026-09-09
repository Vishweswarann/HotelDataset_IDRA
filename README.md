# Hotel Booking Dataset - Exploratory Data Analysis (EDA)

This repository contains an end-to-end Exploratory Data Analysis (EDA) on a large hotel booking dataset. The project demonstrates a complete data science workflow, from initial data loading and quality assessment to deep visual analysis and the generation of actionable business insights.

## Overview

The primary objective of this project is to clean, preprocess, and analyze raw hotel booking data to uncover underlying patterns related to cancellations, average daily rate (ADR) optimization, and customer behavior. The final output is an executive-ready report designed to guide management decisions.

### Key Analysis Phases

1. **Data Loading & Quality Assessment**
   - Initial review of data shape, types, and non-null counts.
   - Identification of missing values in key columns like `Company_ID` and `Agent_ID`.

2. **Data Cleaning & Preprocessing**
   - Imputation of missing values (e.g., treating blank `Children` as 0, mapping missing agent IDs to a baseline).
   - Conversion of date strings (`Booking_Date`, `Arrival_Date`, `Reservation_Status_Date`) into pandas datetime objects.
   - Removal of duplicate records to ensure data integrity.
   - Basic outlier filtering, specifically targeting anomalous negative or extreme ADR values.

3. **Univariate & Bivariate Analysis**
   - Visualizing the overall distribution of canceled vs. non-canceled bookings.
   - Comparing cancellation rates between City Hotels and Resort Hotels.

4. **Group-wise Analysis**
   - Evaluating Average Daily Rate (ADR) distribution across various Market Segments using boxplots.
   - Analyzing the density of Lead Time (days between booking and arrival) and its correlation with cancellation status.

5. **Correlation Analysis**
   - Generating a heatmap to visualize the linear relationships between key numerical variables (e.g., Lead Time, Total Nights, ADR, Previous Cancellations).

6. **Executive Summary & Recommendations**
   - Translating visual and statistical findings into practical, actionable recommendations for hotel revenue and operations management.

## Files Included

* `hotel_booking_dataset.csv`: The raw input dataset (requires placement in the root directory).
* `Executive_EDA_Hotel_Bookings.ipynb`: The Jupyter Notebook containing the full Python code, visualizations, and the executive report.
* `README.md`: This project overview file.
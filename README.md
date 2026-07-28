# Asheville-Airbnb-Listings-Analysis

The goal of this project is to evaluate pricing, demand, and host activity trends to help a travel startup decide whether to expand services in Asheville.

# Key Objectives :
 - What pricing trend looks like?
 - Which neighborhoods and hosts are most active?
 - what review activity says about demand
# Tools Used
- pandas for data cleaning and analysis
- matplotlib and seaborn for visualization
# Methodology
1. Datasets
Two datasets were utilized for this analysis:
 - Listings dataset: Contains detailed information about each property, including id, name, host_id, host_name, neighbourhood, room type, price, and other relevant attributes.
 - Reviews dataset: Includes listing_id and review date.
 2. Data cleaning
    - Removed irrelevant columns to improve data quality
    - Identified and eliminated duplicate records, particularly in the reviews dataset, where 714 duplicate rows were removed.
    - Handled missing values in the listings dataset.Replaced missing values in reviews_per_month and price using the median, ensuring robustness against outliers.
    - Detected outliers and applied the capping (winsorization) technique, limiting values to the 1st and 99th percentiles to minimize their impact.
    - Merged the listings and reviews datasets to create a unified dataset for analysis.

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
1. Datasets.
Two datasets were utilized for this analysis:
 - Listings dataset: Contains detailed information about each property, including id, name, host_id, host_name, neighbourhood, room type, price, and other relevant attributes.
 - Reviews dataset: Includes listing_id and review date.
 2. Data cleaning
    - Removed irrelevant columns to improve data quality
    - Identified and eliminated duplicate records, particularly in the reviews dataset, where 714 duplicate rows were removed.
    - Handled missing values in the listings dataset.Replaced missing values in reviews_per_month and price using the median, ensuring robustness against outliers.
    - Detected outliers and applied the capping (winsorization) technique, limiting values to the 1st and 99th percentiles to minimize their impact.
    - Merged the listings and reviews datasets to create a unified dataset for analysis.
# Key Findings

- Price distribution.

The average price ($169) is significantly higher than the median price ($128), indicating a right-skewed distribution. 
This suggests that while most listings are relatively affordable, a smaller number of high-priced listings, especially for premium listing are pulling the average upward.

  <img width="2538" height="1398" alt="Distribution of listings price" src="https://github.com/user-attachments/assets/60089453-b767-4ae0-854c-9fa89528c531" />


 - Growth Trends.
    
Airbnb activity in Asheville experienced a rapid expansion since 2012, with a slowdown around 2020, probably due to COVID-19.
A steady growth was observed since 2021, with a spike in 2023 before dipping in 2024.

<img width="1747" height="1352" alt="Yearly trends of Airbnd in Ashville" src="https://github.com/user-attachments/assets/d11e41ce-a9ea-4a42-aa48-90263425a7b9" />



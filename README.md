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
   - Two datasets used for this analysis: the listings dataset contains information about each property:
     (id, name, host_id, host_name, neighbourhood, room_type, price,minimum_nights, availability_365,number_of_reviews,reviews_per_month, last_review etc..) and reviews dataset with:
     (listing_id, date)
 2. Data cleaning
    - Dropped irrelevant columns
    - Dropped duplicate rows, especially in the reviews dataset. 714 duplicate rows were deleted.
    - Handled missing values in the listings dataset: reviews_per_month and Price missing values were replaced with their median values.
    - Identified outliers and used the capping method to replace them with the 1st and 99th percentile
    - Merged the listings and reviews datasets.

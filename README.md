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
There is no correlation between price and minimum stay, but the analysis showed that short stay (1-2 nights) has a higher volume compared to any other stay.

 - Growth Trends.
    
Airbnb activity in Asheville experienced a rapid expansion since 2012, with a slowdown around 2020, probably due to COVID-19.
A steady growth was observed since 2021, with a spike in 2023 before dipping in 2024.
The demand analysis also showed a massive upward trend in months like May, July, and October. 

- Property distribution.
  
The market is heavily dominated by Entire homes/apartments with 89% of market share, followed by private rooms with 9.9%
Neighborhoods 28806, 28801. 28803, 28804, and 28805 are the top in both listings and guest reviews make them more competitive in the Asheville Airbnb market.
Neighborhoods 28732 and 28704 have the highest average price, suggesting potential premium listings.
Hosts with multiple listings have a higher price ($144.70) compared to single listings ($125.24)

# Conclusion

The Asheville Airbnb market demonstrates solid growth potential, making it an attractive opportunity for new business entrants. 
A dual strategy focused on entire home listing in high-demand neighborhoods such as 28806 and 28801 can drive volume through competitive pricing, while
targeting areas like 28732 for premium offerings can optimize profitability. Furthermore, with demand peaks in May, July, and October, enables dynamic
pricing strategies to maximize on high-demand periods overall returns.

<img width="2538" height="1398" alt="Distribution of listings price" src="https://github.com/user-attachments/assets/60089453-b767-4ae0-854c-9fa89528c531" />
<img width="1701" height="1352" alt="Correlation between price and minimum nights" src="https://github.com/user-attachments/assets/a193a252-5ef0-450d-809b-dc3476fc8f2e" />
<img width="1747" height="1352" alt="Yearly trends of Airbnd in Ashville" src="https://github.com/user-attachments/assets/d11e41ce-a9ea-4a42-aa48-90263425a7b9" />
<img width="2584" height="1398" alt="Airbnd Trend by month" src="https://github.com/user-attachments/assets/728e023a-fa9f-420d-9104-a7244bc94182" />
<img width="2561" height="1399" alt="Distribution of room-type in Ashville" src="https://github.com/user-attachments/assets/79025004-b103-4a51-841f-7e0cfdde7a24" />
<img width="1646" height="1422" alt="Active listings per neighhborhood" src="https://github.com/user-attachments/assets/4a0fc431-93c9-4044-a644-2117eb2b10e5" />
<img width="1646" height="1351" alt="Average price distribution by neighbourhood" src="https://github.com/user-attachments/assets/f196520e-2acd-4880-b18c-104de97ac3a2" />
<img width="2018" height="1398" alt="Single Host vs Multipe Host avg price" src="https://github.com/user-attachments/assets/567907e5-9d76-46ef-b01c-c31520421feb" />






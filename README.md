------------------------------------------------------------------------------------------------------------------------------------------ 
### Crime Data Analysis (LAPD Dataset)
------------------------------------------------------------------------------------------------------------------------------------------ 
**Project Overview**

This project analyzes crime data to identify patterns, trends, and key risk factors such as time, location, and weapon usage. The goal is to derive actionable insights that can support better decision-making.

### Objectives

*  Identify most common crime types
*  Analyze crime distribution by hour and day
*  Detect high-crime areas
*  Study weapon usage patterns
*  Understand crime trends over time

## Tools & Technologies

*  Python (Pandas, NumPy)
*  Data Visualization (Matplotlib, Seaborn)

 ## Data Cleaning & Preparation
 
*  Converted date columns to datetime
*  Created full_occ_datetime feature
*  Handled missing values (domain-based decisions)
*  Removed duplicates
*  Standardized column names
------------------------------------------------------------------------------------------------------------------------------------------ 
### Visualizations
------------------------------------------------------------------------------------------------------------------------------------------ 
#### Crime per hours

![](ldownload(2).png)
  
  **Why was a bar chart chosen for the 'Which hour of the day has highest crime?**
    A bar chart was selected because it is highly effective for visualizing and comparing discrete categories (the 24 hours of the day) and their corresponding numerical values (the count of crimes). Its distinct bars facilitate easy identification and comparison of crime frequencies across each hour, highlighting peaks and troughs.

**Data Analysis Key Findings**
*   The early morning hours consistently show the lowest crime rates, with 5 AM having the fewest crimes (476 incidents), followed by 4 AM (542 crimes) and 6 AM (615 crimes).
*   Crime activity generally increases in the late morning and peaks in the afternoon and early evening. The hour with the highest crime count is 12 PM (1650 crimes), followed by 8 PM (1617 crimes) and 6 PM (1579 crimes).
*   Crime rates are low in the very early morning, gradually increase throughout the day, reach their highest levels in the afternoon and evening, and then start to decline late at night.
------------------------------------------------------------------------------------------------------------------------------------------ 
#### Crimes on Days

![](ldownload(3).png)
 
  **Why was a bar chart chosen to visualize the 'Crimes on Days' ?**
A bar chart was chosen for the 'Which day has highest crime?' analysis because it is an effective visualization for comparing discrete categories (the days of the week) and their corresponding numerical values (the count of crimes). The distinct bars make it easy to quickly identify and compare crime frequencies across different days.

**Data Analysis Key Findings**

*   **Visualization Choice**: A bar chart was selected for its effectiveness in comparing discrete categories (days of the week) and their corresponding numerical values (crime counts), allowing for clear visual identification of differences and rankings.
*   **Peak Crime Day**: Friday had the highest number of reported crimes, with 4541 incidents.
*   **High Crime Days**: Thursday (4263 crimes) and Saturday (4252 crimes) also showed significantly high crime rates, contributing to an overall increase in criminal activity towards the end of the week.
*   **Lowest Crime Day**: Tuesday recorded the lowest number of crimes, with 3741 incidents, making it the day with the least criminal activity.
*   **General Trend**: Crime rates exhibit an upward trend towards the end of the week, peaking around Friday, Thursday, and Saturday, and are lowest at the beginning of the week, particularly on Tuesday.
------------------------------------------------------------------------------------------------------------------------------------------

#### Distribution of Total Victim Count by Crime Against Category

![](download(lastbut).png)

*   **Why was a box plot chosen for this analysis?**

    A box plot was chosen to visualize the distribution of 'Total victim count' across Crime Against categories because it effectively displays the spread, central tendency (median), and potential outliers within numerical data for each category. It allows for easy comparison of these distributions across different crime types.

**Data Analysis Key Findings**

*   **Property Crimes**: Typically, 'Property' crimes tend to have a lower median 'Total victim count', often around one, and a narrower interquartile range, suggesting that most property-related incidents affect a single entity or have a more consistent victim count.
*   **Society Crimes**: These crimes also generally show a lower median victim count, similar to property crimes, but their distribution might vary depending on the specific nature of the societal offense.
------------------------------------------------------------------------------------------------------------------------------------------ 
#### Most common crimes

![](ldownload(1).png)

**Why was a bar chart chosen to visualize the 'Top 10 most frequent crimes'?**
    A bar chart was chosen because it effectively compares discrete categories (crime types) and their corresponding numerical values (counts), making it easy to identify the most frequent crimes and compare their occurrences.

**Data Analysis Key Findings**
*   The most prevalent crime identified is '487(D)(1) - PC - F - Grand Theft Auto - GTA - 240', accounting for 2201 incidents.
*   The second most common crime is '594(B)(1) - PC - F - Vandalism (\$400 Or More) - Felony - 290', with 2135 incidents.
*   '243(A) - PC - M - Battery On Person - Simple - 13B' ranks as the third most frequent crime, with 1641 incidents.
*   There is a significant decrease in the number of incidents between the top few crimes and those lower down the list, indicating that a small number of crime types are disproportionately frequent.

------------------------------------------------------------------------------------------------------------------------------------------ 
#### High-risk areas

![](ldownload(5).png)

**Why was a bar chart chosen to visualize the 'High-risk areas'?**
A bar chart was chosen to visualize the top 5 crime areas because it is ideal for comparing discrete categories (different geographic areas) and their corresponding numerical values (crime counts). Its clear, distinct bars make it easy to quickly identify and rank the areas with the highest crime frequencies.

**Insights from the `area_wise_crime` Bar Plot:**
Based on the 'area_wise_crime' bar plot, the areas with the highest crime occurrences are:

*  Central
*  N Hollywood
*  77th Street
*  Hollywood
*  Southwest

These areas consistently show the highest number of reported crimes, suggesting they are critical zones for resource allocation and crime 
prevention efforts.

------------------------------------------------------------------------------------------------------------------------------------------ 
#### Majority crimes involve(Weapon or No weapon)

![](ldownload(4).png)

*   **Why was a bar chart chosen for the weapon analysis?**
    A bar chart was chosen because it is highly effective for comparing discrete categories, such as 'crimes committed with a weapon' versus 'crimes committed without a weapon', and their corresponding numerical values. The clear separation of bars allows for a quick visual comparison of the frequency of each category.

**Data Analysis Key Findings**
*   The bar chart clearly shows that crimes committed without a weapon significantly outnumber those committed with a weapon.
*   Specifically, there were 20,437 crimes reported as 'no\_weapon' compared to 8,153 crimes reported as 'with\_weapon'
------------------------------------------------------------------------------------------------------------------------------------------ 
#### Crime Frequency by Day and Hour

![](ldownload(6).png)

 **Data Analysis Key Findings**
*   Crimes are most frequent during late afternoon and evening hours, specifically between 4 PM (16:00) and 9 PM (21:00).
*   The lowest crime rates consistently occur in the early morning hours, particularly between 2 AM (02:00) and 5 AM (05:00).
*   Friday and Thursday exhibit higher overall crime counts compared to other days, especially during peak hours. This finding aligns with a previous 'day_wise_theft' analysis.
*   Saturday also shows significant crime activity, predominantly in the afternoon and evening.
*   Sunday, Monday, and Tuesday generally have relatively lower crime rates throughout the day compared to the end of the week.
*   Specific crime hotspots are observable on Friday and Thursday evenings, indicating these as particularly vulnerable times.
------------------------------------------------------------------------------------------------------------------------------------------ 

#### Daily Crime Trend

![](ldownload(7).png)

 **Data Analysis Key Findings**
*   The crime data was successfully grouped by the date component of the 'full_occ_datetime' column.
*   A total of 608 unique dates recorded crime occurrences.
*   No distinct long-term trend (e.g., increasing or decreasing) was identified from the observed period.
*   Specific spikes were observed on certain days, indicating instances of unusually high crime activity.
------------------------------------------------------------------------------------------------------------------------------------------ 
#### Distribution of Crimes by "Crime Against" Category'
![](download(last).png)

  **Why was a pie chart chosen for this analysis?**
    A pie chart was selected to visualize the distribution of crimes by the 'Crime Against' category because it is effective for showing the proportion of each category relative to the whole. Since 'Crime Against' typically has a limited number of distinct categories, a pie chart provides a clear and intuitive representation of their percentage contribution.

**Data Analysis Key Findings**
*   The pie chart illustrates that 'Person' is the most dominant category, accounting for a significant majority of crimes. This indicates that crimes directly impacting individuals are the most frequently reported.
*   'Property' crimes also represent a substantial portion of the total, suggesting that offenses against assets and possessions are common.
*   'Society' crimes make up a smaller, but notable, percentage, pointing to offenses that impact the community or public order.
*   The 'Unknown' category represents a very small fraction, indicating that most crimes have a specified target.

**Insights or Next Steps**
*   The overwhelming proportion of 'Person' crimes highlights the need for strategies focused on victim protection and reducing person-on-person offenses.
*   Further investigation into the types of 'Person' and 'Property' crimes could provide deeper insights for targeted prevention efforts.
*   Understanding the specific nature of 'Society' crimes can help in developing community-oriented policing strategies.
------------------------------------------------------------------------------------------------------------------------------------------
### Business Recommendations

*  Resource Allocation (Police Deployment)**

Increase patrols during peak crime hours (from your occ_hour analysis)
Focus more officers on high-crime days
*  High-Risk Area Monitoring**

Deploy surveillance (CCTV, patrol units) in top crime areas
Create crime hotspot zones
*  reventive Policing**

Target top crime types with specific strategies
Example: theft → awareness campaigns, better lighting
*  Weapon Control Measures**

If weapon crimes are significant:
Increase weapon checks & enforcement
If “No weapon” dominates:
Focus on petty crime prevention
*  Time-Based Strategy**

Night vs day patterns → adjust staffing shifts
Weekend spikes → increase weekend policing
*  Data-Driven Decision Making

Build dashboards for real-time monitoring
Continuously track trends and update strategies

------------------------------------------------------------------------------------------------------------------------------------------ 
### Conclusion

This project demonstrates end-to-end data analysis including data cleaning, feature engineering, and visualization, providing meaningful insights from raw data.

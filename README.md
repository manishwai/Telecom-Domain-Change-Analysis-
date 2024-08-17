# Telecom-Domain-Change-Analysis-
![image](https://github.com/user-attachments/assets/cb9066c2-4f10-4c87-94cb-d228cdb360fd)




# Telecom Domain Change Analytics

## Background

- **Company**: AtliQo, a leading telecom provider in India.
- **Event**: Launched 5G plans in May 2022.
- **Issue**: Decline in active users and revenue growth observed post-5G launch.
- **Request**: Management has requested a comparative analysis of KPIs for periods before and after the 5G launch.

## Objective

The goals of this analysis are:

- **Comparative Reporting**: Prepare a comparative report and dashboard showcasing changes in KPIs before and after the 5G launch.
- **Insights & Opportunities**: Identify key areas for improvement, including:
  - Cities needing immediate attention.
  - Non-profitable plans.
  - Changes in market size and customer behavior.

## Approach

1. **Data Collection**:
   - Gather data from pre- and post-5G launch periods.
   - Include metrics such as active users, revenue, plan adoption rates, and market share.

2. **Data Analysis**:
   - Compare KPIs between the two periods.
   - Utilize statistical and visualization tools to identify trends and insights.

3. **Dashboard Creation**:
   - Develop an interactive dashboard to visualize the comparative analysis and key metrics.
   - Include features for exploring data and insights interactively.

4. **Insight Generation**:
   - Identify significant changes and anomalies.
   - Provide recommendations based on the analysis to address issues and leverage opportunities.

## Expected Deliverables

- **Comparative Report**: Detailed analysis comparing pre- and post-5G launch KPIs.
- **Interactive Dashboard**: Visual representation of key metrics and comparative data.
- **Insights & Recommendations**: Actionable insights and strategic recommendations based on the analysis.

## Data Overview

We have 6 CSV files:

1. `dim_cities`
2. `dim_date`
3. `dim_plan`
4. `fact_atliqo_metrics`
5. `fact_market_share`
6. `fact_plan_revenue`

### Column Descriptions

#### `dim_cities`

1. **city_code**: Unique code assigned to each city.
2. **city_name**: Name of the city corresponding to the city code.

#### `dim_date`

1. **date**: Starting date of each month.
2. **month_name**: Abbreviated name of the month (e.g., Jan, Feb, Mar). Includes months from January to September, excluding May.
3. **before/after_5g**: Category indicating the period before or after 5G implementation. Categories are "Before 5G" and "After 5G". January to April represents the period before 5G, and June to September represents the period after 5G.
4. **time_period**: Unique sequence number ranging from 1 to 4 for comparison periods before and after 5G (e.g., Jan vs. Jun, Feb vs. Jul, Mar vs. Aug, Apr vs. Sep).

#### `dim_plan`

1. **plan**: Name of the internet plan provided by Atliqo.
2. **plan_description**: Brief description of the internet plan.

#### `fact_atliqo_metrics`

1. **date**: Starting date of each month.
2. **city_code**: Unique code for each city.
3. **company**: Name of the company (always Atliqo in this dataset).
4. **atliqo_revenue_crores**: Revenue generated by Atliqo in crores for that month in the specified city (1 Crore = 10 Million).
5. **arpu**: Average revenue per user (ARPU) in that city for the specified month.
6. **active_users_lakhs**: Number of active users in lakhs (1 Lakh = 100,000) in that city for the specified month.
7. **unsubscribed_users_lakhs**: Number of unsubscribed users in lakhs in that city for the specified month.

#### `fact_market_share`

1. **date**: Starting date of each month.
2. **city_code**: Unique code for each city.
3. **tmv_city_crores**: Total market value in crores for the city for that month (1 Crore = 10 Million).
4. **company**: Competitor names in the telecom industry (e.g., Atliqo, Britel, DADAFONE, PIO, Others).
5. **ms_pct**: Market share percentage of the company from the total market value for that city in the specified month.

#### `fact_plan_revenue`

1. **date**: Starting date of each month.
2. **city_code**: Unique code for each city.
3. **plans**: Name of the internet plan provided by Atliqo.
4. **plan_revenue_crores**: Revenue generated from the respective plan in crores for that month in the specified city (1 Crore = 10 Million).

## Data Model 
![Example PNG](https://i.imgur.com/yfR1ToD.png)

## Metrics

- **Total Revenue**: Sum of Atliqo's revenue across all periods.
- **Average Revenue**: Average revenue generated by Atliqo.
- **Average Revenue Per User**: Average revenue per user (ARPU) for Atliqo.
- **Total Active Users**: Sum of active users using Atliqo's services.
- **Total Unsubscribed Users**: Sum of unsubscribed users from Atliqo's services.
- **Monthly Active Users**: Average number of active users per month.
- **Market Share %**: Average market share percentage of Atliqo.
- **Revenue Before 5G**: Total revenue for all periods before the implementation of 5G.
- **Revenue After 5G**: Total revenue for all periods after the implementation of 5G.
- **ARPU Before 5G**: Average revenue per user for periods before the implementation of 5G.
- **ARPU After 5G**: Average revenue per user for periods after the implementation of 5G.
- **Active Users Before 5G**: Total active users for all periods before the implementation of 5G.
- **Active Users After 5G**: Total active users for all periods after the implementation of 5G.
- **Unsubscribed Users Before 5G**: Total unsubscribed users for all periods before the implementation of 5G.
- **Unsubscribed Users After 5G**: Total unsubscribed users for all periods after the implementation of 5G.

## Tasks

### KPI Comparative Report
- **Total Revenue Analysis**: 
  - Provide insights on total revenue.
  - Compare revenue after the 5G launch with revenue before the 5G launch.
  - Analyze the change in revenue.
- **Active Users Analysis**: 
  - Provide insights on total active users.
  - Compare active users after the 5G launch with active users before the 5G launch.
  - Analyze the change in the number of active users.
- **Average Revenue Per User (ARPU) Analysis**: 
  - Provide insights on average revenue per user.
  - Compare ARPU after the 5G launch with ARPU before the 5G launch.
  - Analyze the change in ARPU.
- **Users Lost Analysis**: 
  - Analyze the number of users lost after the 5G launch.

### Recharge Plan Analysis
- **Monthly Revenue Analysis**: 
  - Analyze revenue from monthly recharge plans on a monthly basis.
- **Recharge Plan Comparison**: 
  - Compare recharge plan revenue across different locations.
  - Provide a comparative analysis of recharge plans before and after the 5G launch.

### Market Share Analysis
- **Market Share of Telecom Providers**: 
  - Analyze the market share of all telecom service providers.
- **Market Share Change**: 
  - Analyze the change in market share of all providers after the 5G launch.
- **Market Share Distribution**: 
  - Analyze market share distribution over different months and cities.

# Dashboard Overview

## KPI Comparative Report
![KPI Comparative Report](https://i.imgur.com/pgibRG7.gif)

- **Total Revenue**: ₹31.87 Billion
- **Average Revenue Per User (ARPU)**: ₹200.74
- **Total Active Users**: 161.72 Million
- **Total Users Lost**: 12.59 Million

**Key Insights:**
- **Revenue Change**: There was a 0.5% decline in revenue across all cities post-5G launch.
- **Top Cities by Revenue**: 
  - Mumbai, Delhi, Kolkata, Bangalore, Chennai (60% of total revenue).
  - Notable revenue declines in Delhi, Kolkata, and Chennai after 5G.
- **ARPU Trends**:
  - Overall ARPU increased by 11% after 5G.
  - Cities with significant ARPU growth: Raipur, Patna, Ahmedabad (20%+ increase).
  - Pune and Chennai experienced a decline in ARPU.
- **Active Users**:
  - There was an 8.28% decline in active users after the 5G launch.
  - Highest user losses in Ahmedabad, Delhi, Patna, Raipur, and Mumbai.
  - Cities with notable improvement in ARPU despite user losses: Raipur, Patna, Ahmedabad.
- **Unsubscribed Users**:
  - User loss increased by 10% after 5G launch.
  - Cities with highest user loss percentages: Lucknow, Pune, Jaipur, Chandigarh, Hyderabad.

## Recharge Plan Analysis
![Recharge Plan Analysis](https://i.imgur.com/XowXvef.gif)

- **Plan Changes**:
  - Discontinued: Plans 8, 9, 10.
  - Introduced: Plans 11, 12, 13.
- **Revenue Trends**:
  - Decline observed in Plans 4, 5, 6, 7.
  - Post-5G, revenue increased for most plans, with significant gains in Mumbai, Delhi, and Kolkata.
  - Bottom-performing cities: Raipur, Gurgaon, Chandigarh.
- **Recommendations**:
  - Focus on underperforming plans (4, 5, 6, 7) and newly introduced plans.
  - Consider promotional offers in Patna, Coimbatore, Chandigarh, Gurgaon, and Raipur.

## Market Share Analysis
![Market Share Analysis](https://i.imgur.com/45e5qTF.gif)

- **Market Share Leaders**:
  - Pico and Birtel are leading.
  - Atliqo ranks third with a market share ranging between 19-20%.
- **Market Share Trends**:
  - Atliqo’s market share dropped to 17.84% in September, from an average of 20.24% pre-5G.
  - Slight overall improvement in market share for competitors.
- **Top Cities for Market Share**:
  - Hyderabad, Delhi, Mumbai, Chandigarh, Gurgaon.


## Chart BY Chart 

Revenue Before 5G & After 5G 

![image](https://github.com/user-attachments/assets/660d4e95-ebc3-4ad1-84e1-d27fb3943625)

![image](https://github.com/user-attachments/assets/bbd92cf3-af7c-4fcf-8186-722af1b4379d)

After 5G Overall Revenue across all cities Dropped by 0.5% 
Mumbai , Delhi , Kolkata , Banglore & chennai are the top  5 cities by revenue and contribute 60% of the total revenue 
Amonng the top 5 cities delhi , koklata & chennai are showing decline in revenue after 5G launch 


ARPU Before 5G & After 5G 

![image](https://github.com/user-attachments/assets/d47dc5e0-dc0a-49b7-ab2a-d4ae980bb0ce)


![image](https://github.com/user-attachments/assets/64af0eab-325e-4add-85b0-f3b430b64b68)

After 5G ARPU  across all cities is increased by 11%.
Raipur, Patna & Ahmedabad has shown the improvement in ARPY by 20+% .
Pune & chennai are the only 2 cities where ARPU has shown negative trend .
Over the time period After 5G Launch ARPU has shown inmprovement as compare to last months.

Active Users Before 5G  & After 5G

![image](https://github.com/user-attachments/assets/f01ee136-2309-4bee-a92d-fcda1ec7631f)

![image](https://github.com/user-attachments/assets/fceb6f78-6b46-4ff3-97ed-c68c609a160f)

Overall there is a decline of monthly actve users by 8.28%
Mumabi , Kolkata , Delhi , Banglore & chennai are the top 5 cities with respect to monthly active users but at the same time Delhi  ,Mumbai , Banglore are lossing customers at high rate as well .
Ahemdabad , Delhi , Patna , Raipur & Mumbai are the top 5 citites which has lost the maximum users contrary to this  Raipur , patna & ahemdabad has shown improvement in ARPU.
Analysing the time period of before & after 5G , Monthky Active users after 5G launch is always less as compared to before 5G Launch time period .

Users Lost Before 5G & After 5G 

![image](https://github.com/user-attachments/assets/7ac0fe08-23e7-49b2-baf7-a00d8a91c681)

![image](https://github.com/user-attachments/assets/25620774-f680-4dd3-ada8-aedbefa6e7dc)

The Unsubscribed users count has been increased drastically after 5G launch which can led to negative publicity of our company we must look into it as early as possible
Overall there is 10% increase in user lost after 5G launch.
Lucknow , pune , Jaipur , CHandigarh ,Hyedarbas has user lost percentage more than 15%. this need to be address.



PLANS ANALYSIS 

Monthly Plan Revenue 

![image](https://github.com/user-attachments/assets/4fe32116-9c55-4bc9-b98b-e608b18a243b)


Plan Reveneue Before & After 5G By City 

![image](https://github.com/user-attachments/assets/5e50b905-f62e-4677-b02f-d0ea63de1db0)

Plan Revenue Before & After 5G Plans Wise

![image](https://github.com/user-attachments/assets/385bc698-48de-4eeb-9901-181cda01d0a3)

Plan 8, 9, and 10 have been discontinued and Plan 11, 12 and 13 have been introduced after 5G. We have observed that Plan 4, 5, 6, and 7 have experienced a declined revenue growth. So, we need to focus more on these plans along with the newly introduced plans to attract more active users. 
Apart from that, we could introduce modified attractive plans and roll out offers to increase the engagement for Patna, Coimbatore, Chandigarh, Gurgaon, and Raipur as these are the bottom 5 cities in terms of revenue generation.


Top 5 Plans 

![image](https://github.com/user-attachments/assets/7d468fc6-da4a-4b29-9367-8b2839499fc5)

Top 5 Cities By revenue 

![image](https://github.com/user-attachments/assets/170e56d2-4b67-4821-96af-9e33f47d9569)


MARKET SHARE ANALYSIS 

Market Share Distribution 

![image](https://github.com/user-attachments/assets/8b50da75-0e19-4a70-85c5-738665a5922b)


Market Share of all providers Before & After 5G

![image](https://github.com/user-attachments/assets/159ef4f4-85bd-4141-8ea7-96429d35cbcd)

Atliqo Market Share Analysis Over Months 

![image](https://github.com/user-attachments/assets/479c463d-b38f-42a9-9b9d-9e50246fc62e)












































# Telecom-Domain-Change-Analysis-
![image](https://github.com/user-attachments/assets/cb9066c2-4f10-4c87-94cb-d228cdb360fd)


Background 
AtliQo is one of the leading telecom providers in India and launched its 5G plans in May 2022 along with other telecom providers.

However, the management noticed a decline in their active users and revenue growth post 5G launch in May 2022. 

Atliqo’s business director requested their analytics team to provide a comparison report of KPIs between pre and post-periods of the 5G launch.

The management is keen to compare the performance between these periods and get insights that would enable them to make informed decisions


Objective 
The objective to to prepare a campartive report & dashboard showcasing the change in KPI After launch of  5G and the other insights assoicated with it .
Provide Insights & Area of opportunities such as cities which need immediate attention , plans which are not profitable , change in market size .

Data Overview 
we have provided 6 CSV files:
1. dim_cities
2. dim_date
3. dim_plan
4. fact_atliqo_metrics
5. fact_market_share
6. fact_plan_revenue



Column Description for dim_cities:
1. city_code: This column represents the unique code given for each city.
2. city_name: This column represents the name of the city corresponding to the city code.



Column Description for dim_date:
1. date: This column represents the starting date of each month. 
2. month_name: This column represents the month names in abbreviated form(Example: Jan, Feb, Mar, etc). We have months starting from January to September except for May.
3. before/after_5g: This column represents the unique category based on the month. We have 2 categories, Before 5G and After 5G. January to April comes represents the period before 5G implementation and June to September represents periods after 5G implementation.
4. time_period: This column represents the unique sequence number ranging from 1 to 4. These time Periods are used to make respective months comparisons before and after 5G implementation (Example: Jan vs Jun, Feb vs Jul, Mar vs Aug and Apr vs Sep)




Column Description for dim_plan:
1. plan: This column represents the various internet plans provided by the Atliqo company to the users. 
2. plan_description: This column represents the brief description about the internet plan.



Column Description for fact_atliqo_metrics:
1. date: This column represents the starting date of each month.
2. city_code: This column represents the unique pincode code given for each city.
3. company: This column represents the company name for which the data is provided. In this dataset it's only Atliqo. 
4. atliqo_revenue_crores: This column represents the revenue that Atliqo got on that particular month in that city_code in crores(unit of currency in India - 1Crore = 10 Million) from the internet users. 
5. arpu: This column represents the average revenue per user. That means on average how much revenue Atliqo generated on single user for a given time period.
6. active_users_lakhs: This column represents the number of active users who are using Atliqo's service on that particular month in that city_code in lakhs(unit of currency in India - 1 Lakh = 100,000).
7. unsubscribed_users_lakhs: This column represents the number of unsubscribed users who unsubscribed from Atliqo on that particular month in that city_code in lakhs(unit of currency in India - 1 Lakh = 100,000). 




Column Description for fact_market_share:
1. date: This column represents the starting date of each month.
2. city_code: This column represents the unique code given for each city.
3. tmv_city_crores: This column represents the total market value of the city in that month in crores(unit of currency in India) from the internet users. 
4. company: This column represents the different competitor names in the telecom industry [Atliqo, Britel, DADAFONE, PIO, Others].
5. ms_pct: This column represents the percentage of market share gained by respective company from the total market value(tmv_city) on that particular month in that city-code. 




Column Description for fact_plan_revenue:
1. date: This column represents the starting date of each month.
2. city_code: This column represents the unique code given for each city.
3. plans: This column represents the various internet plans provided by the Atliqo company to the users.
4. plan_revenue_crores: This column represents the revenue that Atliqo got from that respective plan on that particular month in that city_code in crores (unit of currency in India - 1Crore = 10 Million).


Metrics 
Total Revenue
Avg Revenue 
Average Revenue Per User
Total Active Users 
Total Unsubscribed Users
Monthly active users
Market Share %

We have prepared 3 reports covering Revenue & KPI Analysis with Respect to cities and Time period Comaprison Before 5G vs AFter 5G  , Plans Analysis and Market Shared Analysis

![image](https://github.com/user-attachments/assets/6d87a455-672c-41bb-99d1-7c840bd71d76)


Revenue Before 5G & After 5G 

![image](https://github.com/user-attachments/assets/660d4e95-ebc3-4ad1-84e1-d27fb3943625)

![image](https://github.com/user-attachments/assets/bbd92cf3-af7c-4fcf-8186-722af1b4379d)



ARPU Before 5G & After 5G 

![image](https://github.com/user-attachments/assets/d47dc5e0-dc0a-49b7-ab2a-d4ae980bb0ce)

![image](https://github.com/user-attachments/assets/64af0eab-325e-4add-85b0-f3b430b64b68)


Active Users Before 5G  & After 5G

![image](https://github.com/user-attachments/assets/f01ee136-2309-4bee-a92d-fcda1ec7631f)

![image](https://github.com/user-attachments/assets/fceb6f78-6b46-4ff3-97ed-c68c609a160f)


Users Lost Before 5G & After 5G 

![image](https://github.com/user-attachments/assets/7ac0fe08-23e7-49b2-baf7-a00d8a91c681)


![image](https://github.com/user-attachments/assets/25620774-f680-4dd3-ada8-aedbefa6e7dc)



PLANS ANALYSIS 

Monthly Plan Revenue 

![image](https://github.com/user-attachments/assets/4fe32116-9c55-4bc9-b98b-e608b18a243b)


Plan Reveneue Before & After 5G By City 

![image](https://github.com/user-attachments/assets/5e50b905-f62e-4677-b02f-d0ea63de1db0)

Plan Revenue Before & After 5G Plans Wise

![image](https://github.com/user-attachments/assets/385bc698-48de-4eeb-9901-181cda01d0a3)

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












































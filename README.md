## Airlines Data Analysis Project Using SQL and Python
### Overview
Welcome to the Airline Data Business Project! This repository is dedicated to addressing the critical issue of revenue loss in the airline industry by developing a robust business model using SQL and Python. Our primary objectives are to increase the Occupancy Rate, optimize the Pricing Strategy, and enhance Customer Experience.

The dataset utilized for this project has been sourced from Kaggle.com, providing a comprehensive foundation for our analysis. Through rigorous data analysis and modeling, we aim to uncover actionable insights that will help the airline industry navigate its current challenges and achieve sustainable growth.

### Table of Contents
>- Introduction
>- Business Problem
>- Objectives
>- Exploratory Data Analysis (EDA)
>- Findings
>- Conclusion

### Introduction

Airline Data Business by SQL and Python is a project aimed at addressing revenue loss challenges in the airline industry. Through a combination of SQL and Python, we aim to optimize key areas such as Occupancy Rate, Pricing Strategy, and Customer Experience to enhance overall business performance.

### Business Problem
The airline industry is grappling with several challenges, including:

>- Stricter environmental regulations leading to higher compliance costs.
>- Increased flight taxes and interest rates impacting operational costs.
>- Rising fuel prices contributing to higher overall expenses.
>- A tight labor market making it difficult to recruit and retain skilled personnel.
These factors collectively impact the profitability and sustainability of airline operations. This analysis aims to discover strategies for improving occupancy rates and increasing the average profit per seat.

### Objectives

**1.Boost Occupancy Rates:** Aim to enhance the occupancy rates on underperforming flights to elevate the average profit per seat and counteract the challenges we’re facing.

**2.Upgrade Pricing Strategy:** Develop a dynamic pricing approach that adapts to evolving market conditions and customer preferences to attract and retain more passengers.

**3.Elevate Customer Experience:** Focus on delivering a seamless and convenient journey for customers, from booking to arrival, to stand out in a competitive market and foster greater customer loyalty.

The ultimate goal is to identify and leverage opportunities to improve occupancy rates on flights with lower performance, which will contribute to increased overall profitability for the airline.


### Exploratory Data Analysis (EDA)

EDA using an SQLite3 database in your airline project, consider the following points:

**1.Connect to Database:** Use SQLite3 to connect and query the database for relevant tables and data.     
**2.Query Data:** Write SQL queries to extract data on occupancy rates, revenue, costs, and other metrics.   
**3.Generate Visualizations:** Use Python libraries like Matplotlib or Seaborn to create charts based on SQL query results.    
**4.Analyze Relationships:**    
>- **Correlation Analysis:** Use SQL to compute correlations between occupancy rates, revenue, and costs.   
>- **Identify Patterns:** Look for patterns or clusters in the data using SQL GROUP BY and aggregate functions.

### Findings
The primary objective of this project is to leverage SQL to uncover opportunities for increasing the occupancy rate on
flights that are currently underperforming. By focusing on these low-performing flights, we aim to identify and
implement strategies that can significantly enhance their occupancy rates.

**Tables for Flight Analysis**
![image](https://github.com/user-attachments/assets/e920978f-13f3-42ac-aa32-d23c8dc1e0c3)
The aircrafts_data and airports_data tables provide essential information about the aircraft fleet and
airport locations, which are crucial for understanding flight logistics and capacity. The flights, bookings,
and tickets tables offer insights into flight schedules, passenger bookings, and ticket details, enabling the
analysis of occupancy rates and revenue generation. Meanwhile, the seats, boarding_passes, and
ticket_flights tables help track seat allocation and boarding processes, ensuring efficient seat utilization
and customer experience management.

### **Basic Analysis¶**
**How many planes have more than 100 seats?**

The detailed analysis of data provides insights into the number of planes with more than 100 seats,
how the number of tickets booked and the total amount earned changed over time, and the average
fare for each aircraft with different fare conditions. These findings will be useful in developing strategies
to increase occupancy rates and optimize pricing for each aircraft. Table 1 shows the aircraft with more
than 100 seats and the actual seats count.

![image](https://github.com/user-attachments/assets/b3a7fe9d-5114-44fb-8590-62ba91aab6ac)
![image](https://github.com/user-attachments/assets/6c61b220-101c-4e10-a35b-f29193a6add1)
![image](https://github.com/user-attachments/assets/1ab2758f-216e-46d3-adea-a42f544c5a41)

**How the number of tickets booking and total amount earned changed with the time.**

To gain a more comprehensive insight into the trend of ticket bookings and the revenue generated from those
bookings, we employed a line chart visualization. Analyzing the chart reveals that the number of tickets
booked shows a gradual upward trend from June 22nd to July 7th, followed by a relatively stable pattern from
July 8th through August, with a significant peak in ticket bookings where the highest number of tickets was
booked on a single day. It is crucial to note that the revenue generated by the company from these bookings
closely mirrors the number of tickets booked. Consequently, we observe a similar pattern in the total revenue
earned by the company over the analyzed period.
findings suggest that further exploration of the factors contributing to the peak in ticket bookings may be beneficial
for increasing overall revenue and optimizing operational strategies.

![image](https://github.com/user-attachments/assets/10876e3c-a7de-40a1-b96d-b5fa2c7013fd)

![image](https://github.com/user-attachments/assets/fd158864-8577-4525-8257-f9eb10b13c67)

![image](https://github.com/user-attachments/assets/e1dac6a8-7219-48d0-89ff-a262c38e40c0)
![image](https://github.com/user-attachments/assets/892f66cd-030f-4c4c-9a2a-d589d92f56d5)

**Calculate the average charges for each aircraft with different fare conditions.**

The bar chart highlights the average amount spent across various aircraft codes, segmented by fare
conditions—Business, Economy, and Comfort. Business class consistently shows the highest
average expenditure, notably exceeding 100,000 units for aircraft code 319. In contrast, Economy
class expenditures are significantly lower across all aircraft codes. Comfort class data, available
only for aircraft code 773, indicates moderate spending between Business and Economy classes.
This visualization emphasizes the high revenue potential of Business class, suggesting targeted
strategies to enhance premium service offerings. These insights can inform pricing models and
marketing efforts, aiming to improve occupancy rates and maximize average profit per seat, thereby
boosting the airline's financial performance.

![image](https://github.com/user-attachments/assets/c1ad2e28-6c84-480b-937a-02c83dddfc54)
![image](https://github.com/user-attachments/assets/a1f12e02-bbc8-4d45-abdc-3ab43d62a574)

### **Analyzing occupancy rate**
**For each aircraft calculate the total revenue per year and the average revenue per ticket.**

Analyzing occupancy rate Airlines must thoroughly analyze their revenue streams in order to maximize profitability. The overall
income per year and average revenue per ticket for each aircraft are important metrics to consider. Aircraft code SU9 stands out
as the top performer, generating an impressive total revenue of approximately $5.11 billion from 365,698 tickets, with an average
revenue of around $13.99k per ticket. Close behind is aircraft code 319, which, despite handling fewer tickets (52,853), achieves
a remarkable total revenue of roughly $2.71 billion and boasts the highest average revenue per ticket at about $51.20k. Another
notable player is aircraft code 763, which records a substantial total revenue of about $4.37 billion from 124,774 tickets, with an
average revenue per ticket of $35.03k. On the other hand, smaller aircraft like CN1 and CR2 contribute more modest revenues,
with totals around $96.37 million and $1.98 billion, respectively, and average revenues per ticket of $6.57k and $13.21k. Aircraft
codes 321, 733, and 773 show moderate revenue performance, ranging from approximately $1.43 billion to $3.43 billion in total
revenue and average ticket revenues between $15.29k and $23.77k. 

This revenue analysis highlights the substantial financial contributions of larger aircraft, particularly
those with higher ticket volumes and elevated average ticket prices. Understanding these revenue
patterns can inform strategic decisions aimed at optimizing fleet utilization, enhancing profitability,
and targeting specific aircraft types for revenue maximization.

![image](https://github.com/user-attachments/assets/af5e8f09-288d-4474-80e6-ef89649cdf47)

![image](https://github.com/user-attachments/assets/c40212f4-9eab-4d74-a942-a7c43c918eac)

**Calculate the average occupancy per aircraft.**

In evaluating the performance of various aircraft types, the analysis of occupancy rates reveals significant variations.
Aircraft code 773 exhibits the highest occupancy rate at approximately 65.90%, indicating a strong utilization of its
seating capacity. Following closely, aircraft code 733 has an occupancy rate of about 61.74%, reflecting a high
efficiency in seat usage. Aircraft code 763 shows a solid occupancy rate of 51.32%, while aircraft code 319, with an
occupancy rate of 46.19%, demonstrates lower utilization compared to the top performers.
Conversely, smaller aircraft such as CN1 and CR2 have occupancy rates of 50.04% and 42.97%, respectively. Although
these rates are lower, they still suggest a moderate level of seat usage relative to their capacity. Aircraft code SU9, with
an occupancy rate of 58.57%, falls in between the higher and lower performing aircraft.
Integrating this occupancy data with revenue performance, aircraft code 773 stands out not only for its high occupancy
rate but also for generating approximately $3.43 billion in total revenue, underscoring its significant financial
contribution. Aircraft code 763, with its occupancy rate of 51.32%, also generates a substantial revenue of around
$4.37 billion. Aircraft code SU9, despite a lower occupancy rate compared to the highest performers, contributes
approximately $5.11 billion in total revenue, indicating that while it may have a lower occupancy rate, its overall
revenue generation remains exceptional.

In contrast, aircraft with lower occupancy rates, such as aircraft code 319 and 321, still contribute considerable revenues—
around $2.71 billion and $1.43 billion, respectively—suggesting that high average revenue per ticket can offset lower
occupancy.
This analysis highlights the importance of balancing occupancy rates with revenue generation. Aircraft with high occupancy
rates and high revenue per ticket, like aircraft code 773, tend to be the most profitable. However, even aircraft with lower
occupancy rates can achieve substantial revenues if they maintain high average revenue per ticket. These insights are crucial
for optimizing fleet operations and enhancing overall profitability.

![image](https://github.com/user-attachments/assets/172c0116-0125-4b38-a65d-ac5fafb29731)
![image](https://github.com/user-attachments/assets/c1aa5c55-a9bc-435b-9491-2bd1d61a61de)
![image](https://github.com/user-attachments/assets/e1188bcd-ce11-4d94-9f34-ae35565348f4)

**Calculate by how much the total annual turnover could increase by giving all aircraft a 10% higher occupancy rate.**

Increasing the occupancy rate of each aircraft by 10% could significantly boost total annual revenue. For instance, aircraft code
SU9, currently generating approximately $5.11 billion, would see an increase of about $5.63 billion if its occupancy rate were
improved. Similarly, aircraft code 763, with a current revenue of $4.37 billion, could experience an additional revenue of around
$4.81 billion with the increased occupancy. Aircraft code 773, generating $3.43 billion, could see its revenue rise to about $3.77
billion.
Aircraft code 319’s revenue could increase by approximately $2.98 billion, reaching around $2.71 billion from its current figure.
Aircraft code 321 could experience an increase of about $1.80 billion, reaching approximately $1.43 billion. Smaller aircraftlike
CN1 and CR2 would also see revenue boosts, with CN1’s revenue potentially rising to around $106 million and CR2’s by
approximately $2.18 billion.
Overall, a 10% increase in occupancy rates across all aircraft could result in a substantial uplift in total revenue, highlighting the
significant impact of improved seat utilization on financial performance.

![image](https://github.com/user-attachments/assets/83d2839b-bd15-4db7-9f89-3ce650ce7b44)

![image](https://github.com/user-attachments/assets/227515c3-a575-434f-a01c-02681d6187fa)

### **Conclusion**

In the airline industry, analyzing key revenue indicators like total revenue per year, average revenue per
ticket, and average occupancy per aircraft is essential for enhancing profitability. By evaluating these
metrics, airlines can pinpoint areas for improvement and refine their pricing and route strategies. A
critical factor in boosting profitability is increasing occupancy rates, which enables airlines to optimize
revenue and reduce the costs associated with empty seats. To address pricing challenges, airlines
should adjust fares to reflect the condition and amenities of each aircraft, ensuring that prices are
neither too high nor too low to attract passengers effectively.
However, improving occupancy rates should not compromise customer satisfaction or safety.
Maintaining a balance between profitability and high-quality service is crucial. Airlines may achieve longterm success in a highly competitive business by adopting a data-driven revenue analysis and
optimization strategy.

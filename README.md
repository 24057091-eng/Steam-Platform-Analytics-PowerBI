# Steam-Platform-Analytics-PowerBI
End-to-End Data Analytics Project using Power BI and Python.
Added Project Documentation (Report) and Python Data Cleaning Script
Project Documentation: Steam Platform Analytics

Name: Wasim Ahmad Khan

 Roll Number: 24057091

Batch/Program: B.Tech Computer Science and Engineering (2024-2027)

1. Title
Steam Platform Analytics Dashboard: Insights & Trends

Problem Statement: 
Streamlining Market Intelligence for PC Gaming 
In the PC gaming industry, thousands of games are released annually on the Steam platform, making it difficult for developers and publishers to understand market trends. Raw transactional data remains fragmented, preventing management from identifying key operational inefficiencies. This project addresses three major bottlenecks: 
Genre Saturation and Revenue: It is difficult to identify which genres (Action, Indie, RPG, etc.) are dominating the market and driving player interest. 
Pricing vs. Engagement: Without granular tools, it is challenging to understand the correlation between a game's price and its actual user engagement (Positive Ratings). 
Historical Trends: The lack of centralized year-over-year game release data makes it difficult to forecast future competition and market density.
																						








Project Goal: 

The objective of this project is to engineer a unified, interactive Business Intelligence (BI) dashboard that transforms the raw Steam dataset (over 27,000 games) from Kaggle into a strategic decision-making tool. This enables stakeholders to refine pricing strategies and allocate resources according to actual market preferences.


Data Engineering Methodology (Tech stack)
Data Import & Connectivity: The steam.csv dataset from Kaggle was ingested into Power BI. "Data Type" validation was performed—for example, ensuring the "release_date" column was recognized as a Date format to enable the time-series analysis for yearly trends. 
Initial data cleaning, including missing value imputation and text standardization, was performed using a Python script (Pandas library) before importing the dataset into Power BI.

Data Transformation (Power Query): 
Column Standardizing: The platforms column (which contained grouped text like "windows;mac;linux") and genres column were parsed and cleaned to maintain accuracy in visual representations.
•	Data Cleaning: Handled duplicates and ensured null values were accounted for so that aggregations like Total Games and Average Price remained mathematically accurate.
Custom Attribute Creation (DAX): Created optimized DAX measures for high-level metrics such as "Total Publishers", "Average Price", and "Total Positive Ratings" to provide instant insights on the KPI cards.








Comprehensive Feature Analysis (The "Deep Dive")
Solution & Features
This section describes the functionality built in Power BI, utilizing a structured two-page architecture:

1.	Centralized Command Center (Page 1 - Overview): Developed a high-impact header featuring four real-time KPI cards: Total Publishers, Total Developers, Average Price, and Total Positive Ratings. This provides an instant health check of the platform's scale.

2.	Temporal Trend Analysis: Integrated a line chart to track 'Games Released by Year', enabling stakeholders to identify the explosive growth of game releases over time.

3.	Categorical Market Breakdown: Engineered a clustered bar chart ('Total Games by Genre') to visualize market preferences, alongside a donut chart for OS support distribution highlighting platform dominance.

4.	Deep Dive Analytics (Page 2): Designed a dedicated secondary page featuring a highly detailed Matrix/Table to inspect individual game metrics. Additionally, a scatter plot was integrated to map the relationship between game prices and engagement.

5.	Interactive Navigation: Implemented custom "Action Buttons" to allow users to seamlessly switch between the 'Overview' and 'Deep Dive' pages, ensuring a smooth UI/UX flow.

VISUAL REPRESENTATION


 
<img width="790" height="418" alt="image" src="https://github.com/user-attachments/assets/3c9be0e3-188e-4953-9a0e-e1e29d4060de" />




 
TOOLTIP-1


			
 <img width="619" height="464" alt="image" src="https://github.com/user-attachments/assets/5aab17bd-5054-4e17-bf8d-a5316a9cdfc5" />





<img width="1242" height="661" alt="image" src="https://github.com/user-attachments/assets/e7424493-f4ee-4f7c-a241-19bb7cd2f8dc" />




<img width="570" height="426" alt="image" src="https://github.com/user-attachments/assets/c02e5471-2848-497d-b44f-4a4f0c5f06f7" />


 
TOOLTIP-2










Unique Points of the Project
This section highlights why  Power BI work is superior to a basic report.
	Two-Page Master/Detail Architecture: Instead of cramming all visuals onto a single canvas, I engineered a sophisticated two-page layout. This keeps the Overview page clean while allowing users to drill down into granular data on the Deep Dive page when necessary.
	Diagnostic Engagement Modeling: The 'Price vs. Positive Ratings' scatter plot is not just for show; it is a diagnostic tool. By plotting these variables against each other, the dashboard automatically identifies "Overpriced" games with low engagement, or "Highly Engaged" budget titles.
	Advanced Custom Report Page Tooltips: Instead of standard black-box text tooltips, I utilized Custom Report Page Tooltips. When a user hovers over a data point, an entirely new micro-visual (such as a detailed breakdown of Price and Ratings) pops up dynamically, showcasing advanced Power BI capabilities.

Future Improvements & Scalability
Transition to Live Data Architecture: Currently, the project uses a static Kaggle CSV dataset. A future enhancement is to establish a live connection to the Steam Web API to refresh the dashboard with real-time game releases and active player counts.
Machine Learning (Sentiment Analysis): The next phase could involve integrating Python to perform Natural Language Processing (NLP) on user reviews. By analyzing review text, we can plot a "Sentiment Score" to understand the core reasons driving the Positive Ratings.
Automated Anomaly Detection: By utilizing Power BI's AI features, automated alerts can be set up to notify publishers if competition in a specific genre spikes suddenly, or if user ratings drop below a critical threshold.											




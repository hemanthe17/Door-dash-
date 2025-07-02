Project Overview:
A strategic initiative to enhance decision-making in DoorDash's food delivery operations using data analytics.
Aims to analyze datasets on customer orders, delivery operations, and partner interactions.
Goals include identifying growth opportunities, optimizing delivery routes and times, and improving overall customer satisfaction.
Insights will inform strategies to meet customer needs, improve engagement, and enhance delivery efficiency.
Key Users of the Analysis:
Business Strategy Team (long-term planning).
Marketing Department (campaign planning and execution).
Sales Managers (new restaurant partner acquisition).
Operational Heads (daily delivery logistics).
Executives (broader strategic initiatives and decisions).
Data Sources:
Customer Transactions: Detailed order data including purchase amounts, order times, frequency, and preferences.
Operational Data: Information on delivery costs, time metrics, and efficiency.
Feedback and Surveys: Direct feedback from customers and restaurant partners for qualitative insights.
Data Linking and Transformation Plan:
Linking Data: Utilizing unique identifiers like Restaurant IDs to merge datasets for a cohesive data model within the BI tool.
Data Transformation Needs:
Normalizing date formats and currency.
Categorizing unstructured feedback.
Aggregating data points for reports and dashboards.
Key Measures Created (DAX Formulas):
Average Cost for Well-Reviewed = CALCULATE(AVERAGE('Data Table'[Average_Cost($)]),'Data Table'[Reviews] > 50) 
Average Minimum Order = AVERAGE('Data Table'[Minimum_Order($)]) 
Total Average Sales = SUM('Data Table'[Average_Cost($)]) 
Total Delivery Time = SUM('Data Table'[Delivery_Time_in_minutes]) 
Total Orders = COUNTROWS('Data Table') 
Valid Ratings Count = COUNTROWS(FILTER('Data Table', 'Data Table'[Rating Validity] = "Valid Rating")) 
Team Member Responsibilities:
Harshitha Nayana & Bhavana Samineni: Data cleaning, transformation, visual design, and report creation.
Hemanth Ediga: DAX application and R Integration for visualizations preparation
Nehitha Reddy Aramati: Final presentation review (layout, font size).
Sai Charan Konanki: Providing key metrics and report summary.
Dashboard Visualizations and Insights:
Cost and Order Value Comparison by Location: Bar chart comparing average minimum order value against average cost per order by city, used to identify locations with high order values and assess minimum order impact.
Average Delivery Time Insight: Numerical display showing overall delivery efficiency, crucial for customer satisfaction and identifying areas for logistical improvement.
Filter for Rating Validity: Interactive checkboxes to segment valid and invalid customer feedback, ensuring insights are based on authentic experiences.
Review Count and Rating Correlation: Dual-axis chart analyzing the relationship between review volume and average rating per restaurant, useful for understanding brand reputation and pinpointing improvement areas.
Restaurant Popularity and Engagement by Location: Bar chart and table showing restaurant count, reviews, and votes by location, guiding expansion strategies and targeted promotions.
Overall Dashboard Value:
Provides a multi-faceted view of the business's operational health.
Guides investment decisions, operational tweaks, and customer relationship management.
Highlights strengths and areas for improvement, ensuring effective resource allocation for customer satisfaction and revenue maximization.

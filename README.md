# OLA-DA-POJECT

🛠️ Project Summary
This project uses a simulated dataset of Ola bookings to analyze key performance metrics and identify trends. The dataset, created using a ChatGPT prompt, includes columns such as Booking_Status, Vehicle_Type, Booking_Value, and Payment_Method. By performing data analysis, we can gain a better understanding of customer and driver behavior, revenue streams, and operational efficiency. The project is structured to answer specific business questions using both SQL and Power BI.

📊 Power BI Dashboard Highlights
The project's Power BI dashboard is designed to provide a comprehensive, interactive view of the business data. It is divided into several sections, each focusing on a different aspect of the business operations.

Overall
This section provides a high-level overview of the total number of bookings and their success rates.

Total Bookings: 103,024

Total Booking Value: 35M

Booking Status Breakdown: A pie chart shows the proportion of different booking statuses, with 62.05% of rides being successful. Other statuses include canceled by driver (9.83%), canceled by customer (17.89%), and driver not found (10.19%).

Ride Volume Over Time: A line graph shows booking counts over the one-month period, revealing daily fluctuations.

Vehicle Type
This view provides a breakdown of performance by vehicle type.

Average Ride Distance: The average ride distance is around 25 km for most vehicle types, except for Auto, which has an average distance of 10.04 km.

Total Booking Value: Prime Sedan and Prime Plus have the highest total booking values at 8.30M and 8.05M, respectively.

Driver and Customer Ratings: Ratings are generally high across all vehicle types, averaging around 4.00.

Revenue
This section focuses on financial performance and payment methods.

Revenue by Payment Method: The bar chart shows that Cash is the most preferred payment method, generating the highest revenue. UPI is the second-most popular, followed by Credit Card and Debit Card.

Top 5 Customers: The top five customers by total booking value are identified, with CID308763 and CID355074 being the highest-spending customers.

Cancellation
This view provides insights into ride cancellations, categorized by the party responsible.

Total Canceled Bookings: A total of 28,933 bookings were canceled.

Reasons for Cancellation:

Customer Cancellations: The primary reason for customer cancellations is the driver not moving toward the pickup location (30.24%). Other reasons include the driver asking to cancel, wrong addresses, or a change of plans.

Driver Cancellations: The most common reason for driver cancellations is personal and car-related issues (35.49%).

💻 SQL Analysis
The project includes a series of SQL queries to extract specific data points and support the Power BI visualizations. Here are a few examples:


Average Ride Distance: SELECT Vehicle_Type, AVG(Ride_Distance) FROM bookings GROUP BY Vehicle_Type; 


Total Successful Bookings: SELECT SUM(Booking_Value) FROM bookings WHERE Booking_Status = 'Success'; 



Top 5 Customers: SELECT Customer_ID, COUNT(Booking_ID) FROM bookings GROUP BY Customer_ID ORDER BY total_rides DESC LIMIT 5;


Snap Shots of Dashboards -- 
https://github.com/AYU3117/OLA-DA-POJECT/blob/main/Snapshots%201.png
https://github.com/AYU3117/OLA-DA-POJECT/blob/main/Snapshots%202.png
https://github.com/AYU3117/OLA-DA-POJECT/blob/main/Snapshots%203.png
https://github.com/AYU3117/OLA-DA-POJECT/blob/main/Snapshots%20%204.png
https://github.com/AYU3117/OLA-DA-POJECT/blob/main/Snapshots%205.png

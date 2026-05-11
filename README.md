# Uber Demand-Supply Gap Analysis

## Project Overview
This project analyzes Uber trip data to identify and visualize the demand-supply gap across different pickup points (City vs. Airport) and times of the day. The goal is to understand patterns of trip completion, cancellations, and instances of 'No Cars Available' to provide insights into operational efficiencies and areas for improvement.

## Data Source
The analysis is based on `uber-data (8).csv`, which contains details such as request ID, pickup point, driver ID, status, and request/drop timestamps.

## Analysis Performed
1.  **Data Preprocessing**: Converted 'Request timestamp' to datetime objects and extracted the hour of the day.
2.  **Time Slot Categorization**: Categorized hours into 'dawn', 'early morning', 'noon', 'late evening', and 'night' to analyze demand patterns.
3.  **Overall Cab Availability**: Calculated and visualized the distribution of 'Cab Available' vs. 'Cab Not Available' trips.
4.  **Trip Status Distribution**: Visualized the overall distribution of 'Trip Completed', 'Cancelled', and 'No Cars Available' statuses.
5.  **Requests by Hour**: Plotted the number of requests throughout the day to identify peak hours.
6.  **Status by Pickup Point**: Analyzed and visualized trip status distribution for 'Airport' and 'City' pickup points separately.
7.  **Hourly Status Distribution**: Detailed analysis of trip status distribution by hour for both overall data and separately for 'City' and 'Airport' pickups.

## Key Findings
1. Overall Trip Status Distribution by Hour of Day:

-Morning Rush (around 5 AM to 9 AM): There's a significant peak in 'Cancelled' requests, especially from 6 AM to 9 AM. This suggests high demand during these hours, but also a large number of cancellations, possibly due to drivers canceling or high surge pricing.
-Evening Peak (around 5 PM to 9 PM): The 'No Cars Available' segment sees a substantial increase during these hours. This indicates that while there is high demand, there aren't enough drivers to meet it, leading to many requests going unfulfilled.

2. Trip Status Distribution by Hour of Day for City Pickup:

-Morning Rush (around 5 AM to 9 AM): Requests originating from the City show a very high proportion of 'Cancelled' trips during these hours. This suggests that city drivers might be less willing to take rides towards the airport, or that demand within the city itself during peak hours is hard to meet.

3. Trip Status Distribution by Hour of Day for Airport Pickup:

-Evening Peak (around 5 PM to 10 PM): Requests from the Airport prominently show a high number of 'No Cars Available' during these hours. This leading to a large number of passengers being stranded or having long wait times. This is likely due to drivers not wanting to make a trip from the city in the morning towards airport, and then return empty.

## Recommended solutions
1. Give extra bonuses for airport rides.
2. Company can collaborate with airports for pre-booked rides.
3. The app can group passengers going in the same direction.

## Technologies Used
-   Python
-   Pandas (for data manipulation)
-   Matplotlib (for plotting)
-   Seaborn (for enhanced visualizations)

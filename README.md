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
-   Identified peak demand hours and corresponding supply challenges (cancellations or no cars available).
-   Revealed differences in demand-supply dynamics between City and Airport pickup locations.
-   Visualizations clearly show time slots where demand significantly outstrips supply, or where cancellations are high.

## Technologies Used
-   Python
-   Pandas (for data manipulation)
-   Matplotlib (for plotting)
-   Seaborn (for enhanced visualizations)

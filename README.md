# Hospitality-Industry

Hospitality Industry Power BI Report
# Overview
This Power BI report provides a detailed analysis of the hospitality industry for the months of May, June, and July 2022. The report focuses on key performance metrics such as RevPAR, ADR, revenue, occupancy, and more. It leverages five CSV files to offer insights into the performance of hotels and their rooms, including booking trends, cancellations, and guest satisfaction.

# Key Metrics
The report tracks several key metrics to provide a comprehensive view of the industry's performance:

RevPAR (Revenue per Available Room) and its WoW% (Week-over-Week percentage change)
ADR (Average Daily Rate) and its WoW%
Revenue and its WoW%
Total Bookings
Total Capacity
Occupancy Percentage
Average Rating
Number of Days
Total Cancelled Bookings
Cancellation Percentage
Total Checked Out
No Show Bookings
No Show Rate Percentage
Booking Percentage by Platform
Booking Percentage by Room Class
Realisation Percentage and its WoW%
DBRN (Day Before Realised Night) and its WoW%
DSRN (Day Same Realised Night) and its WoW%
DURN (Day Utilized Realised Night) and its WoW%

# Data Files
The analysis is based on data from the following CSV files:

dim_date
dim_hotels
dim_rooms
fact_aggregated_bookings
fact_bookings

# Column Descriptions

dim_date
date: Represents dates in May, June, and July.
mmm yy: Date formatted as monthname year (e.g., May 22).
week no: Unique week number for each date.
day_type: Indicates if the day is a Weekend or Weekday.

dim_hotels
property_id: Unique ID for each hotel.
property_name: Name of each hotel.
category: Class of the hotel (Luxury, Business).
city: Location of the hotel.

dim_rooms
room_id: Type of room (RT1, RT2, RT3, RT4).
room_class: Class of the room (Standard, Elite, Premium, Presidential).

fact_aggregated_bookings
property_id: Unique ID for each hotel.
check_in_date: Check-in dates of customers.
room_category: Type of room (RT1, RT2, RT3, RT4).
successful_bookings: Number of successful room bookings for a particular room type in the hotel on that date.
capacity: Maximum count of rooms available for a particular room type in the hotel on that date.

fact_bookings
booking_id: Unique Booking ID for each customer.
property_id: Unique ID for each hotel.
booking_date: Date the customer booked their room.
check_in_date: Date the customer checked in.
check_out_date: Date the customer checked out.
no_guests: Number of guests who stayed in the room.
room_category: Type of room (RT1, RT2, RT3, RT4).
booking_platform: Platform through which the room was booked.
ratings_given: Ratings given by the customer.
booking_status: Status of the booking (Cancelled, Checked Out, No Show).
revenue_generated: Amount of money generated from the booking.
revenue_realized: Final amount received by the hotel after adjustments for cancellations or no shows.

# Usage
This report can be used by hotel management to:

Monitor key performance metrics over time.
Analyze booking patterns and trends.
Identify areas for improvement in service and capacity management.
Understand customer behavior and preferences.
Make data-driven decisions to enhance profitability and customer satisfaction.

# Conclusion
This Power BI report provides an in-depth analysis of the hospitality industry for May, June, and July 2022, using comprehensive data from multiple sources. It offers valuable insights into the performance of hotels, aiding in strategic decision-making and operational improvements.

For further details or to explore the data, please refer to the included CSV files and the corresponding Power BI dashboards

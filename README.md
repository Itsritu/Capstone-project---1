# Capstone-project--1--Hotel Booking Analysis(EDA)
# Objective
We are provided a csv file that contains the record of hotels.

Our main objective is perform EDA on the given dataset and draw useful conclusions about general trends in hotel bookings and how factors governing hotel bookings interact with each other.
# Dataset

1) There are 119390 rows.

2) There are 32 columns in our dataset.
# Description of columns:
hotel : Name of the hotel (Resort Hotel or City Hotel)

is_canceled : If the booking was canceled(1) or not (0)

lead_time : Number of days before the actual arrival of the guests

arrival_date_year : Year of arrival date

arrival_date_month : Month of arrival date

arrival_date_week_number : Week number of year for arrival date

arrival_date_dat_of_month : Day of arrival date

stays_in_weekend_nights : Number of weekend nights(Saturday or Sunday) spent at the hotel by the guests

stays_in_week_nights : Number of weeknights(Monday to Friday) spent at the hotel by the guests

adults : Number of adults among guests

children : Number of children among guests

babies : Number of babies among guests

meal : Type of meal booked by the guests

country : Country of guests

market_segment : Designation of market segment, guests belong to which segment

distribution_channel : How the customer accessed the stay by corporate booking/Direct/TA.TO

is_repeated_guest : If the booking was from repeated guest(1) or not(0)

previous_cancellations : Number of previous bookings that were cancelled by the customer

previous_booking_not_canceled : Number of previous bookings not cancelled by the customers

reserved_room_type : Type of room type reserved by the customers

assigned_room_type : Type of room type assigned

booking_changes : Number of changes made to the booking

deposit_type : Type of deposit made by the guests

agent : ID of travel agent who made the booking

company : ID of the company that made the booking

days_in_waiting_list : Number of days the booking was in waiting list

customer_type : Type of customer

adr : Average daily rate

required_car_parking_spaces : Number of car parking spaces required by the customer

total_of_special_requests : Number of special request made by customer

reservation_status : Reservation-status(canceled,check_out or no show)

reservation_status_date : Date at which the last reservation status was updated

# Data Cleaning

# (1) Removing Duplicate rows

All duplicate rows were dropped.

# (2) Handling null values

company column contains the higher number of null values so, we dropped this column ftom the dataset.

Null values in column agent were replaced by 0.

Null values in column country were replaced by 'others'.

Null values in column children were replaced by 0.

# (3) Converting columns to appropriate data types

Changed data type of children, company, agent to int type.

# (4) Removing outliers

One outlier was found in the adr column. Simply dropped it.

# (5) Creating new columns

Created new column total_stays_nights by adding stays_in_weekend_nights+stays_in_week_nights.

Created new column total_guest by adding adults+children+babies.

# Charts used for visualization
Mainly performed using Matplotlib and Seaborn library and the following graph and plots had been used:

Bar Plot.

Pie Chart.

Line Plot.

Heatmap.

Horizontal Bar plot

Pairplot

# Challenges
(1) There was a lot of duplicate data.

(2) Data was present in wrong datatype format.

(3) Choosing appropriate visualization techniques to use was difficult.

(4) A lot of null values were there in the dataset.


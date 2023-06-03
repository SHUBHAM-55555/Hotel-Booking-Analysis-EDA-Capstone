**Hotel Booking Analysis EDA**

Have you ever wondered when the best time of year to book a hotel room is? Or the optimal length of stay in order to get the best daily rate? What if you wanted to predict whether or not a hotel was likely to receive a disproportionately high number of special requests? This hotel booking dataset can help you explore those questions!
This data set contains booking information for a city hotel and a resort hotel, and includes information such as when the booking was made, length of stay, the number of adults, children, and/or babies, and the number of available parking spaces, among other things. All personally identifying information has been removed from the data.
Explore and analyze the data to discover important factors that govern the bookings.

**Objective**

**We are provided with a hotel bookings datase**t.


The first and formost objective for every business is that to make it stable to survive in the market for long run, growth will be the secondary parameter, it will grow definetly with time and efforts but the important aspect of every business is revenue through their services that they are offering to servive for long run. To analyse the data and to figure out the insights to sucess factors is the main objective of every business


Our main objective is perform EDA on the given dataset and draw useful conclusions about general trends in hotel bookings and how factors governing hotel bookings interact with each other.

Hotel Bookings Exploratory Data Analysis




**Dataset:-**

We are given a hotel bookings dataset. This dataset contains booking information for a city hotel and a resort hotel. It contains the following features.

1.**hotel** = Hotel type( resort hotel or city hotel)

2.**is_canceled** = if the booking was cancelled if yes (1) or not (0)

3.**lead_time** = Number of Days before the actual arrival of guests

4.**arrival_date_year** = year of arrival

5.**arrival_date_month** = month of arrival

6.**arrival_date_week_number** = week number in which week guest arrived

7.**arrival_date_day_of_month** = Day of arrival from month

8.**stays_in_weekend_nights** =Number of Days spent on saturday and Sunday

9.**stays_in_week_nights** = Number of days spent on weekdays

10.**adults** =No. of Adults

11.**children** = No. of Children

12.**babies** = No. of Babies

13.**meal** = Type of Food ordered

14.**country** = Guests belongs to

15.**market_segment** = Designation of market segment

16.**distribution_channel** = Name of Booking Distribution Channel

17.**is_repeated_guest** = If the booking was from repeated Guest (1) or not (0)

18.**previous_cancellations** = Number of previous bookings cancelled by the customer prior to the current booking

19.**previous_bookings_not_canceled** = Number of previous bookings not cancelled by the customer prior to the current booking

20.**reserved_room_type** = Code of room type reserved

21.**assigned_room_type** = Code of room type assigned

22.**booking_changes** = Changes in booking made by the customer

23.**deposit_type** = Type of Deposit

24.**agent** = ID of the travel agent who made the booking

25.**company** = Company through the booking was made

26.**days_in_waiting_list** = Number of days the booking was in the waiting list

27.**customer_type** = Type of customer

28.**adr** = Average Daily Rate

29.**required_car_parking_spaces** = Number of Car parking required

30.**total_of_special_requests** = Number of special request made by the customer

31.**reservation_status** = Reservation Status(Canceled, Check-out, No-show

32.**reservation_status_date** =Date on which the reservation status was updated

Total number of rows in data: 119390

Total number of columns: 32


**Data Cleaning and Feature Engineering**


(1) Removing Duplicate rows, all duplicate rows were dropped.

(2) Handling null values
Null values in columns company and agent were droped.
Null values in column country were replaced by 'others'.
Null values in column children were replaced by "0".

(3) Converting columns to appropriate data types
Changed data type of children, company, agent to int type.


(4) Creating new columns
Created new column total_stay by adding stays_in_weekend_nights+stays_in_week_nights.
Created new column total_people by adding adults+children+babies.
Exploratory Data Analysis

 

**Mainly performed using Matplotlib and Seaborn library and the following graph and plots had been used:**

Bar Plot.

Histogram.

Scatter Plot.

Pie Chart.

Line Plot.

Heatmap.

Box Plot




**Observations:- **
 
 1.) Most demanded room type is A, but better adr generating rooms H, G and C. Hotels should increase the no. of room types A and H to maximise revenue.
 
 2.) Around 60% bookings are for City hotel and 40% bookings are for Resort hotel, therefore City Hotel is busier than Resort hotel.
 
 3.) Guests use different channels for making bookings out of which most preferred way is TA/TO.
 
 4.) July- August are the most busier and profitable months for both of hotels. 
 
 5.) Most of the guests came from european countries, with highest number of guests from Portugal.
 
 6.) Most common stay length is less than 4 days and generally people prefer City hotel for short stay, but for long stays, Resort Hotel is preferred.
 
 
 
**Conclusion:**-


 1.) Overall adr of City hotel is slightly higher than Resort hotel and no. of bookings of City hotel is also higher than Resort hotel. Hence, City hotel is makes more revenue.
 
 2.) City hotel has slightly higher median lead time. Also median lead time is significantly higher for both hotels, this means customers generally plan their hotel   visits way early.
 
 3.) Almost 30 % of City Hotel bookings got canceled.
 
 4.) Both hotels have very small percentage that customer will repeat, but Resort hotel has slightly higher repeat % than City Hotel.
 
 5.) TA/TO is mostly used for planning Hotel visits well ahead of time. 
 
 6.) While booking via TA/TO one may have to wait a little longer to confirm booking of rooms.
 
 7.) GDS channel brings higher revenue generating deals for City hotel, in contrast to that most bookings come via TA/TO. City Hotel can work to increase outreach on GDS channels to get more higher revenue generating deals.
 
 8.) TA/TO has highest booking cancellation %. Therefore, a booking via TA/TO is 30% likely to get cancelled.
 
 9.) Longer lead time has no affect on cancellation of bookings.
 
 
 10.) Not getting same room as demanded is not the case of cancellation of rooms. A significant percentage of bookings are not cancelled even after getting different room as demanded.
 
 
 11.) Arrivals in hotels increases at weekends and also the avg adr tends to go up as month ends. 
 
 12.)Moslty bookings are done by couples(bookings have two adults).


**Conclusion**

(1) Around 60% bookings are for City hotel and 40% bookings are for Resort hotel, therefore City Hotel is busier than Resort hotel. Also the overall adr of City hotel is slightly higher than Resort hotel.

(2) Mostly guests stay for less than 5 days in hotel and for longer stays Resort hotel is preferred.

(3) Both hotels have significantly higher booking cancellation rates and very few guests less than 3 % return for another booking in City hotel. 5% guests return for stay in Resort hotel.

(4) Most of the guests came from european countries, with most of guests coming from Portugal.

(5) Guests use different channels for making bookings out of which most preferred way is TA/TO.

(6) For hotels higher adr deals come via GDS channel, so hotels should increase their popularity on this channel.

(7) Almost 30% of bookings via TA/TO are cancelled.

(8) Not getting same room as reserved, longer lead time and waiting time do not affect cancellation of bookings. Although different room allotment do lowers the adr.

(9) July- August are the most busier and profitable months for both of hotels. 

(10) Within a month, adr gradually increases as month ends, with small sudden rise on weekends.

(11) Couples are the most common guests for hotels, hence hotels can plan services according to couples needs to increase revenue.

(12) More number of people in guests results in more number of special requests.

(13) Bookings made via complementary market segment and adults have on average high no. of special request.

(14) For customers, generally the longer stays (more than 15 days) can result in better deals in terms of low adr.

**And many more conclusions.**
**Challenges**


(1) There were a lot of duplicate data.

(2) Data was present in wrong datatype format.

(3) Choosing appropriate visualization techniques to use was difficult.

(4) A lot of null values were there in the dataset.


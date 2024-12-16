# Hotel-Bookings-Dashboard-using-ELK-stack-and-Analyzing-Streaming-Data


### About the Dataset

# *Context*
Have you ever wondered when the best time of year to book a hotel room is? Or the optimal length of stay in order to get the best daily rate? What if you wanted to predict whether or not a hotel was likely to receive a disproportionately high number of special requests?

This hotel booking dataset can help you explore those questions!

# *Content*
This data set contains booking information for a city hotel and a resort hotel, and includes information such as when the booking was made, length of stay, the number of adults, children, and/or babies, and the number of available parking spaces, among other things.

# *Dataset Overview:*
Total Records: 119,390 rows
Total Columns: 21

# *Key Columns and Description:*

Hotel: Type of hotel (Resort Hotel or City Hotel).

Is Canceled: Indicates if the booking was canceled (0 = No, 1 = Yes).

Lead Time: Number of days between booking date and arrival date.

Arrival Date: Includes columns like arrival_date_year, arrival_date_month, and arrival_date_week_number.

Adults: Number of adults included in the booking.

Children: Number of children included in the booking.

Babies: Number of babies included in the booking.

Meal: Type of meal plan booked:

BB: Bed & Breakfast
HB: Half Board (breakfast + one meal)
FB: Full Board (all meals)
SC: Self-Catering
Undefined: No meal plan specified

Market Segment: Booking source or channel (e.g., Direct, Corporate, TA/TO, Groups).

Distribution Channel: Booking distribution method (TA/TO, Direct, Corporate, GDS).

Reserved Room Type: Type of room reserved by the guest.

Assigned Room Type: Room type actually assigned during the stay.

Stays in Week Nights: Number of nights the guest stayed during weekdays.

Stays in Weekend Nights: Number of nights the guest stayed during weekends.

Previous Cancellations: Number of prior cancellations for the guest.

Previous Bookings Not Canceled: Count of confirmed bookings in the past.

Reservation Status: Final status of the booking (Check-Out, Canceled, No-Show).

Days in Waiting List: Number of days the booking was on a waiting list.

Customer Type: Type of guest (e.g., Transient, Contract, Group).

ADR (Average Daily Rate): Average rate per day for the booking.

Total of Special Requests: Number of special requests made by the guest.

# *Acknowledgements*
The data is originally from the article Hotel Booking Demand Datasets, written by Nuno Antonio, Ana Almeida, and Luis Nunes for Data in Brief, Volume 22, February 2019.

# *Objectives:*

1. **Enhance Meal Offerings:**  
   - Promote **BB (Bed & Breakfast)** packages as the most preferred option.  
   - Improve flexibility and affordability of **FB (Full Board)** to increase adoption.  
   - Minimize "Undefined" meal types through better data collection.

2. **Optimize Booking Channels:**  
   - Focus on **TA/TO channels** for long lead-time bookings with early-bird offers.  
   - Boost **Direct and Corporate bookings** through targeted campaigns.  
   - Leverage **GDS and Undefined channels** for last-minute deals.

3. **Leverage Market Segments:**  
   - Capitalize on **Group bookings** with tailored packages and discounts.  
   - Strengthen **Online TA partnerships** to drive adult bookings.  
   - Expand **Corporate and Direct** segments for diversified revenue.

4. **Improve Occupancy Trends:**  
   - Boost **weekday stays** with business-friendly packages.  
   - Increase **weekend bookings** through family and leisure promotions.

5. **Reduce Cancellations and No-Shows:**  
   - Implement flexible cancellation policies with confirmation incentives.  
   - Reduce no-shows through deposits and timely reminders.

6. **Attract Family Bookings:**  
   - Offer family-friendly packages with discounts, kid-friendly meals, and activities.  

# *Insights*

## Graph 1. Count of Children:

o	Total number of children across all bookings: 51,469.

## Graph 2.	Average Lead Time per Distribution Channel:

o	TA/TO (Travel Agents/Tour Operators) has the highest average lead time, close to 100 days.

o	Direct and Corporate channels have moderate average lead times, around 60 days.

o	Undefined and GDS channels have the shortest lead times, averaging below 30 days.

Key Insight: TA/TO bookings require significantly more lead time compared to other distribution channels, while GDS and Undefined channels involve shorter-term bookings.

## graph 3. Average Lead Time by Market Segment:

o	Groups account for the largest share of bookings with 36.11%, followed by:

	Offline TA/TO: 28.77%

	Online TA: 15.98%

	Direct: 10.8%

o	Smaller segments include Corporate and Other.

## graph 4. Adult Count by Market Segment:

o	Online TA leads in the number of adults booked, with nearly 25,000 bookings.

o	Offline TA/TO comes next, followed by Groups and the Other segment.

Key Insight:

•	Group bookings dominate in terms of market share but not in total adults booked, where Online TA leads.

•	Direct and Corporate segments hold a smaller share, suggesting limited reliance on these channels for bookings.

## graph 5. Average of stays in weeknights vs. weekend nights

•	Average stays in weeknights: 2.925

•	Average stays in weekend nights: 1.106

  Guests tend to book longer stays during weekdays (average ~3 nights) compared to weekends (~1 night). This could indicate that:
  
•	Business travel is a primary driver for hotel bookings during weekdays.

•	Guests may book shorter stays on weekends, likely for leisure or short vacations.

## graph 6. Reservation status of Adults vs. Children

•	The Checkout status has a significantly high number of adults (~14) compared to children.

•	The Canceled and No-show statuses have relatively lower counts of both adults and children, with similar proportions for each.

•	Families with children tend to have fewer reservations compared to adults-only bookings.

•	The number of canceled and no-show bookings indicates a manageable cancellation rate, but cancellations may still need attention.

## graph 7. Reservation Status of Adults

•	Checkout dominates the reservation statuses (~35,000 adults).

•	Canceled reservations have a noticeable presence, though much lower compared to Checkouts (~15,000).

•	The No-show status is the least common among adults.

Most bookings successfully result in Checkouts, which is a positive trend for hotel operations. However, a considerable number of bookings are canceled, which might affect revenue forecasts.

## graph 8. Meal preferences of adults

1.	BB (Bed & Breakfast):
   
o	This is the most preferred meal option among adults, with nearly 40,000 counts in the graph.

o	It significantly surpasses all other meal types, indicating that guests prefer having breakfast included while maintaining flexibility for other meals.

2.	HB (Half Board):
o	The second most preferred meal option, with a steep drop in count compared to BB.

o	The HB meal includes breakfast and one additional meal (usually dinner), which appeals to fewer guests compared to BB.

3.	Undefined:
   
o	The third category represents "Undefined" meal types, indicating cases where the meal preference is not specified or missing in the booking data.

o	Its presence in the graph shows that some bookings did not clarify the meal plan.

4.	SC (Self-Catering):
   
o	This meal option, where guests prepare their meals, has an even smaller share compared to BB and HB.

o	Self-catering likely appeals to budget-conscious travelers or those staying in apartments.

5.	FB (Full Board):
   
o	FB (Full Board), which includes all meals, is the least preferred option.

o	Its low count suggests that guests are less inclined to opt for packages including all meals, possibly due to higher costs or reduced flexibility.







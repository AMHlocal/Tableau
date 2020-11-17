# Tableau-Challenge
Link to workbook: 
https://public.tableau.com/profile/austin.hauck4786#!/vizhome/CitiBike-Homework_16055788478190/CitiBikeStory?publish=yes


## Task
<hr>
Your task in this assignment is to aggregate the data found in the Citi Bike Trip History Logs and find two unexpected phenomena.
Design 2-5 visualizations for each discovered phenomena (4-10 total). You may work with a timespan of your choosing. Optionally, you may merge multiple datasets from different periods.
<hr>

## Next, as a chronic over-achiever:
<hr>
Use your visualizations (does not have to be all of them) to design a dashboard for each phenomena.
The dashboards should be accompanied with an analysis explaining why the phenomena may be occuring, in the analysis section of the ReadMe.
<hr>

## City officials would also like to see one of the following visualizations:
<hr>
Basic: A static map that plots all bike stations with a visual indication of the most popular locations to start and end a journey with zip code data overlaid on top.

The map you choose should also be accompanied by a write-up unveiling any trends that were noticed during your analysis, in the analysis section of the ReadMe.
<hr>

# Homework Breakdown
## Cleaning
After taking the data into a Jupyter Notebook for cleaning, the decision to remove data that is the upper bound of an IQR for each data set was made.

Data that is below 5 minutes (300 seconds in trip duration) was also removed to make sure that all the rides that are taken are rides that are meant to be taken instead of riders that decided to end their ride short, didn't mean to start a ride, or had times that just didn't seem logical for a paid bike ride.

# Analysis

## Top Stations Overall Dashboard
In this dashboard all stations are shown but the stations that are the most popular to start trips at are larger in size and darker in color. The explaination for why these stations are the most popular can be that the stations are near high tourest areas like Central Park, govenment buildings, popular piers, and universities.

## Top Start / End locations by Gender
In this dashboard each gender is broken to the most popular start and end locations. For Females the most popular locations are grouped around senic areas like Central Park, meaning that females could be using the bikes as a leasure activity. For Males the highest grouped stations are more in the business district, meaning that males could be taking bikes to and from work. For those who marked their gender as Unknown the most popular locations are grouped around senic areas like Central Park, meaning that the unknown gender could be using the bikes as a leasure activity like females.


## Ride Breakdown Dashboard
### Total Duration
In the customer category, unknown gender has the most time ridden while in the subscribers males have the most time. This trend is constant as you select a month to look at
With COVID-19 affecting every aspect in life it does not seem to affect the amount that people are riding as the amount of total duration increases from April to June, this can also be explained by the transition from Winter to Spring months bringing in warmer weather.

### Average Duration
While subscribers had a higher total time their average trip duration is lower than customers. This trend is constant no matter what month you select.
In both user categories females have a longer average duration than males, but a lower average than unknown gender. This means that on average females are taking fewer, but longer trips than males who seem to be taking more trips at longer durations

### Peak Start Times
For all months, the peak start times for rides are 8am and 5pm. For customers, the peak is only at 5pm. This leads to the thinking that users are using the bikes to go to and from work as the New York City area is known for having some of the worst traffic in the continental United States.
As we look at individual months the shift in peaks change. For April subs it is still 8am/5pm but with a lot fewer rides. April customers peak only at 5pm with the volumes of rides being around the same as March. May subs return to the 8am/5pm peaks with ride counts increasing, May customers peak between 4-5pm but have increased the volume of rides by nearly 32k. June continues the 8am/5pm trend for subs but now sees the most amount of ride at 5pm with 131k. June customers also see and increase in rides to peak at nearly 62k rides but continues to peak at 5pm.

### Peak End Times
For all months we see the same trend for the peak times. Meaning that the trips taken are mostly shorter.
We do see very obvious peaks when going to the individual months but these trends follow the “Start Times” very closely.
Some of the rides that started in June do go into July. Since data for July was not collected for this analysis the main explanation for this would be users that started rides towards midnight and ended sometime on July 1st as there are customer rides that last all day.




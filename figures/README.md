## Introduction
In February 2024, the Philippine Center for Investigative Journalism (PCIJ) collected data on the prices and process of booking a Grab ride on different routes and times of day. 

### Plots
1. Surge factor over time (split by route or destination, with peaks and dips) - DONE
2. Surge factor box plot and summary measures - DONE
3. Surge factor vs travel distance (to confirm correlation, and not travel time because price and therefore surge factor is determined beforehand) - DONE
4. Surge factor vs ETA and ETT (to check if their payment model still is reasonable even with surges) - DONE
5. OVERALL plot of surge factor vs time - DONE
7. ETT vs ETA (can put in fig 3) - DONE
8. Surge factor split by surge notice (dichotomous) 
9. LAST: MAKE SEPARATE SPREADSHEETS FOR EACH NOTEBOOK w/ specific data

## Insights
### Notebook 1 
Let's look at all the average peak and dip times of the surge factor over seven days on each of the routes. 

For Route 1 going to SM North EDSA, the peaks on weekdays tend to be later in the day, while on weekends the graphs tend to be unpredictable in where the dips and peaks will be. Sunday peaked later in the day while Saturday dipped.

For Route 2 going to UP Alumni Hostel, the first three days had consistent peaks around 10 to 15 hours after midnight. The range of surge factors lessened on Saturday and Sunday, but Sunday had one significant peak in the middle of the day. The two days after that had prominent dips but not a lot of peaks.

For Route 3 going to Mall of Asia Arena Coral Way, from Wednesday to Saturday, the graphs seem to be growing exponentially, peaking at times from 16 to 19 hours after midnight. For these days, the dips occured in the morning from 6 to 10 hours after midnight. The last three days had a smaller range of surge factors and more prominent dips than peaks.

For Route 4 going to SM Aura, it is expected to have the same results as Route 1, as they are both malls and it is assumed that higher surge factor means higher demand. For every day except Sunday, the peaks are from 15 to 19 hours after midnight. On Sunday, the surge factor peaks at 12 hours after midnight, probably due to people having lunch at this mall. The highest surge factor so far out of the four routes is seen on Saturday, with a value of 1.77 at 17 hours after midnight.

For Route 5 going to Puregold Paso de Blas, the peaks are usually in the morning from as early as 6 hours after midnight to 12 hours after midnight. This could be because people run errands in the morning. This route also has the lowest peaks out of all the routes.

For Route 6 going to 168 Shopping Mall, the range of surge factors looks fairly low (this will be verified in Notebooks 2). The peak times are unpredictable, either being around 8 or 19 to 21 hours after midnight. 

For Route 7 going to The Medical City Ortigas, the peak times range from 8 to 22 hours after midnight. The hospital can be needed at any time for emergencies, creating unpredictable surge factors. However, it is mostly during the day because of scheduled appointments. On Sunday and Monday, the range of surge factor was noticeably less than the other days.

For Route 8 going to One Orchard Road Eastwood, the peak times are usually in the late afternoon to night, from 16 to 23 hours after midnight. The area might have a popular nightlife. On Sunday, the range of surge factor is very low, the graph is almost a straight line with some distrubances.

For Route 9 going to Victory Liner - Pasay Terminal, the peak times have a very high range. They range from 6 to 22 hours after midnight. These times are usually midday to early afternoon. This is most likely because bus stops run all day and commuting is very common.

For the last route, Route 10 going to Baclaran Church, the peak times range from 0 to 17 hours after midnight. The dip times are mostly always at 8 hours after midnight. The day with the lowest surge factors and the most noticeable dip is Monday, maybe due to people already having gone to church on Sunday.

### Notebook 2
This is where the box plot and summary statistics about the calculated "Surge factor" can be found. 

Based on the box plot (Figure 2), the route with the highest range is Route 4, but the one with the highest median (since outliers are present) is Route 9. This route has a consistently high surge factor since its standard deviation is low. Route 4 also has the highest 75th percentile, while Route 5 has the lowest. Route 5 has the lowest range and a very low standard deviation. All the values for this route are low, implying low demand in that area (or high supply). 

### Notebook 3 
This was made to check the correlation between surge factor and distance of the travel. The correlation coefficient was too low (r = 0.155) so the plots have no significance. The question now is: if their is no correlation between these variables, then what does the surge factor depend on?

### Notebook 4
The surge factor does not depend on the ETT or ETA, but it has a weak correlation with the published fare. This is because the published fare is one of the factors in calculating for the surge factor. ETT doesn't depend on ETA either.

### Notebook 5
Someone who uses Grab often would want to know at what time is a good time to book a ride. A parametric test (utilizes means) and non-parametric test (utilizes medians in the presence of outliers) were run on the data to see if the surge factor varies across the different times. Both tests revealed that the surge factor does indeed vary significantly across different times with an alpha value of 0.01, meaning we are 99% sure this conclusion is correct. Knowing this, we can now see that the surge factor depends on different times of day. The time with the lowest median surge factor is 9 AM while the highest is 4 PM. 3 PM also has a fairly high median surge factor.  

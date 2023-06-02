Ask:

  Company goal: Convert casual riders to member riders.
  My business task: Analyze how annual members and casual riders use Cyclistic bikes differently and make recommendations on how to convert casual riders to annual members.


Prepare:
  The data I used was downloaded directly from the company's database. In total, there were 12 .csv files - one for each month from April 2022 to March 2023. Although there were some null values and outlier data, there was enough relevant information to perform an analysis.


Process:
  To process my data, I changed all 12 .csv files to .xlsx files, so I could import them into SQL Server. Then, I combined all 12 tables into one, making it easier to query my data in SQL. All cleaning and manipulation were saved locally in my "SQLQuery12" file.


Analyze:
  To analyze, I had to make sure I had all the relevant columns in my SQL table. I created extra columns for date and time, as there was only a DATETIME column provided; ride length by day and minute, day of the week, and month. All these queries are in the same SQLQuery12 file.


Share:
  Currently, casual riders make up 40% of all Cyclistic users, so it is worth the effort to convert them to members. To do this, we must understand the key difference between casual and member riders: what they used the bikes for. Member riders tend to use the bikes for commuting to and from school or work, while casual riders use them for leisure, usually in scenic environments. When coming up with business recommendations, we must look at some key metrics.

  First, let’s look at time of use. Unsurprisingly, the month-by-month popularity of the bikes is the same for both casual and member riders, peaking in the summer months and valleying in the winter months.However, if we break it down by week and day, we see some interesting differences. Weekly, we see that member riders plateau Monday through Thursday, have a slight decrease on Friday, and drop significantly on the weekends, implying that members are using the bikes for commuting to work or school. This implication is backed when we look at the daily popularity. With member riders, we see spikes at around 8:30 AM and 5:30 PM - right before and after the workday. Casual members, on the other hand, have a peak on Friday, Saturday, and Sunday with no morning spike but instead a gradual climb to a peak at around 6 PM. Member riders prefer using the bikes during workdays and work hours, while casual riders are the complete opposite. If we want to convert casual riders, we have to cater to those who ride for leisure, not for commute.

  Second, let’s look at location of use. The three most popular stations by ride count are on the campus of the University of Chicago. The next three are in the downtown area of Chicago. The top three most popular stations for casual riders are along the lakeshore, in parks, and other scenic areas. This is especially true for the most popular station, located in tourist attraction Navy Pier, with a total ride count of nearly 40,000 riders in 12 months. This is almost double the second most popular station which had just under 22,000 riders in the same time span. This tells us that if we want to convert casual riders into members, we need to focus on these parks, piers, and other scenic places.

  One other important metric to consider is the average ride time for each group. Members ride for an average of 12.20 minutes, while casual riders ride for an average of 21.39 minutes. Casual riders ride for nearly twice as long per ride. For each rider we recruit from a leisure ride in the park, it would be like recruiting two commuter riders.

My recommendation:
  1. Focus on parks, scenic routes, and tourist areas. It is clear that casual riders prefer riding in these areas, and it would be easier to connect with them. For some ideas, we can host events in the parks, partner with the parks to give discounts, or create bike routes that can only be used by member riders.
  2. Offer an evening discount, as that is when casual riders are most active. For example, we could partner with local restaurants or have an event like a group sunset bike ride.
  3. Offer a seasonal membership. Obviously, both members and riders ride outdoor bikes more in the summer, but the nice weather is a bigger plus for the casual riders, who are riding for sheer pleasure. Offering a seasonal membership would be more attractive to casual riders.

Other insights:
  Member riders prefer the classic bike over the electric bike, while casual riders prefer the opposite. However, the top three stations used by casual riders, including the Navy Pier station, use classic bikes. Therefore, I don't think marketing electric bikes is the best strategy, even though that is what casual riders generally prefer.

What I learned:
	This was my first non-completely guided data analytics project, and I learned plenty more than just Excel, SQL, and Microsoft PowerBI. Going through the Google Data Analytics Certificate taught me how to have the proper mindset before going in and playing with data. As I was first learning data analytics and going through guided projects on YouTube, I only wanted to play around with the data. Having Google lay out the steps of Ask and Prepare taught me to think deeper about my data and what exactly it is I am doing before I actually do it. Making sure the data ROCCCs, making sure I am documenting everything properly, making sure I know the business task are all important concepts that I did not consider before. Answering those questions gave structure to my work in Excel, SQL, and PowerBI. Finally, seeing a real “best in class” presentation of a data project was incredibly helpful. It gave me something to strive for and, again, was a reminder that data analytics is not just playing around with data in SQL and PowerBI. This certificate and capstone project was a great lesson in the foundations of data analytics. 
 

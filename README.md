# Excel-Kickstarter-Project

## Problem Description: 
Though, over 2B is raised is Kickstarter crowdfunding platform, only a third of campaigns are successful in raising the required funds. 


## Analysis Goal: 
Find out the reasons behind success and failure in a Kickstarter campaign using the data from the past campaigns


### Exploratory Analysis

**Analysis identifies high and low performance categories based on their success rate. Some results are surprising !**

Kickstarter campaigns in music category has the highest success rate (About 77%) whereas journalism campaigns has striking 0% success rate (all of them are cancelled). Theatre and Film & Video are the other well doing categories with about 60% and 58% respectively. On the contrary, Food category is performing poor with a low 17% success rate. 

<div style="text-align:center"><img src="graph1.png"></div>

Looking into the sub-categories of the high and low performing categories indicate that
- Rock (a 100% success rate!) and indie rock contributes to the success of music category
- Theatre category is kind of a safe zone, where all the categories are likely to succeed more than half a time. Also, there are significantly more “plays”  than any other type of campaigns overall. However, this posses only about 65% success rate
- It seems like backers love non-fiction, radio & podcasts (both at 100% success rate) and totally hate everything else (100% failure rate)!
- Similarly, while table-top games getting  100% success mobile and video games getting 100% failure ! (Big surprise)
- “Wearable” campaigns are the main reason why Technology category is not performing. However, “hardware” campaigns are doing well with 100% success rate.
- Documentaries (in film & video category) has a 100% success rate! 
- “Food truck” campaigns (100% failure) are the main contributor to the low performance of “food” category 
The below graph helps to illustrate the success rate and the number of the campaigns for all subcategories. Moving towards up and right indicates high success with greater number of campaigns. “Rock” is giving 100% success rate with about 300 campaigns 

<div style="text-align:center"><img src="graph2.png"></div>

**
Kickstarter got extremely popular in 2015 as number of campaigns surged. However, this declined the success rate. This might be because, the number of backers and their investment might not have increased proportionately, resulting in the investment splitting across multiple projects, leading to many projects not able to meet the goal.
**

<img src="graph3.png" style="float:left"><img src="graph4.png" style="float:left">

The total campaign numbers finds a peak at 2015, however, it appears that success rate is relatively low in that year. Though, there is a growth of Kickstarter campaigns  between 2013 to 2015, success rate declined during this period with a higher failure rate. And it is growing upwards since then, though the total number of campaigns are reducing. 

**Least campaigns happens in December but also, this month sees the lowest success rate. This might not be a surprise as it is a festival month and people usually takes off from work**


<img src="graph5.png" style="float:left"><img src="graph6.png" style="float:left">

**Based on further Analysis**

**There are fewer campaigns with higher goals. Also, as the goal amount increases success rate decreases, with an exception between 30000-50000 with a slight increase**

<div style="text-align:center"><img src="graph7.png"></div>


### What are some limitations of this dataset?

- The analysis has only limited data. 
  - The critical information about campaign owners and members (for example the stars acting in a TV show), the success (failure) history of campaign owners based on their previous campaigns (if any) are not present
  - Information on traffic to the campaign is not given (click stream analytics/google analytics) to understand the important information like the conversion rate (How likely a backer pledge after viewing the campaign? This could be proxying how interesting the campaign is)
  - This analysis is solely based on parameters given below:

   - goal – required funding
   - pledged – obtained funding
   - state – state of the campaign (successful, failed, live, canceled)
   - country
   - currency
   - deadline
   - launched_at
   - staff_pick – kickstarter chosen interesting campaigns
   - backers_count – No of backers
   - spotlight – Feature gets kicked in after successful funding (not useful)
   - Category and Sub-Category

 - Not having a detailed description (apart from “name” and “blurb”) of the campaigns to do an effective analysis (E.g.: Predict whether a campaign succeeds or not based on the text in description. This proxies how well the description is crafted. A bad written campaign cover might end up failing, just like a badly done resume gets no attention)

 - Dataset doesn’t contain information on a daily basis pledge details, rather contains only the final/total outcome (This information could have been used for understanding the relationship with time and pledge amount for different campaigns. For instance, if we identify a successful campaign’s pledge grows exponentially over time (per days), it is possible to predict the status of the campaigns well in advance and can take proactive measures to ensure the success.


### What are some other possible tables and/or graphs that we could create?

Along with the plots used to explain above conclusions, the below ones could be useful

- A frequency plot (histogram), to capture the relationship between state and backers (1 each for success and failed states). This is to see if there is any relationship between number of backers and the destiny of the campaign

- A frequency plot (histogram), to capture the relationship between state and goal (1 each for success and failed states). This is to see if there is any relationship between the goal and the destiny of the campaign

- A frequency plot (histogram), to capture the relationship between duration and goal (1 each for success and failed states). This is to see if there is any relationship between the duration and the destiny of the campaign

- A pivot table between state and staff_pick showing the count of campaigns. This is to understand if there is any advantage of being chosen as a staff_pick campaign

## Statistical Analysis and Final Conclusions

The statistical measures on backers count for successful and failed campaigns are as shown below



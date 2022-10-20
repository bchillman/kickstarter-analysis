# An Analysis of Kickstarter Campaigns

## Overview of Project
In this project, we have looked at data from previous Kickstarters in order to give Louise more information about her play, *Fever*. Witht this analysis, Louise can hopefully make a more informed and better decision about the Kickstarter for her play. This analysis includes identifying how outcomes changed based on when in the year the Kickstarter was launched, so that Louise can compare her own Kickstarter to these trends. Also included is analysis of the success of Kickstarters based on what the monetary goal of the Kickstarter was. Using these, hopefully Louise can identify whether the success or failure of her own Kickstarter was due to one of these trends.

## Analysis and Challenges
This analysis was done fully in Microsoft Excel. Using the data of over 4,000 Kickstarters, the 
### Launch Date Analysis
First, the launch date of these kickstarters was analyzed. A pivot table was created from the data with the category of Kickstarter and year that the Kickstarter was launched as filters. This pivot table describes the the outcome of the Kickstarter (successful/failed/canceled) as dependent on the month that the Kickstarter was launched. Finally, the category filter was used to only look at Kickstarters in the **Theater** category since only these are relevant to Louise's interests. A graph was made based on this pivot table, as shown here.

![Theater_Outcomes_vs_Launch.png](https://github.com/bchillman/kickstarter-analysis/blob/main/Resources/Theater_Outcomes_vs_Launch.png)
This graph shows how many successful, failed, and canceled kickstarters there were that were launched in each month. The year filter was not used, however, it could potentially be used to see if more recent Kickstarters followed the same trends that were seen across all years.
### Goal Analysis
Second, the monetary goal of these kickstarters was analyzed. First, 12 buckets were made to sort the goal amounts into:
1. Less than $1,000
2. Between $1,000 and $4,999
3. Between $5,000 and $9,999
4. Between $10,000 and $14,999
5. Between $15,000 and $19,999
6. Between $20,000 and $24,999
7. Between $25,000 and $29,999
8. Between $30,000 and $34,999
9. Between $35,000 and $39,999
10. Between $40,000 and $44,999
11. Between $45,000 and $49,999
12. More than $50,000
Then, the number of successful, failed, and canceled Kickstarters in each of these buckets was counted (making sure to only include Kickstarters in the subcategory of **Plays**), and the percentage of each of these outcomes was calculated for each bucket. These percentages were then graphed, as shown below:
---
![Outcomes_vs_Goal.png](https://github.com/bchillman/kickstarter-analysis/blob/main/Resources/Outcomes_vs_Goals.png)
This gives us and Louise an idea of how changing the goal of a Kickstarter can affect the outcome of that Kickstarter.
### Challenges
I only ran into one challenge while performing these analyses. This came in the analysis of the outcomes based on goals. While attempting to sort the data based on the buckets that were created, I incorrectly defined the limits of the buckets in my COUNTIFS function. I noticed as I was filling these cells, that there was a very small number of Kickstarters as I was getting to larger goals and that my subsequent graph was not going to look like the sample graph provided. After I filled all this data in, I checked the total number of Kickstarters that I was looking at and compared it to the total number of plays in the data. When I saw that I was missing about 15-20%, I went back and checked the limits I had used in my formulas and realized I was not including any Kickstarters that were exactly $1,000, $5,000, $10,000, etc. This was a fairly quick fix, and was easily checked to make sure it was fixed.
## Results
These analyses provide us with some interesting results for Louise to consider. 

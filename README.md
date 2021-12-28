#Kickstarter Analysis
##Project Overview and Purpose
	This project was meant to investigate data from Kickstart campaigns to find trends to help determind if there are factors that can help a campaign's successful funding.
	For my purposes, I was helping someone that wanted to successfully obtain funding to preform the play _Fever_, a one-man show theatrical production.
	The fact that they were starting a Kickstarter for a play helped narrow the focus of my analysis to find successful and unsucessful treads for theater/play kickstarters.
	With the provided data I was able to find certain treads and recommened critera that, when followed, would suggest a higher likelyhood of obtaining full funding for the production.
##Analysis and Challenges
###Analysis
The data consisted of 4115 Kickstartes between the years of 2009 to 2017
Data from successful and failed Kickstartes came from a large variety of categories including... 
	-Film and Video
	-Food
	-Games
	-Journalism
	-Music
	-Photography
	-Publishing
	-Technology
	-Theater
Within the workbook I generated seperate sheets with data that breaks down and visulizes...
	-Category and Subcategory Statistics
	-Descriptive Statistics
	-Outcomes based on launch date
	-Outcomes based on funding goals			
To begin my analysis of the data I first looked at the overall workbook to get an idea of the data that had been pull for me.
Since my analysis was for the purpose of helping with a play, I generated more columns to be able to filter down to the parnet categories (listed above) and subcategories (specifically plays).
From there I was able to gather statistics and visulize treads.
Some of the points I put together included If when the campaign was launched effected success and if the funding goal effected success. These fomulas used to gather the data for outcomes based on goals were the longest of the entire analysis.
`=COUNTIFS(Kickstarter!$F:$F,"successful",Kickstarter!$D:$D,">=1000",Kickstarter!$D:$D,"<4999",Kickstarter!$R:$R,"plays")` This formual, and the others like it in the Outcomes Based on Goals sheet, were used to collect and seperate the number of campaigns that were or were not successful and the funding goal.
This particular fomula is to count the number of play campaigns that were successful with funding goals between $1000 and $4999. The vizulaization for this and the other data collected for outcoems based on goals is found below in the Results section.
##RESULTS
###Theater Outcomes by Launch Date		



Conclusions from the theater outcomes when focusing on when to launch the campaign (see corresponding line chart)
	1. The data shows that there is an increase in success rate of campaigns that begin in the month of May.
		**Late April to early May would be the best time to launch any theater related kickstarters** 
	2. The data shows that the chance of success steadly decreases through the rest of the year with December being the worst time to launch a campaign
		**Idealy, the lastest to begin a theater based kickstarter campaign would be July**
	Based on these findings, the time of year to ensure the greatest chance of success would be early to mid summer. 
###Outcomes Based on Goals



Conclusion from the outcomes of kickstarter campaigns for plays when focused on funding goals (see corresponding line chart)
	1. There are few plays that are successfully funded that have funding goals greater than $5000
		**The percentage of successful campaigns drops approximately 25% when the funding goal is greater than $5000**
Based on this finding, the ideal funding goal is less than $5000			
##Limitations
	1.	More investigtation into the specific successful and failed campaigns marketing could be of great use.
		If possible, data for marketing stratagies, calls to action, and breakdowns of backer benefits could generate very valuble data for how to have a successful kickstarter campaign.
	2.	Since this specific play _Fever_ is a one-man show production, it would have been more beneficial to analyze other Kickstarters that were for other one-man shows.
		When sifting through the data, only six of the play campaigns were also one-man shows (according to the **Blurb** column when searching for "One-Man"). 
		The ability to preform analysis on more one-man shows could prove to show specifically what factors matter most for successful funding of that type of production.
			**Note: all one-man shows in the data were succeffully funded and had funding goals less than or equal to $5000, which falls in line with our conclusions.
	3.	While there was a substatioal amount of data to work with, there could always be more. More data would help to get more accurace results/findings.
		According to Kickstarter.com, there have been nearly 214,000 successfully funded campaigns while the raw data in my analysis only covers 4115. 
		Of course analysis of all of these campaigns is not nessecary, but more data is always going to help improve the accuracy of the results.				
##Challenges and Difficulties Encountered
There were a handful of challenege that required a few extra steps/more effort to overcome. 
	1. ome relevent data needed to be converted/altered into readable formats. For example the raw data for dates were in unix timestamps, which requried converting. I did this using this formula `=(((J2/60)/60)/24)+DATE(1970,1,1)` which converts the unix timstamp to the mm/dd/yyyy format. 
	2. at one point I thought my data had been corrupted because I was unable to scroll or build new pivot tables. Thankfully I was able to troubleshoot and resolve the issue and it turned out to be that the "freeze panes" option had prevented my analysis. An easy fix and a mistake I wont make again!

				
				
				
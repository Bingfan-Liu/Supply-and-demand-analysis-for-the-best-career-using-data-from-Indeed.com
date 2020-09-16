# A Short Supply and Demand Analysis for the Careers using Data from Indeed.com

#### Approximated readding time is about 10 mins


### Part 1: The dataset and its relavance to the whole Canadian labor market
This analysis used the data obtained from the Indeed.com contained the information about the job postings in varies industry in 2018. And the goal of this analysis was to use the data from the Indeed.com to predict which kind of jobs or the industries would be good to step into years later.  

The job information from Germany, Canada, and USA from the Indeed.com were gathered initially. Hoever, because of different histories, locations, cultures, and policies, the structures of the labor market are different between German, Canada, and the USA. And also the labor is hard to move between countries. So, it’s probably a good reason to look at only one country, Canada, rather than all of the three. It was assumed that for each job ID, it only corresponded to one job opening, and this is the same for all industries. Thus, the jobs were mapped into the same industrial category as to how it was defined in Bank of Canada. 

The first thing that was taken into considerations was whether the indeed.com dataset can be a good representative of the labor market in Canada. On the top left side of the first page, the employment information of different industries from Statistics Canada was obtained. And about 5% of the working-age population were unemployed which could be ignored in this analysis since this was the controlled rate of unemployment in Canada, and most of them would find a job within the next 3 months. Thus, the total employment status in Canada was assumed to be satisfied which means that the number of employments in the market is equal to the demand of labor in the market. And the demand of the labor referred to the number of the jobs offered by the companies in Canada during this year. 

On the bottom of the first page, the left side plot was the demand of the labor in the indeed.com dataset. And that demand in the indeed.com dataset was considered as a subset of the whole Canadian labor demand in the market. By comparing to the employments in Canada (the demand of the labor in Canada) in the right side plot, we would find that the volumes of the labor demand in different industries in the two sources were almost matched. The top 4 industries in indeed.com were still the top 4 industries from the data from Statistic Canada. There was a larger proportion of the professional service jobs demanded in the Indeed.com than that across the whole country. Those were mainly technology-related jobs. This may indicate that people should probably find tech jobs using Indeed.com. However, for this analysis, we believed the bias in the profession of the audience was heavily skewed towards technology or STEM-related professions. So, we will ignore the bias in the dataset here.  

### Part 2: The demand and supply relationships in the market
Since it could represent some features in the whole labor market in Canada, we could then look at the supply and demand relationship in the whole market only using the Indeed.com dataset. Define the supply of the labor to be the number of clicks in each job and categorize them into the same industrial categories defined by Statistics Canada. 
Then, we could obtain the two plots of supply and demand in Canada on the top of the second page. We wanna see if there is some miss allocation of the labor resources by comparing the proportions of the supply and demand of jobs in different industries. For example, is there a large demand in the farming industry while everyone wants to do cs jobs or searching cs jobs here?

However, as we could see that not only the ranking of the supply and demand were the same but also the proportions were similar. The only difference existed in the ranking of Manufacturing and business support services jobs. And there was more demand for labor than the supply for labor in manufacturing. So you may wanna find a manufacturing job in the future rather than business, support services. Or you may want to go indeed to find jobs in manufacturing industry.

But the disadvantage of just using the Indeed.com dataset was that we can not predict the labor in the further future since the data was only about one-year-long in 2018. So, the data obtained from Statistics Canada over the past 12 years (the max people can get) were subtracted and were used in training times series models like ARIMA, VAR, and etc. The labor demand and the growth rate of the labor demand were both predicted and summarized in the bottom. There are many industries that had high current labor demand. However, for the young job seeker, the recommendation was to combine the demand and the supply status from the top image and looked for industries that would have high labor demand and relatively high labor growth rates in the future. 






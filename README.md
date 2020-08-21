# Weather_Trends_UdacityProject1

## Introduction
----------------------------
A/B tests are very commonly performed by data analysts and data scientists. It is important that you get some practice working with the difficulties of these
For this project, you will be working to understand the results of an A/B test run by an e-commerce website.
Your goal is to work through this notebook to help the company understand if they should implement the new page, keep the old page, or perhaps run the experiment longer to make their decision.

### Part I - Probability:
----------------------------
**1.** Now, read in the ab_data.csv data. Store it in df. 
**2.** For the rows where treatment is not aligned with new_page or control is not aligned with old_page, we cannot be sure if this row truly received the new or old page.

### Part II - A/B Test:
----------------------------
Notice that because of the time stamp associated with each event, you could technically run a hypothesis test continuously as each observation was observed.
However, then the hard question is do you stop as soon as one page is considered significantly better than another or does it need to happen consistently for a certain amount of time? How long do you run to render a decision that neither page is better than another?
These questions are the difficult parts associated with A/B tests in general.

**1.** For now, consider you need to make the decision just based on all the data provided. 
If you want to assume that the old page is better unless the new page proves to be definitely better at a Type I error rate of 5%.

''Null hypothese -> H0: Pold>=Pnew
Alternative hypothese -> H1: Pnew>Pold''

**2.** Assume under the null hypothesis,  pnew and pold both have "true" success rates equal to the converted success rate regardless of page - that is pnew and  pold
are equal. Furthermore, assume they are equal to the converted rate in ab_data.csv regardless of the page. Use a sample size for each page equal to the ones in ab_data.csv. 
Perform the sampling distribution for the difference in converted between the two pages over 10,000 iterations of calculating an estimate from the null. 

### Part III - A regression approach:
----------------------------
**1.** In this final part, you will see that the result you acheived in the previous A/B test can also be acheived by performing regression.




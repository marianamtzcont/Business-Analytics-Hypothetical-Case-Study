## **Business Analytics Hypothetical Case Study**
Analyzing the state of a fictional credit startup called *Credit Up For All*

---------------

By considering the state of the business, first, this analysis aims to study the startup's profitability, net income, and other aspects for the following 12 months. After analyzing the Contigo products, we will analyze a strategy for Contigo A customers to render this customer segment profitable.

*The data and the case study were taken from a test to apply for a position in the Business Analytics team in a company. Some information was modified.*



#### Business description 

---------------

Credit Up For All has one credit product called Contigo. Depending on risk, the customer will receive:

1. Contigo A given to high risk customers: $1,000 loan to be paid in full after one month with 15% interest. 

2. Contigo B given to low risk customers: $2,000 loan to be paid in full after one month with 10% interest. 


Past debt delinquency (DQ) rates have determined the interest for both products. Is estimated that the monthly DQ rate A will be 13.5% and 8% for B, throughout this year.

Credit Up startup has an ambitious growth plan for the year. At month 1, the company had a total of 5,000 Contigo A customers, expected to grow at a rate of 25% month over month. Contigo B has the largest share of customers, 10,000 in total. But with a very competitive market for premium loans, Contigo B is expected to grow at a 10% month over month rate throughout the year. The operation of this startup scales proportionately to its customer base, with negligible fixed expenses.

The current operative monthly cost per account sits at $30.

*Business analysis, part 1.*


The startup is concerned that the change in DQ rates and the aggressive expansion may reduce profitability in the following months. We need to analize: 
- what factors may be against the profitability of the startup? What should we look at in an analysis of the net income for the following months? 
- Is this startup going to be profitable during the next 12 months? What are the major trends driving changes in net income?
- What changes are required to sustain the business not only throughout the year but in the long run? 

These questions and the explanation are shown in the "Business Analytics Hypothetical Case Study.py" file 

#### Description of collection strategy 

---------------


The Credit department has decided to prioritize collections on Contigo A customers, since they have the largest DQ rate. A collections analyst has determined that a DQ rate of 10% will be enough to render this customer segment profitable. The team has decided to apply immediate action from month 1 and is looking for a collection strategy to recover (at least!) 175 of the 675 accounts that went delinquent, out of the starting 5,000 Contigo A accounts.

One idea is to collect by calling the customer. Using the collection results, the data science team has created a model to estimate contactability (i.e. the probability of reaching the customer successfully by calling). The collections team estimates that the customer will pay around three quarters of the time after being contacted, and it has no chance to pay if they never connect the call. Calling the customer is quite expensive! Operations has determined that a phone call campaign costs around 30 pesos per DQ customer, regardless of the contact result. The contactability scores are available in the "contactability_scores.csv" file 

*Analysis of a collection strategy, part 2.*

The startup wants to launch this campaign to all 675 DQ customers. We aim to compute the probable results for some main KPIs, such as recovered accounts, total debt recovered, revenue coming from collected interest, and so on. We will also analyze the impact this campaign has on overall business performance. Finally, we will suggest some possible improvements for this campaign.

The analysis needed for this part was performed in "Analysis_of_collection_strategy.sql" and the results were resumed in a dashboard in the "Analysis of collection strategy_resume.xls" file.

#### Results

---------------


*Business analysis*

Based on the analysis done, we are able to determine: 

- The Startup is not going to be profitable not even in the first month.The forecast shows it is necessary to apply immediate changes. The main trends driving changes in net income are interest rates which seems to be too low and affecting profitability. Another trend is the composition of the credit portfolio rates of the accounts. Also, delinquency rates are affecting interest income and loan losses.

- The company is experiencing losses, and starting from month 6, it has more customers in product A compared to product B, which exposes it to higher potential losses due to defaults. Since Contigo A customers are considered high-risk and have high delinquency rates, the rapid increase in the number of Contigo A customers results in the acquisition of high-risk clients, as reflected in the composition of the credit provided which by month 10, the company would be lending the same amount of money for both products



*Analysis of a collection strategy*

Based on the analysis done, we were able to determine the campaign results which are summed in the below visualization.
 


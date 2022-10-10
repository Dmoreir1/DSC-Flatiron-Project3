# DSC-Flatiron-Project3

## Business Objective 
Gemtel has recently experienced a decline in customer retention. So we were asked to investigate this decline. We began by investigating the amount of customers that terminated their contracts followed by the factors that had the most influence on customer turnover. And finally, we came up with implementable strategies to minimize customer turnover.  

## Initial Analysis, methodology, and limitations  

### Our investigation found that of the accounts we researched, 483 customers had churned which was equal to about 14.5% of the client base we sampled. 
### We saw a loss of about $27,100 in revenue with the average plan costing $58. That equated to a substantial 16.9% of total revenue. 
![prop to customer churn p3](https://user-images.githubusercontent.com/103558721/194739977-afdc6ff3-54ee-4be9-a3d3-00d9d700c2e3.png)


![p3 abu](https://user-images.githubusercontent.com/103558721/194739981-87217421-1861-4927-b714-019e9b9ed310.png)

This is Mr. Abu Sami. We reached out to several customers who left and found Mr. Sami’s story was similar to many others.  We asked what his reasons were for stopping service with Gemtel. Mainly, it was due to high fees incurred for international calls (to speak with his family in the US) and the lack of resolve when he reached out to the customer care team.  We decided to investigate Mr. Sami’s account...

![bluf p3](https://user-images.githubusercontent.com/103558721/194787931-aef4db72-cc18-40df-b86f-da9ef9fde4ad.png)

And we learned that this was a common scenario. The primary factors linked to the customer attrition were above average calls to the customer care team, the high price for international plans, and the lack of voicemail features

Factors we used in our modeling included age of the account, the frequency of customer service calls, voicemail usage, total minutes, International plans, and overall cost of plans. 

We ran several models and found our most successful to be XGBoost.. We gauged its performance using a metric called Recall. At 96%, we chose this metric as it minimizes the likelihood that our predictions would wrongly estimate a customer staying with Gemtel when they would actually churn- in other words we chose to err on the side of caution. Our data was limited to account/phone usage but lacked demographics. We were also limited in our sampling by geographic region vs international usage patterns



![p3 features](https://user-images.githubusercontent.com/103558721/194739983-435874bc-0ca4-47e9-84d5-010ae5c6e1af.png)


The features that contributed most to high attrition rate at GemTel:
1) Customer Service Calls
2) International Plan
3) Total Bill Charge
4) Voicemail

![p3 customer care calls](https://user-images.githubusercontent.com/103558721/194739988-902f7ae5-62f7-46b7-8d3a-07fca9341352.png)


Our Analysis found that customers who called customer service line 2 or more times increased the likelihood of them leaving GemTel by 30%.

<img width="650" alt="international plan" src="https://user-images.githubusercontent.com/103558721/194739998-8a756122-4557-4b1b-98d4-e7db3192fb30.png">

Additionally, we learned that many customers with international plans were overall making less international calls than those without the plan. 45% of the time customers playing for the additional plan left as cost was too high. 

<img width="659" alt="price churn p3" src="https://user-images.githubusercontent.com/103558721/194739997-a3a0f303-a7af-4f98-baa7-f0200dddb7dc.png">
When it came to recurring monthly charges, we found the threshold of $70 or more the point where customers were most likely to leave. 

<img width="759" alt="vm vs churn p3" src="https://user-images.githubusercontent.com/103558721/194739996-49ebb3a9-555d-4d88-b29b-2ed23fe4b44d.png">

Lastly, out of the 3,333 customers sampled, 842 customers had the voicemail plan. Of the customers that were paying for the voicemail plan, about 80 (or 9%) had left. 403 or 18% of the customers who did not have the voicemail plan found the additional fees for using voicemail too high and churned.

## Recommendations

### 1) Retention calls and save attempts
![offer accepted p3](https://user-images.githubusercontent.com/103558721/194739995-ca7ae002-9669-42ad-a315-cfb1140c3761.png)

We scraped and analyzed data from competitor telecommunication companies, focusing on factors they had utilized to increase customer retention and found that 
one strategy was to initiate 'save attempts' or make retention calls with retention offers to prevent customers from leaving or bring them back. With success rates above 50%, we recommend initiating save attempts for customers that have been tracked in making 2 or more customer service calls to prevent them from churning. 

### 2) Lower average plan price
![avg cost of plan p3](https://user-images.githubusercontent.com/103558721/194740000-62880bdb-ab6b-4e5f-99ff-8ad319360047.png)
We compared the average plan price of GemTel customers who had churned vs customers of competitors that also churned, and found that Gemtel plans were on average $10 more a month. Our recommendation is to offer a lower standard plan price to be more competitive 

### 3) Billing Structure
![biling structure p3](https://user-images.githubusercontent.com/103558721/194788614-d41b2384-f84c-48b8-89c9-22887534fa41.png)
Gemtel calculates their total charge by adding up the various charges including daytime/evening/night time/international usage minutes -all individual charges. In comparison, competitors offer standard plans then place additional fees based on features. We recommend offering a more simplified, customer friendly billing structure


## Future Considerations 
#### 1) Utilize AB testing to see what promotions yield the best results / highest customer acquisition 
#### 2) Deeper dive into customer base demographics; analyze usage trends based on age, location, household income level, etc.
#### 3) Investing in other technologies to offer additional features like 5G or wifi calling


![abu final p3](https://user-images.githubusercontent.com/103558721/194739999-5cfc2fb3-1d5d-4774-aa08-7885449882db.jpg)
We reached out to Abu Sami and asked if he would come back (possibly as a test group)  if these recommendations were implemented including lower plan cost that included features like international calling… and he said yes (given he would receive a free iphone). 


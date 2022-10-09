# DSC-Flatiron-Project3

## Business Objective 
Gemtel has recently experienced a decline in customer retention. So we were asked to investigate this decline. We began by investigating the amount of customers that terminated their contracts followed by the factors that had the most influence on customer turnover. And finally, we came up with implementable strategies to minimize customer turnover.  

## 

Our investigation found that of the accounts we researched, 483 customers had churned which was equal to about 14.5% of the client base we sampled. 

![prop to customer churn p3](https://user-images.githubusercontent.com/103558721/194739977-afdc6ff3-54ee-4be9-a3d3-00d9d700c2e3.png)
How much of a hit was this loss? Well, lets talk money. We saw a loss of about $27,100 in revenue with the average plan costing $58. That equated to a substantial 16.9% of total revenue. 



![p3 abu](https://user-images.githubusercontent.com/103558721/194739981-87217421-1861-4927-b714-019e9b9ed310.png)

Well I’d first like to introduce you to a former customer, Mr. Abu Sami. We reached out to several customers who left and found Mr. Sami’s story was similar to many others.  We asked what his reasons were for stopping service with Gemtel. Mainly, it was due to high fees incurred for international calls (to speak with his family in the US) and the lack of resolve when he reached out to the customer care team.  We decided to investigate Mr. Sami’s account...
![p3 features](https://user-images.githubusercontent.com/103558721/194739983-435874bc-0ca4-47e9-84d5-010ae5c6e1af.png)
And we learned that this was a common scenario. The primary factors linked to the customer attrition were above average calls to the customer care team, the high price for international plans, and the lack of voicemail features
We ran several models and found our most successful to be XGBoost. We gauged its performance using a metric called Recall. At 96%, we chose this metric as it minimizes the likelihood that our predictions would wrongly estimate a customer staying with Gemtel when they would actually churn- in other words we chose to err on the side of caution. Our data was limited to account/phone usage but lacked demographics. We were also limited in our sampling by geographic region vs international usage patterns
Factors we used in our modeling included age of the account, the frequency of customer service calls, voicemail usage, total minutes, International plans, and overall cost of plans. 

![p3 customer care calls](https://user-images.githubusercontent.com/103558721/194739988-902f7ae5-62f7-46b7-8d3a-07fca9341352.png)

<img width="759" alt="vm vs churn p3" src="https://user-images.githubusercontent.com/103558721/194739996-49ebb3a9-555d-4d88-b29b-2ed23fe4b44d.png">
<img width="659" alt="price churn p3" src="https://user-images.githubusercontent.com/103558721/194739997-a3a0f303-a7af-4f98-baa7-f0200dddb7dc.png">
<img width="650" alt="international plan" src="https://user-images.githubusercontent.com/103558721/194739998-8a756122-4557-4b1b-98d4-e7db3192fb30.png">
![offer accepted p3](https://user-images.githubusercontent.com/103558721/194739995-ca7ae002-9669-42ad-a315-cfb1140c3761.png)
![abu final p3](https://user-images.githubusercontent.com/103558721/194739999-5cfc2fb3-1d5d-4774-aa08-7885449882db.jpg)
![avg cost of plan p3](https://user-images.githubusercontent.com/103558721/194740000-62880bdb-ab6b-4e5f-99ff-8ad319360047.png)

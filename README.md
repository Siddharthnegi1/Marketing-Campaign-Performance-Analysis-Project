
#Nykaa Marketing Campaign Performance Report

1. Introduction
This project analyse the performance of digital marketing campaigns conducted by Nykaa using a simulated dataset sourced from Kaggle. The goal is to evaluate campaign effectiveness across different channels, audience segments, and time periods, and to derive actionable business insights.

2. About the Dataset
The dataset represents marketing campaign data from an e-commerce platform. Each row corresponds to campaign performance metrics tracked across various marketing channels.
Key Features:
•	Campaign ID
•	Marketing Channel (Social Media, Email, Ads, etc.)
•	Impressions
•	Clicks
•	Conversion Rate
•	Cost Per Click (CPC)
•	Total Spend
•	Revenue Generated
•	Return on Investment (ROI)
•	Customer Segment
•	Campaign Duration

3. Data Preparation & Calculated Fields
To enhance analysis, the following calculated fields were created:
•	Revenue per Channel
= Revenue ÷ Channel Count
•	Channel Count
= Number of channels used in a campaign
= LEN([Channel Used]) − LEN(REPLACE([Channel Used], ",", "")) + 1
•	Channel-wise Revenue Allocation
Revenue was distributed across channels using conditional calculations:
Example:
IF CONTAINS([Channel Used], "YouTube")  
THEN [Revenue per Channel]  
END
Similar calculations were applied for Instagram, Google, Email, Facebook, and other channels.

4. Executive Summary
The dashboard provides a comprehensive overview of marketing performance. Overall, campaigns generated strong revenue with a positive return on investment. However, performance varies significantly across campaign types and acquisition costs.

5. Key Metrics Overview
•	Total Revenue: ₹28,65,63,64,282
•	Average ROI: 2.714
•	Total Conversions: 5,73,80,922
•	Total Impressions: 3,06,04,07,471
Insight:
The ROI greater than 1 indicates that the business is operating profitably, reflecting effective marketing strategies.

6. Performance by Campaign Type
•	Top Performer: Social Media
•	Strong Performers: Influencer Marketing, Paid Ads
•	Moderate Performance: SEO
•	Lowest Performance: Email Campaigns
Insight:
Social media campaigns generate the highest revenue and ROI, while email marketing shows relatively weak performance and requires optimization.

7. Channel-wise Revenue Distribution
Revenue contribution is distributed across multiple channels:
•	Instagram
•	YouTube
•	WhatsApp
•	Google
•	Email
•	Facebook
Insight:
•	The distribution is balanced, indicating a diversified marketing strategy.
•	Social platforms like Instagram and YouTube slightly outperform others.

8. Audience Engagement Analysis
Key Observations:
•	Highest Engagement:
o	Bengali – Working Women: 39,649
•	Strong Segments:
o	English – Premium Audience: 39,030
o	Tamil – College Audience: 39,287
•	Consistent Performers:
o	Working professionals across all languages
•	Lower Engagement:
o	Youth segment (especially Tamil audience)
By Language:
•	High: Tamil, English
•	Moderate: Hindi
•	Low: Bengali
By Segment:
•	High: Working Professionals, Tier 2 Cities
•	Low: Youth segment
Insight:
Regional targeting works effectively, especially for Tamil and English audiences. Working professionals are the most responsive group.

9. Campaign Timeline Analysis
•	Revenue remains stable throughout the year
•	A significant drop occurs in June
•	Strong recovery from July onwards
Insight:
The June dip may be due to seasonality or campaign inefficiencies, highlighting an opportunity for improvement.

10. ROI vs Acquisition Cost Analysis
Key Findings:
•	Strong inverse relationship between acquisition cost and ROI
•	Lower cost → Higher ROI
•	Higher cost → Lower ROI
•	Most campaigns cluster around low cost with moderate ROI
•	Some outliers show extremely high ROI at minimal cost
Example Outlier:
•	Campaign: NY-CMP-13007
•	Acquisition Cost: 9
•	Revenue: ₹45,79,910
•	ROI: 74.42
Insight:
Cost efficiency plays a critical role in maximizing returns. High-cost campaigns are not proportionally improving ROI.

11. Key Insights
•	Social media is the most effective marketing channel
•	ROI is highly sensitive to acquisition cost
•	Audience engagement varies by language and segment
•	A mid-year performance dip requires investigation

12. Recommendations
1.	Increase investment in social media and influencer marketing
2.	Optimize or redesign email marketing campaigns
3.	Focus on high-performing segments (working professionals, Tier 2 cities)
4.	Reduce acquisition costs to improve ROI
5.	Investigate and fix the June performance drop
6.	Strengthen regional targeting, especially for Tamil and English audiences

13. Conclusion
Nykaa’s marketing strategy is overall effective, generating strong revenue and maintaining a positive ROI. However, there is significant scope for improvement through cost optimization, better targeting, and enhancing underperforming channels. By leveraging these insights, the company can further maximize marketing efficiency and profitability.

14. Screenshot
![image alt]( https://github.com/Siddharthnegi1/Marketing-Campaign-Performance-Analysis-Project/blob/main/Dashboard.png)



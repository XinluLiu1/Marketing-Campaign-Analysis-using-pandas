# Marketing-Campaign-Analysis-using-pandas
This project utilizes the Pandas library in Python to analyze marketing campaigns and implement A/B testing in an email campaign. The project covers several topics such as basic marketing metrics, marketing channels across age groups, problem-solving in house ads conversion rate, and A/B testing in email campaigns.

The project provides a detailed report outlining the methodology, findings, and actionable insights to help marketing teams optimize their campaigns and increase ROI. The report includes visualizations of the data, as well as explanations and interpretations of the results.

## Project Contents

### Business Understanding
#### Business Problem
Improve the profitability of a marketing campaign
#### Objections
Max Conversion Rate & Retention Rate

### Date Understanding
This marketing campaign dataset contains customer demographics (age, language), conversion information, variant, subscription and cancellation dates, subscribing channel, and retention status.

### Data preparation
1. Updated data column “is_retained”, “converted” to ‘bool’
2. Added new columns for further analysis

### Exploratory Analysis & Summary Statistics
1. Basic marketing metrics
(1) Out of the 7,309 people marketed to, 1,030 subscribed, resulting in a conversion rate of 14.09%. 
(2) Out of the 1030 people subscribed, 696 remained subscribed, resulting in a retention rate of 67.57%.

2. Comparing language conversion rate
The analysis reveals that the conversion rate varies significantly across different languages, with German having the highest conversion rate of 71.62%, followed by Arabic at 50%, Spanish at 20%, and English at 13.12%. This suggests that language preference is an important factor in driving conversions and should be taken into account when designing future marketing campaigns.

3. Comparing daily conversion rate
The daily conversion rate fluctuates significantly between days, with some days as high as 25% and others as low as 5%. There seems to be a general trend of higher conversion rates during weekends, with the conversion rate on Sundays being the highest at 14.18%. The lowest conversion rate during the observed period was on January 31st, at 5.29%. This data suggests that the timing of the marketing campaign may have an impact on the conversion rate.

4. Marketing channels across age groups
(1) Marketing channels are reaching all users equally?
The dataset shows the number of users for different age groups across different marketing channels. The highest number of users in all age groups was through House Ads, followed by Facebook and Instagram. The age group with the highest number of users was 45-55 years across all channels. The age group with the lowest number of users was 0-18 years across all channels.
(2) Whose channel had the best retention rate from the campaign?
- House Ads had the highest conversion rate overall (0.58) followed by Facebook (0.67) and Email (0.72). Instagram and Push had lower overall conversion rates (0.64 and 0.7 respectively).
- There are no discernible patterns in the conversion rates for any particular subscribing channel over the 31-day period. Some channels have higher conversion rates on certain days than others, and vice versa.
- The NaN values suggest that some subscribing channels were not used on certain days, which could potentially be an area for improvement in future marketing strategies.
- It may be beneficial to analyze the demographic characteristics of subscribers across different subscribing channels to identify any trends or patterns that could inform more targeted marketing efforts.

## Problem solve - House ads
The house ads team has become worried about some irregularities they've noticed in conversion rate.- Explore the language problem

(1) What percentage of users were not being served ads in the right language
Based on the given data, the percentage of users not being served ads in the right language varied from day to day. On some days, such as January 1st, 2nd, 6th, and 7th, almost all users (above 98%) were served ads in the right language. However, on other days, such as January 3rd, 4th, and 10th, all users were served ads in the wrong language. On January 11th, only 87.1% of users were served ads in the right language.
These fluctuations suggest that there may be issues with the language targeting system on certain days or that the targeting parameters may need to be adjusted for certain marketing channels or campaigns. It may be beneficial to conduct further analysis to identify the root cause of these fluctuations and implement measures to ensure that users are consistently served ads in the right language.

(2) Estimate what daily conversion rates should have been if users were being served the correct language
Assuming that users were being served ads in their preferred language, the daily conversion rates would have been higher for Spanish-speaking users (by a factor of 1.68), Arabic-speaking users (by a factor of 5.05), and German-speaking users (by a factor of 4.49) compared to the overall conversion rate.
This suggests that serving ads in the appropriate language can significantly impact conversion rates and should be a priority for any multilingual marketing campaign. Additionally, it may be beneficial to further segment the user base based on language preference to create more targeted campaigns and improve overall conversion rates.

(3) Calculate how many subscribers were lost due to mistakenly serving users English rather than their preferred language
The analysis estimates that 32.14 subscribers were lost during the affected period due to mistakenly serving users English instead of their preferred language. This was calculated by multiplying the number of users by the expected conversion rate for each language and subtracting the actual number of subscribers obtained during the period despite the language bug.

## A/B testing in email campaign
Firstly, the control group conversion rate was compared with the conversion rate of a personalized email campaign. The results showed that personalization increased the conversion rate by 38.85%, the personalization is effective in improving the conversion rate in email campaigns.

Secondly, A/B testing was conducted by segmenting the audience based on language and age. The results showed that Spanish-speaking individuals had the highest lift in conversion rate (166.67%) while people aged between 24-30 years showed the highest lift (161.19%). The Spanish-speaking audience and people aged between 24-30 years showed the highest lift, indicating that these segments should be targeted more effectively in future email campaigns.

## Takeaways
1. Serving ads in users' preferred language is crucial to retain subscribers and prevent losses.
2. House Ads targeting should be improved to serve ads in the user's preferred language.
3. Personalization should be implemented in email campaigns.
4. Targeting Spanish-speaking individuals and people aged 24-30 years effectively can result in higher conversion rates.

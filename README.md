# Megaline

I work as an analyst at a telecommunications company named Megaline. The company offers its clients two types of prepaid packages, namely the Surf package and the Ultimate package. The advertising department wants to know which prepaid package generates more revenue, so they can create an appropriate advertising budget. You will conduct an initial analysis of these prepaid packages based on a relatively small sample of 500 Megaline clients. The dataset includes information such as who they are, where they come from, which package they use, and the number of calls and messages they sent in the year 2018.

## Goals
This project has two main objectives:
1. Analyzing consumer behavior for each package provided by Megaline.
2. Analyzing which prepaid package generates more revenue.

## Steps

This project will consist of few steps:

1. Import and initial examination of the data.
2. Data transformation to prepare for analysis.
3. Analysis of calls, messages, and internet usage.
4. Comparison of revenue between Surf and Ultimate packages.
5. Hypothesis testing to validate analysis results.
6. Conclusion and recommendations based on findings.

## Description of Data

This project contain 5 dataset:

- Table: users (user data):

  - `user_id`: User ID
  - `first_name`: User's first name
  - `last_name`: User's last name
  - `age`: User's age (years)
  - `reg_date`: Subscription start date (dd, mm, yy)
  - `churn_date`: Date when the user stopped using the service (if the value is missing or absent, it means the service is still in use when this data was created)
  - `city`: User's city of residence
  - `plan`: Phone plan name

- Table: calls (call data):

  - `id`: Unique web session ID
  - `call_date`: Call date
  - `duration`: Call duration (in minutes)
  - `user_id`: User ID making the call

- Table: messages (SMS data):

  - `id`: Unique SMS ID
  - `message_date`: Date the SMS was sent
  - `user_id`: User ID sending the SMS

- Table: internet (web session data):

  - `id`: Unique web session ID
  - `mb_used`: Volume of data consumed during the session (in megabytes)
  - `session_date`: Web session date
  - `user_id`: User ID

- Table: plans (phone plan data):

  - `plan_name`: Phone plan name
  - `usd_monthly_fee`: Monthly fee in US dollars
  - `minutes_included`: Monthly allocated call minutes
  - `messages_included`: Monthly allocated SMS
  - `mb_per_month_included`: Monthly allocated data volume (in megabytes)
  - `usd_per_minute`: Price per minute if exceeding the allocated plan limit (e.g., if the plan has an allocation of 100 minutes, usage starting from the 101st minute will incur a charge)
  - `usd_per_message`: Price per SMS if exceeding the allocated plan limit
  - `usd_per_gb`: Price per extra gigabyte of data if exceeding the allocated plan limit (1 GB = 1024 megabytes)

## Conclusion

The data analysis confirms our initial hypothesis, revealing notable differences in revenue between the Surf and Ultimate plans, as well as variations in earnings between users from the NY-NJ region and those from other areas. A detailed visualization illustrates a consistent monthly increase in Surf plan users, suggesting its cost-effective structure resonates well across regions. While factoring in additional charges for exceeding Surf plan limits increases overall earnings, a closer examination emphasizes the Ultimate plan's superior profit-generating capability. In conclusion, strategically allocating the advertising budget toward the Ultimate plan is recommended due to its potential for higher revenue compared to the Surf plan.

## Future Work

For future analysis, it would be beneficial to:

- Expand the dataset to include a larger sample size for more robust insights.
- Explore user preferences and satisfaction through surveys or feedback collection.
- Investigate regional variations in user behavior and plan preferences.
- Implement predictive modeling to forecast revenue trends and customer churn.





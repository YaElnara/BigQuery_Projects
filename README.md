# BigQuery

## Data Preparation for BI Reporting [\[Link\]](https://console.cloud.google.com/bigquery?sq=162602427492:d3d17f1fcbed48cc92edd34211fcc890)
 - Generated a table with event, user, and session information from GA4 for 2021.
 - Included fields such as `event_timestamp`, `user_pseudo_id`, `session_id`, `event_name`, `country`, `device_category`, `source`, `medium`, and `campaign`.
 - Filtered the data to include specific event types like session start, product view, add to cart, begin checkout, add shipping info, add payment info, and purchase.

## Conversion Calculation by Date and Traffic Channels [\[Link\]](https://console.cloud.google.com/bigquery?sq=162602427492:7a826dd5697a41eb939ac76123ac7f99)
 - Created a table to analyze conversion metrics from session start to purchase.
 - The table includes `event_date`, `source`, `medium`, `campaign`, `user_sessions_count`, `visit_to_cart`, `visit_to_checkout`, and `visit_to_purchase`.
 - Calculated unique session counts by considering both session and user identifiers.

## Conversion Comparison Between Different Landing Pages [\[Link 1\]](https://console.cloud.google.com/bigquery?sq=162602427492:fc17b2cba51c482b88d8bd753172bc1b) [\[Link 2\]](https://console.cloud.google.com/bigquery?sq=162602427492:5cdbb80c7bc947e5a7f726f575efeef3)
 - Extracted `page_path` from `page_location` in session start events for 2020.
 - Calculated metrics such as the number of unique sessions by unique users, the number of purchases, and the conversion rate from session start to purchase for each unique landing page.
 - Linked session start events with purchase events using user and session identifiers.

## Correlation Between User Engagement and Purchases [\[Link\]](https://console.cloud.google.com/bigquery?sq=162602427492:4ea906f9cc2c4ed4a8454dd0f2d76aff)
 - Determined user engagement during each session by checking if `session_engaged` was ‘1’ and calculating the total activity time from `engagement_time_msec`.
 - Identified whether a purchase occurred during the session.
 - Calculated the correlation coefficient between user engagement and purchases, and between total activity time and purchases.


# Summary

By completing these tasks, I gained valuable experience in preparing and transforming data from GA4 for BI reporting, calculating conversion metrics across various traffic channels and dates, comparing conversion rates between different landing pages, and analyzing the correlation between user engagement and purchases. I learned how to construct efficient SQL queries to extract, aggregate, and analyze large datasets. Additionally, developed skills in linking user interactions to meaningful business outcomes, providing actionable insights for optimizing marketing strategies.








# data-512
### The goal of this project is to "construct, analyze, and publish a dataset of monthly traffic on English Wikipedia from January 1 2008 to August 30 2020". Through the process of creating this dataset and perfomring the analysis, we will learn the best practices for data curation with the ultimate object being providing reproducible analysis and research.

The data is acquired from APIs provided by Wikimedia through 2 endpoints: 1. a legacy pagecounts API endpoint and 2. a pageviews API endpoint.

The legacy pagecounts endpoint is available here: https://wikimedia.org/api/rest_v1/#!/Pagecounts_data_(legacy)/get_metrics_legacy_pagecounts_aggregate_project_access_site_granularity_start_end 

The legacy pagecounts API documentation is available here: https://wikitech.wikimedia.org/wiki/Analytics/AQS/Legacy_Pagecounts

The pageviews API endpoint is available here: https://wikimedia.org/api/rest_v1/#!/Pageviews_data/get_metrics_pageviews_aggregate_project_access_agent_granularity_start_end The pageviews API documentation is available here: https://wikitech.wikimedia.org/wiki/Analytics/AQS/Pageviews

In my final data file, titled 'en-wikipedia_traffic_200801-202008.csv' the datafields and their definitions are as follows:

year = the year the datapoint is associated with (taken from the first 4 characters of the timestamp)
month = the month the datapoint is associated with (taken from the 4-6th character of the timestamp)
pageview_desktop_views = the number of page views from users using desktop client
pageview_mobile_views = the number of page views from users using a mobile client (can be either mobile web or mobile app)
pageview_all_views = the number of page views from users using both mobile or desktop clients
pagecount_desktop_views = the number of pagecounts from the legacy API of users using the desktop client
pagecount_mobile_views = the number of pagecounts from the legacy API of users using the mobile client
pagecount_all_views = the number of pagecounts from the legacy API of users using either the mobile or desktop client



### Known Issues: One known issue is that the different data sources and APIs have variable amount of data coverage. As such, we have an incomplete picture of usage in the desired time range. Another consideration to make is that the Pageview API excludes spiders/crawlers from the data that the Pagecounts API does not explicitly exclude.

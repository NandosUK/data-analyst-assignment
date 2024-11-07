# Nando's Data Analyst Assignment

As a organisation we are always looking to be data informed and use our skills and data to provide clear and concise information to help answer business questions and optimise how things work.
This task is looking to understand your coding and presentation skills and how you infer and show action-orientated insight.

This assignment should take about an hour to complete.
The queries that you write should be of production quality, code you are proud of and with consideration of future maintenance that could be done by another team.

For each question write the code that you've written and any comments or documentation that you think might be useful to help someone understand the data.
You can present your solutions in any preferred format; please email them to your interview contact at least 24 hours before the scheduled interview.


## Prerequisites

This assignment requires Google Cloud BigQuery access, which can be used for free via [the BigQuery sandbox instructions](https://cloud.google.com/bigquery/docs/sandbox).

Note that the free access tier granted by following these instructions includes 1TB of queried data per month. The largest table that you will query is 7.47 GB.


## The Data Source

Citibike is a bike rental scheme popular with commuters for getting around New York City in the USA.
Bikes can be collected and dropped off at different locations (called "stations").
The data for Citibike is stored in two public BigQuery tables:
 - `bigquery-public-data.new_york_citibike.citibike_trips` - a list of trips taken on Citibikes
 - `bigquery-public-data.new_york_citibike.citibike_stations` - a list of Citibike stations

You can view and explore these tables via [the BigQuery `new_york_citibike` dataset page](https://console.cloud.google.com/bigquery?p=bigquery-public-data&ws=!1m4!1m3!3m2!1sbigquery-public-data!2snew_york_citibike).


## Questions

You've been tasked with identifying which Citibike stations could be given more bikes to meet peak demand, as sometimes riders complain that there are no bikes available at their preferred station.

1. Write a query to return the ten stations that had the most starting journeys on 2018-04-18. The output should include each station's name, the number of bikes available at each station, and each station's busiest hour for starting journeys on that day.

2. Assuming that each station is fully restocked to have `capacity` bikes at midnight daily, which of the ten stations from question 1 do you think is the best candidate?
Use `bigquery-public-data.new_york_citibike.citibike_trips` to track bikes as they are taken and returned from each station to help with your answer.
Write a query to calculate this.
Don't use any machine learning algorithms to answer this question.

3. Please put together one or two slides (or similar presentation method) to display some information/trends and derive other insight and some recommendations that will help Citibike.
This presentation should be time-limited to a maximum of two minutes.

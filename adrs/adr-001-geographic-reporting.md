# Geographical trend

Date: 2021-10-27

## Status

Accepted

## Context

A Geographical trend analysis is needed to help Farmacy Family know what type of food to deliver food to specific fridges. Each geography or neighborhood may prefer difference dishes than another. By having a good geographical understanding of each areas wants in terms of food we can better provide those fridges with the dishes that will be better received by the community.

## Decision

We will use [Looker](https://www.looker.com) and Big Query from Google. Looker already provides geographical views for us to use. Looker will continuously improve over time as it is releasing new versions. Big Query allows us to ingest a large amount of data from all the fridges or POS systems, for example, information about a transaction that is just made. Looker will be able to query this data to show a clear picture of what food choices are being made across different areas.

To help with engagement the fridges will be able to query BigQuery as well to provide information to the customers. The fridges will provide a quick poll to the users after their purchase about what meals they would like to see more of. The options to this poll will be populated with dish names that are becoming popular to the area. This data is retrieved from BigQuery. 

## Consequences

Looker will have a steep learning curve to fully understand and integrate. Looker is not free and comes with a subscription cost.
# Farmacists

## Narative

Farmacy Foods is a grocery retailer that wants to expand its offering to be more personal and innovative. They are calling this offering Farmacy Family and want to utilitize customer profiles to engage users by being a part of a food community.

Many modern architectures use existing services in the appropriate space for bringing new solutions online. For example, using Atlas for Mongo DB, Microsoft Vision for object recognition, and Facebook for social interaction would all be considered efficient and modern solutions for bringing a new system online.

Farmacy Foods is a retailer, specifically a food retailer. The largest provider of grocery store software and services is NCR. Utilizing the NCR Business Services Layer (BSL), this solution will illustrate a practical way to meet all of the requirements of Farmacy Family with a minimum of new services to create.

Because the primary focus of this extension on Farmacy Food is consumer engagement, the NCR Consumer Data Manager (CDM) service will be utilized. By having users add their information into CDM, their food preferences, address and demographic info can be known. The NCR Security Service will provide authentication and Role-Based Access Control (RBAC) to give proper permissions for data. This allows health professionals to see data that others cannot.

For a forum, local Facebook groups will be created which will give a sense of community without needing to create a forum service from scratch. Links to these are provided from the main portal based on browser location.

For analytics, the Google Looker platform is leveraged to show data with flexible geographical views.

To interact via messages with an edietiton, the email address from NCR CDM can be used. Facebook messaging is also an option.

Custom software and services will be created only where it is absolutely needed, with the majority of this solution leveraging existing systems.

The 'seamless' interaction with the existing system, 'Farmacy Food', is accomplished through the Transaction Document Manager (TDM). By submitting completed transactions to this system, NCR analytics can combine the dimensions and measurements from food family (community) with the existing system (transactions).

## Solution Summary

## Requirement

• Add a new system to manage customer profiles, allowing community 
engagement, personalization around preferences and dietary needs

## Solution

A Front end UX design was created to show customer interaction with a web site hosted in our Kubernetes engine. When users enroll with this system, they will be tracked in the Customer Data Manager (CDM). When preferences and personalition options are chosen, the NoSQL format of Firestore is leveraged allowing for flexible data to be stored.

## Requirement

• Support geographical trend analysis to hone Farmacy Family’s ability to 
optimize the foods delivered to fridges (an additional integration point TO 
Farmacy Foods)

## Solution

When transactions are submitted to TDM from Farmacy Foods, that data is crossed with Customer data from CDM and Firestore that shows how purchasing behaviors align. This data is submitted to a data lake for large-scale long term storage. Based on on this data, Looker can generate views that show geographical data between the food items an categories purchased and the locations they were purchased from. Based on the Looker dashboards, better decision can be made for delivering food to fridges.

## Requirement

• Support both push and pull models for community engagement. In other 
words, Farmacy Family will manage forums,emails, and create connections 
between similar demographics. Farmacy Family needs transactional member 
information for outreach purposes. The engagement model includes 
subscriptions, forums, reference material, class information, and other media 
that supports Food-as-medicine

## Solution

With data collected around similar food purchasing behaviors, groups can be formed from the Looker data. The groups of people can be collected into a social media platform of choice using data from the Customer Data Manager (CDM).

# Farmacists

## Narative

Farmacy Foods is a grocery retailer that wants to expand its offering to be more personal and innovative. They are calling this offering Farmacy Family and want to utilitize customer profiles to engage users by being a part of a food community.

Many modern architectures use existing services in the appropriate space for bringing new solutions online. For example, using Atlas for Mongo DB, Microsoft Vision for object recognition, and Facebook for social interaction would all be considered efficient and modern solutions for bringing a new system online.

Farmacy Foods is a retailer, specifically a food retailer. The largest provider of grocery store software and services is NCR. Utilizing the NCR Business Services Layer (BSL), this solution will illustrate a practical way to meet all of the requirements of Farmacy Family with a minimum of new services to create.

Because the primary focus of this extension on Farmacy Food is consumer engagement, the NCR Customer Data Manager (CDM) service will be utilized. By having users add their information into CDM, their food preferences, address and demographic info can be known. The NCR Security Service will provide authentication and Role-Based Access Control (RBAC) to give proper permissions for data. This allows health professionals to see data that others cannot.

For a forum, local Facebook groups will be created which will give a sense of community without needing to create a forum service from scratch. Links to these are provided from the main portal based on browser location.

For analytics, the Google Looker platform is leveraged to show data with flexible geographical views.

To interact via messages with an edietiton, the email address from NCR CDM can be used. Facebook messaging is also an option.

Custom software and services will be created only where it is absolutely needed, with the majority of this solution leveraging existing systems.
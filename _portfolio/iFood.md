---
title: "1. iFood"
excerpt: "Descriptive analysis of iFood's Marketing Campaings data <br/><img src='/images/ifood-campaigns.png'>"
collection: portfolio
---

# iFood

A descriptive analysis of a dataset containing Marketing Campaigns from the app iFood.

## What is the data, and where does it come from?

The dataset consists of 2206 customers of the company with data on customer profiles, product preferences, campaign successes/failures and channel performance. It is available as a GitHub repo as well as a Kaggle kernel, in a csv format. Also, there was a dictionary in a png image format, describing many variables.

## What's the problem here?

There was no specific business demand; instead, we were encouraged to explore and describe the data, and find our own insights within it. (This has been used in the past as part of the hiring process for the company, but we only discovered it much later).   

## How was the solution planned?

We were free to choose methods and tools. As part of the initial look into the dataset, the csv was loaded onto a Google Sheets spreadsheet. Ultimately, we felt no need to change tools. The focus was onto what to approach, and how to present the data. So we were planning as we went exploring. 

While exploring, the nature of the data and the perceived value from performance indicators and initial variables suggested a power law approach. The curve of value spent by customers brought the realization that a small percentage of customers accounted for a very large amount of revenue. In addition, the title of the dataset itself (as well as campaign acceptance variables) drew more attention to marketing, and therefore to the success or failure of marketing campaigns. Thus, we planned a Pareto analysis using the 80/20 rule, but this was not accurately verifiable in the analysis: 80% of revenue came from almost 40% of customers, while 20% of customers brought in almost 54% of revenue. We opted for the second alternative, believing that, since 1/5 of customers brought in more than half of the revenue, the scope would be more precise for data learning and actionable variables.

The data came from marketing campaigns. Thus, we imagined a goal: to improve the performance of the marketing department. This department wants to generate more purchases, and larger purchases, and wants its campaigns to be successful. So what is the profile of the customer who generates these larger and/or more frequent purchases? And what is the impact of the marketing campaigns already carried out? We therefore sought to extract answers to these questions from the 20% of customers who brought in the most revenue. So, imagining a Fact, it would be the total amount spent by a user in the period between the first and last campaign.

## And the solution itself, how was it executed?

We categorized the many available variables into “Customer characteristics” (age, salary, relationship), “Products and values” (purchases of wine, meat, vegetables), “MKT campaigns” (acceptance or rejection of a given campaign), “Customer actions” (purchases, visits, reports), and total amount spent. If we want the 20% of [fact] with the greatest influence on [dimension], then we want the 20% of [customers with the highest spending] that influence [actionable dimensions by those who requested it] the most; in this case, marketing.

We consider relationship status, age, number and type (child, teenager) of children at home, web visits, length of time as a customer, purchases of wine, fruit, meat, fish, and sweets to be actionable variables.

In the end, the average profile of our best customers is: They are between 40 and 70 years old, are in a relationship, and have no children at home (or at most one); They have been registered on the platform for 6 or more years and visit the website* at most 3 times a month; They spend between $500 and $1,000 on wine and between $250 and $750 on meat, but less than $100 on fish, fruit, and sweets; They did not accept any of the last 6 campaigns, or at most one: most likely Campaign 5 or 6 (out of a total of 6 campaigns).

The data was organized into graphs and a Google Presentations presentation [is available with the full report](https://docs.google.com/presentation/d/1hhrehqbdsP8Nds4t8JDCsnoJY1s5WTcutgenPmkPaa8/).

## Conclusion? Difficulties? Future work?

We observed that the absence of children and the presence of relationships point to stable, long-term couples with good joint purchasing power. These high-paying customers are already loyal: for the most part, they do not depend on campaigns, but are still very attracted to them. And purchases of wine and meat contribute significantly to the final result.

It would be desirable to encourage other teams to expand the customer base within the average profile found, and meat and wine can be prioritized in this expansion. It is also worth looking at campaigns 2, 3, and 4, and understanding their focus and the reason for the results, while campaigns for purchases of fish, fruit, and sweets should be reviewed (in light of the indicators).

The biggest difficulty was deciding how to approach the analysis itself. Segmentation by power law does not always work; it depends on the case. It took some time to decide on a Pareto distribution approach -- or something close to it, which is what happened.

At the time of publication of this analysis, the database had not been updated for several years. If it were possible to access updated data in another way (with someone else uploading it, for example), it would be possible to run a longer analysis, i.e. with a larger client database, or with more campaign variables, or a bigger variety of products.




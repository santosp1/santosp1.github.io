---
title: "Portfolio item number 2"
excerpt: "Short description of portfolio item number 2 <br/><img src='/images/dashboard_olympic.png'>"
collection: portfolio
---

# Olympic Games analysis

A descriptive analysis of a dataset containing participants and medal winners from the Modern Olympic Games, from their inception in 1896 to the 2016 Olympic Games in Rio de Janeiro.
What is the problem here?

There is a business problem, a demand sent in from the editorial manager of a media and press company. The demand and a brainstorm/overview of it are in the business-demand-news file.

In short, there is a request to generate a data visualization that would help readers understand the historical performance of countries at the Olympic Games, with the possibility of selecting their own country. Additional details about competitors are also interesting, as well as any other insights the analyst might find.

## How was the solution planned?

The data came from a .bak file: a backup of a SQL Server database. This already implies the use of this database manager. As the main objective was data visualization, we needed a tool for this. We therefore decided on Power BI, remaining on a Microsoft stack. So, the solution would involve the usual pre-processing (cleaning, transformation, preparation) of the data, selecting the relevant columns, transforming what was necessary, and generating an SQL that would arrive at the desired result. From there, a .csv would be extracted for Power BI and the visualization created in it, and if necessary DAX would be used to refine the values.

## And the solution itself, how was it executed?

<img src='/images/dashboard_olympic.png'>

The database backup was loaded into SQL Server by copying the file to the directory where it can be accessed (depending on the version of SQL Server Management Studio). There, SQL queries investigated the database, which has two tables, one of which is just the nation code and subsequent name, and another table with all the other data: athlete's name, id, nation code, sport, the category they competed in, the Olympics they took part in, the medal they received (or not), and others.

The .csv generated was imported into Power BI. On the left of the dashboard, there are slicers for selecting the season (summer or winter Olympics), year of the games, country, competitor and sport. The first variable has exclusive items, so always one, and only one, is active; the other options in the other variables can be all, some or none.

We used DAX to calculate the total number of competitors, medal winners, and the breakdown by gender, and included them in cards and pie charts. Bar charts show the medals by sport, by competitor and by age group, and an area chart shows the timeline of total medals since the first Olympics, broken down by medal and by year.

## Difficulties? Future work?

The database is incomplete in many ways. It's 2024, we've already had the 2018 and 2022 Winter Olympics, and the 2020 Summer Olympics (in 2021, due to the pandemic) but the data stops at 2016. In addition, in team sports not all athletes are present as medal winners. Some names are also missing characters, especially letters with accents.

One difficulty with this first iteration was deciding on the number of medals. In the overall medal table, the allocation is by event. So, for example, field soccer gives one medal. But in the current version, each athlete registered in the database as a medalist counts one medal for their country.

In a future version, each event will be filtered to correct these differences. Both the medal allocations per country and the individuality of each medal-winning athlete. They will be counted differently, and displayed on the dashboard in different places.

The first table in the database didn't prove to be really useful in principle because the many country name changes make it difficult to assign today. For example, an athlete from the former Yugoslavia or the Soviet Union has no information (such as city of origin) in this database to link him to the current country, and only if desired can the historical medal series be retraced.

Exploring other databases can help with this issue, as can correcting medals by sport and athlete. DAX formulas are also an option for dealing with this directly in Power BI.
---
title: "911 Calls"
excerpt: "Descriptive analysis of Montgomery County's 911 calls <br/><img src='/images/911-outliers.png'>"
collection: portfolio
---

# 911 Calls

An exploratory analysis of the dataset containing 911 call information in Montegomery County. This project was completed as part of an online data science course.

## What is the data, and where does it come from?

The database contains information from Montgomery County 911. The data is public, available in a Kaggle kernel in csv format. 

## What's the problem here?

The project is part of an online course, so some of the tools were already included, or were implicit. There is no specific problem pointed out by the person in charge of the database or the course instructor; the idea is to explore the database and extract information, generate insights, build visualizations and enable others to learn more about the data in order to make a decision. 

## How was the solution planned?

The proposition is to build the solution from a Jupyter Notebook, using Python and Numpy, Pandas, Matplotlib and Seaborn libraries. This set of tools enables data loading, pre-processing (cleaning, transformation, preparation), as well as modeling and visualization. From those come insights, the search for extra information and interpretations of phenomena found. Other tools and processes can be used to contribute to this objective.

This choice of programming language and tools also counts as a project premise; since they are considered part of the course's learning, it would not be ideal to go down a different path.

## And the solution itself, how was it executed?

As the proposition was to make a Jupyter Notebook, exploratory analysis would bring discoveries from each verification of the data. The solution was built in blocks of lines of code, interspersed with the resulting visualization (be it an image or other information from aggregated data), the interpretation of what was executed and, if applicable, the overall impact on the project, or a follow-up to the next section.

From what was loaded from the csv into a Pandas DataFrame, the analysis both created visualizations and manipulated and transformed data. Initially, it was found that there was missing data, but throughout the analysis this did not prove to be an impediment. Columns were broken down into others and new ones created -- such as creating `reason` ("category") from `title` ("full description of the call") and date, time, day of the week and month columns from `timeStamp`. 

Bar graphs were created to quantify `reason` in general numbers, as well as looking at the total number of calls (separated by category) per day of the week, per month of the year, per year and for all the months in the dataset. Line graphs were also drawn to look at calls per month (both total and separated by category), as well as the respective trend analysis linear regressions. Finally, outliers were investigated by drawing linear graphs based on days, obtaining interesting findings (in particular, 3 major days of severe weather events), and heatmaps and clustermaps for different visualizations.

## Difficulties? Future work?

At the time of publication of this analysis, the database had not been updated for several years. If it were possible to access updated data in another way (with someone else uploading it, for example), it would be possible to run a longer analysis, i.e. over a wider time range of records.

It would also be possible to use other libraries instead of existing ones. For example, Polars instead of Pandas. Or even another programming language, such as R, but this would be outside the scope of the project.

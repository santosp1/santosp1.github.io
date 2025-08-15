---
title: "3. Freight in Brazil"
excerpt: "A quick analysis based on a set of product freight data <br/><img src='/images/excel_analysis_freight.png'>"
collection: portfolio
---


# Freight in Brazil

A quick analysis based on a set of data on product freight, with the aim of generating a final PDF report with data graphs and short paragraphs of text. 

## What is the data, and where does it come from?

The source of the data is an Excel spreadsheet, with information about product freight, with prices, locations, dates and other identifications.

## What is the problem here?

There is no specific problem pointed out by the person responsible for the database or the course instructor; the idea is to explore the database and extract information, generate insights, build visualizations and enable others to learn more about the data in order to make a decision.

## How was the solution planned?

The proposition was to use Excel's own functionalities. I realize from observation that many people would use Power Query and pivot tables; I would probably do the same. However, encouraged by the project's creator, only standard Excel functions such as sum, average and count would be used. Finally, Excel itself would also be used to generate a PDF report.

## And the solution itself, how was it executed?

From the first tab, containing raw data, a copy was made to start cleaning the data. There, the display of dates (order, purchase, dispatch and delivery) and freight prices was corrected, and the Sistema column was removed. I also created a month column to isolate this data.

For the analysis, a new tab was created and we used functions to calculate the desired metrics. Total overall freight; by state, the total value, the average, the highest and lowest, as well as the amount of freight, and the variation in delivery days - the fastest, the longest, and the average; by month, the total, the average, the amount; by SKU, total and average freight values, and the amount of freight; and the percentage by payment method. 

A new tab with the metrics calculated, and I generated graphs. Here I fumbled a bit with how to represent them: bar, pie chart, line and others, until I found a visually pleasing solution. Finally, a PDF report was generated with short paragraphs describing each graph.

## Difficulties? Future work?

This was my first analysis using Excel. I'm used to programming (Python, in particular), and although Excel is quite powerful, I was afraid of running into some limitations in the analysis. This wasn't the case; for this dataset, the functions covered a good part of what they were intended to analyze. My biggest limitation was in visualization: my own lack of storytelling and aesthetics knowledge. That fear became doubt as to whether the graphics were legible, not too congested, and if they could really tell the story of the data. 

Another difficulty was generating the PDF itself. The initial idea was to use Excel itself to generate a quick PDF, but it didn't turn out to be quick at all. Page breaks are often confusing and adding or removing text changes the whole layout. I preferred to use Word instead, so as not to waste too much time. 

For the future, I thought it would be interesting to work with Excel in this way. Although I don't see too many job listings requiring Excel as high priority, it's still well used for quick analysis. I think I can do something exploring more advanced functionalities, such as pivot tables, Power Query, or even code. As well as Copilot integrated into Microsoft tools, and Python itself.
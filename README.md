# Kickstarting with Excel

## Overview of Project

### Purpose

The following analysis was performed to provide Louise, who is interested in raising funds for her play, with insight into fundraising campaign outcomes based on factors such as the launch date of the campaign and the fundraising goal of the campaign.  This analysis was based on a Kickstarter data set of 1,413 campaigns launched between 2009 and 2017 across various fundraising categories and in multiple countries. Specific analyses in this report may have used a smaller segment of the population data to derive more targeted insights.
  
## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date

An initial analysis of campaign outcomes based on launch date was prepared. To prepare the Kickstarter dataset for this analysis:

- the 'launched_at' date in unicode format from the original Kickstarter data set had to be converted to a human-readable date.  This was accomplished by adding a new column called 'Date Created Conversion' using the formula `=J2/60/60/24 + DATE(1970,1,1)` where 'J2' refers to the date field in unicode format.

- to enable the final analysis to be able to be filtered by launch year, an additional calculated column called 'Years' was added using the formula `=YEAR(S2)` where 'S2' refers to the 'Date Created Conversion' field.

A pivot table was created based on the enhanced Kickstarted data, with filters for 'Parent Category' and 'Years', and with the count of outcomes displayed by 'Outcome' in the columns and by month of launch date in the rows.  As we were only concerned with completed campaigns, the 'Live' campaigns were filtered out of the Outome columns. The 'Parent Category' was filtered to 'theater' which is the category most relevant to Louise, as she considers her campaign to fund a play.

At this point the data for the analysis was displayed in tabular form, but to enable more visually intuitive understanding of the data, a line chart was created:


### Analysis of Outcomes Based on Goals

### Challenges and Difficulties Encountered

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

- What can you conclude about the Outcomes based on Goals?

- What are some limitations of this dataset?

- What are some other possible tables and/or graphs that we could create?

# launch_month
Analysis of data by month

ANALYSIS METHODS

EXCEL
Downloaded Google spreadsheet
Used "month" function to read month from "Date of Contact" column
to create new column - Month
Formatting - changed month number to text using formula =TEXT(DATE(2011,E988,1),"MMM")
Inserted pivot table - counted months.
Observation: October is the month with the highest number of contacts
Conclusion: Coming of summer (August) in the lead up to fall (October) 
is the time when contacts increase most for the whole year. 

Is there a difference between years? Is one year skewing the data? 
I created a new column of "Year" using 'year' function to read year from 
"Date of Contact" column
Inserted pivot table "yearly_pivot" counts by month, grouped by year
Observation: The trend for fall leadup increase was obvious for each of the years
Conclusion: Client contacts has consistently increased every year coming into the fall

Visualization
I included a simple line graph to demonstrate the total number of contacts by month
across all years - see monthly_pivot

I also included a cool radar graph to show the spike in contacts in fall months for each year
- see 'yearly_pivot' tab. 

PANDAS
Saved Google spreadsheet as a CSV file
Imported CSV file to Pandas
Read file and loaded into a dataframe
Extracted month names from the "Date of Contact' column
Observation: October is the month with highest number of contacts

Is October the most popular month every year? 
To answer this, the year value was extracted from 'Date of Contact' then
the number of contacts by month by year was counted.
Observation: Although slightly complicated looking, the result clearly shows that 
October is popular every month.

I illustrated the results with two simple graphs
1. Plot of total number of contacts by month
2. On a five year axis, the total number of contacts by month

Observation: The time arranged total contacts show a new trend that has not been obvious
from other graphs, and that is a trend downwards every October. From the first year, the 
number of contacts in October was around 60, and by 2017 that number was down to 40. 

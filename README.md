# UFOs
## Overview
Dana’s webpage and dynamic table are working as intended, but she’d like to provide a more in-depth analysis of UFO sightings by allowing users to filter for multiple criteria at the same time. In addition to the date, you’ll add table filters for the city, state, country, and shape. Include a write up.
## Deliverable 1
• in [index.html](https://github.com/jzebker/UFOs/blob/main/index.html), the search button has been removed and there are ***five*** options for filtering the search form
<p align="center">
  <img src="https://github.com/jzebker/UFOs/blob/main/readmepics/D1nobutton.png?raw=true" alt="HTML Form" width="500">
</p>

• in [app.py](https://github.com/jzebker/UFOs/blob/main/static/js/app.js), the event listener detects changes in each search filter
<p align="center">
  <img src="https://github.com/jzebker/UFOs/blob/main/readmepics/D1eventlistener.png?raw=true" alt="Event Listener" width="500">
</p>

• in [app.py](https://github.com/jzebker/UFOs/blob/main/static/js/app.js), the **updateFilters()** function saves the element, value, and id
<p align="center">
  <img src="https://github.com/jzebker/UFOs/blob/main/readmepics/D1updatefilter.png?raw=true" alt="updateFilters()" width="500">
</p>

• in [app.py](https://github.com/jzebker/UFOs/blob/main/static/js/app.js), the **filterTable()** function loops through the filters and keeps data that matches the filter values
<p align="center">
  <img src="https://github.com/jzebker/UFOs/blob/main/readmepics/D1filtertable.png?raw=true" alt="filterTable()" width="500">
</p>

• the webpage filters the data based on user input, an example for City - "Benton" follows
<p align="center">
  <img src="https://github.com/jzebker/UFOs/blob/main/readmepics/D1webpage.png?raw=true" alt="filterTable()" width="500">
</p>

## Deliverable 2
### Results
***Using the website to filter the table:***

(1) Scroll down to the table

(2) Enter your search criteria in the provided form
<p align="center">
  <img src="https://github.com/jzebker/UFOs/blob/main/readmepics/D2emptyform.png?raw=true" alt="Empty Search Form" width="500">
</p>

(3) The table updates on user input into one or more of the search form fields (the example below shows the table filtered by date = "1/8/2010" and state = "tx")
<p align="center">
  <img src="https://github.com/jzebker/UFOs/blob/main/readmepics/D2datecityfilter.png?raw=true" alt="filterTable()" width="500">
</p>

(4) To reset filters reload the page or empty the search form fields
### Summary
***Drawbacks:***

• user input must match data values within the table ***exactly*** in order for it to appear in the filtered table

• the data is difficult to search because (specifically in the **Shape**, **Duration**, and **Comments** columns) it is inconsistent in format and/or spelling
<p align="center">
  <img src="https://github.com/jzebker/UFOs/blob/main/readmepics/D2inconsistentformat.png?raw=true" alt="filterTable()" width="700">
</p>
<p align="center">
  <sub>Durations are not reported in a consistent format and various typos exist in the data.  Defined shapes do not always correspond to the same shape.</sub>
</p>

• the data itself is sparse but we can't really do anything about that in this case (ex: short period of time, only from USA etc)

***Suggestions for further improvement/development:***
• lighten and italicized placeholders in filter search input fields for better contrast between input and placeholders, an example is below

• make a drop down menu instead of text input for the **Shape** column; this allows the user to see what he/she should be searching for in a column with limited options

• write a function to clean the **Duration** column and make it of a searchable format; this will allow the user to search the duration column with text matching

• change the **filterTable()** function so that it finds data from ***inexact*** text matches in addition to ***exact*** text matches

• make the website prettier

• make an alert if the search returns no results

• add start date stop date in filter

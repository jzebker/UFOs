# UFOs
## Overview
Dana’s webpage and dynamic table are working as intended, but she’d like to provide a more in-depth analysis of UFO sightings by allowing users to filter for multiple criteria at the same time. In addition to the date, you’ll add table filters for the city, state, country, and shape. Include a write up.
### Deliverable 1
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

### Deliverable 2
#### Results
**Using the website to filter the table:**

(1) Scroll down to the table

(2) Enter your search criteria in the provided form
<p align="center">
  <img src="https://github.com/jzebker/UFOs/blob/main/readmepics/D2emptyform.png?raw=true" alt="Empty Search Form" width="500">
</p>

(3) The table will update when the user enters input into the search form (works with multiple filters, to reset filters reload the page or empty the search form fields - the example below shows the table filtered by date = "1/8/2010" and state = "tx")
<p align="center">
  <img src="https://github.com/jzebker/UFOs/blob/main/readmepics/D2datecityfilter.png?raw=true" alt="filterTable()" width="500">
</p>

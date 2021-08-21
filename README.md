# UFOs
## Overview
Dana’s webpage and dynamic table are working as intended, but she’d like to provide a more in-depth analysis of UFO sightings by allowing users to filter for multiple criteria at the same time. In addition to the date, you’ll add table filters for the city, state, country, and shape. Include a write up.
### Deliverable 1
• the search button has been removed and there are ***five*** options for filtering the search form in the [index.html](https://github.com/jzebker/UFOs/blob/main/index.html) file
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

• in [app.py](https://github.com/jzebker/UFOs/blob/main/static/js/app.js), the **filterTable()** function loops through the filters (user input) and keeps data that matches the filter values
<p align="center">
  <img src="https://github.com/jzebker/UFOs/blob/main/readmepics/D1filtertable.png?raw=true" alt="filterTable()" width="500">
</p>

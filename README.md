# UFOs
### Overview

This repository has the code that creates a table dynamically based on [this dataset](static/data.js). The page allows the users to filter the table data for chosen values. The technologies used are HTML, JS and CSS and the libraries are Bootstrap and D3.js.


### Result: Webpage

This is a responsible web page with a table that is loaded dynamically from data out of an array located in *data.js*. We use D3.js and a custom made function **buildTable** to load the data.
In the HTML there is a form to let the user enter the filter he/she wants to use to filter the data. Here are the fields:
`date/time`, `city`, `state`, `country` and `shape`.

 In the JS there is an event listener that checks when the input is changes and calls the **updateFilters** function to update the table.

### Result: How to use

* By default, the whole dataset is loaded:
<br/>

![nofilter.png](static/nofilter.png)

* We can use any field that is located on the left to filter, here is the filter search:
<br/>

![filter.png](static/filter.png)

* Here I enter `fl` in the state field to see how it is filterd by this state:
<br/>

![filter.png](static/filtered.png)

### Summary

* This web app allows the user to interact with a web page in a dynamical way, using code that runs in the client, without any server interaction.

* One drawback from this design is that if there is much information the page will be large. There should be pagination to avoid this. Another improvement that could be made is adding select elements when possible in the filter so the user don't have to type the whole field. In the date field, there could be a date pickup using a calendar. Also the possibility to select a range, like a year to see all UFO reporting from a given year.

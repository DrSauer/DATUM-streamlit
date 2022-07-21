# DATUM-streamlit

This app was created to visualize the data collected from tunnelling projects. It supplements the DATuM software developed in-house at Dr Sauer and partners.

## Input
The input of this app should be a .csv file with the following headings.

![](https://github.com/kenneth-yap/DATUM-streamlit/blob/main/table_headings.PNG)

It is important that all the headings have the exact same alphabets and capitalization. A few things to note:

* Please clean the data before uploading. If the chainage is unusually large the web app will have problems uploading the file and crash. This can be mitigated by removing start and end chainages with unusually large magnitude. The same applies to time. Overall, the columns that need to be cleaned are: (i) tunnel_meter_start, (ii) tunnel_meter_finish, (iii) time_start and (iv) time_stop.

* If the data is not cleaned properly, it will produce erronous results - garbage in, garbage out. 

* The code will automatically calculate the time taken and the chainages between the start and end point. You don't have to create a new column on excel for that.

* There is a 200 mb file limit.

## Filters
After inputting the data that needs to be analysed, filters are applied to obtain key insights of the data. The filters can be split into filters for the graph and filters for descriptions. 

**Filter for dashboard**
* On the right of the histogram, a legend of activities is provided to indicate the porportion of time spent at each location for respective activities. To visualize a specific activity, simply double click on the activity from the legend and it will segregate the data accordingly. To return to visualizing all the data, simply double click again and it will return to its default view.

**Filter for key insights**


## Output

The output of the app are the following:

* A plotly dashboard indicating the time allocated for each activity at each location.

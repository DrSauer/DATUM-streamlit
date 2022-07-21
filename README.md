# DATUM-streamlit

This app was created to visualize the data collected from tunnelling projects. It supplements the DATuM software developed in-house at Dr Sauer and partners.

## Input
The input of this app should be a .csv file with the following headings.

![](images/table_headings.png?raw=true)

It is important that all the headings have the exact same alphabets and capitalization. A few things to note:

* Please clean the data before uploading. If the chainage is unusually large the web app will have problems uploading the file and will crash. This can be mitigated by removing start and end chainages with unusually large magnitude. Overall, the columns that need to be cleaned are: (i) tunnel_meter_start, (ii) tunnel_meter_finish, (iii) time_start and (iv) time_stop

* The code will automatically calculate the time taken and the chainages between the start and end point. You don;t have to create a new column on excel for that.

## Output

The output of the 

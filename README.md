# Covid_19 ETL Project

Project Description

I discovered data from John Hopkins University that was compiled by data.data.org. I filtered the data for March 2020 and calculated the number of cases according to the number of confirmed cases, deaths, and recoveries.


Data Cleanup and Analysis


Transformation:

My transformation steps I needed to clean the data to be readable, presentable, and easy for me to query in the later stages. This was done by:

Developing a cleaning function in python that would select the data in the month of March 2020. This was applied to all datasets that I have.
All of the dates that have in the data sets we treated as values through the pd.melt function in Pandas.
Found a way of finding the daily increase with respect to each table. This value was converted from a float to an integer


Loading Part:

To store the data, I connected to a local PostgreSQL server on our desktop.
built three tables and a database.
We need to be able to access and query the data in our Jupyter Notebook, so I pushed  the Pandas DataFrame to the local PostgreSQL server.



Analysis :

SQL Queries I'm trying to determine:
Top 5 nations by number of most/least confirmed cases 
Top 5 nations by most/least number of deaths
Top 5 countries with the most/least recovered
Most confirmed/deaths/recovered dates in March

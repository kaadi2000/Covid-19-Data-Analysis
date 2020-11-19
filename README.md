# Covid-19-Data-Analysis

Covid – 19 Data Processing is a Program which can load, merge, clean and aggregate
the COVID-19 time series data. This program can give graphs and stats about any
country in the world. It is designed by using Python Language, Matplotlib, Seaborn, Alter,
Numpy and Pandas.

It takes the updated data from the web and show the current stats of Covid – 19 such as
Confirmed, Recovered, Death and Active cases around each country for which the user
requires. Further this program also compares data of newly confirmed cases between
multiple countries.

METHODS AND MATERIAL USED
3.1 MATERIAL USED
 Jupyter Notebook/ Google Colaboratory
3.2 METHODS
3.2.1 DESIGNING THE PROJECT
Confirmed, deaths and recovered are kept in different CSV files. That makes difficult for
plotting them in the same data visualization.
This COVID-19 Data processing runs the following steps:
1. Download raw CSV dataset from JHU CSSE public Github page.
2. Load raw CSV dataset and extract the common date list.
3. Merges the raw confirmed, deaths, and recovered CSV data into one DataFrame.
4. Performs data cleanings due to missing values, wrong datatypes and cases from
cruise ships.
5. Data Aggregation: Add an active case column Active, which is calculated
by active_case = confirmed — deaths — recovered. Aggregate data
into Country/Region wise and group them by Date and Country/Region. After that,
add day wise New cases, New deaths and New recovered by deducting the
corresponding cumulative data on the previous day. 

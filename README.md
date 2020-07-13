# SegmentingAndClusteringNeighborhoodsInToronto

**Introduction**
In this project I will explore, segment, and cluster the neighborhoods in the city of Toronto. The neighborhood data was not readily available on the internet.

For the Toronto neighborhood data, exists the following Wikipedia page: *https://en.wikipedia.org/wiki/List_of_postal_codes_of_Canada:_M*

Once the data is in a structured format, I can start the analysis to explore and cluster the neighborhoods in the city of Toronto. 
I will build the code to scrape the following Wikipedia page: *https://en.wikipedia.org/wiki/List_of_postal_codes_of_Canada:_M*, 
in order to obtain the data that is in the table of postal codes and to transform the data into a pandas dataframe.

The dataframe consists of three columns: PostalCode, Borough, and Neighborhood. I will only process the cells that have an assigned borough. 
I ignore cells with a borough that is Not assigned. More than one neighborhood could exist in one postal code area. 
For example, in the table on the Wikipedia page, you will notice that M5A is listed twice and has two neighborhoods: Harbourfront and Regent Park. 
These two rows were combined into one row with the neighborhoods separated with a comma. 
If a cell has a borough but a Not assigned neighborhood, then the neighborhood will be the same as the borough. 
So for the 9th cell in the table on the Wikipedia page, the value of the Borough and the Neighborhood columns will be Queen's Park.

There are different website scraping libraries and packages in Python. One of the most common packages is BeautifulSoup and I'm using it in this project. 
Package's main documentation page: *http://beautiful-soup-4.readthedocs.io/en/latest/*

The missing maps were added as images.

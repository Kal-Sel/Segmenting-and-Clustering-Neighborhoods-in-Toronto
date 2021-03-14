# SegmentingAndClusteringNeighborhoodsInToronto
 
In this project I was exploring, segmenting, and clustering the neighborhoods in the city of Toronto. The neighborhood data was not readily available on the internet.

For the Toronto neighborhood data, exists the following Wikipedia page: *https://en.wikipedia.org/wiki/List_of_postal_codes_of_Canada:_M*

Once the data was in a structured format, I started the analysis to explore and cluster the neighborhoods in the city of Toronto. 
I build the code to scrape the following Wikipedia page: *https://en.wikipedia.org/wiki/List_of_postal_codes_of_Canada:_M*, 
in order to obtain the data that is in the table of postal codes and to transform the data into a pandas dataframe.

The dataframe consists of three columns: PostalCode, Borough, and Neighborhood. I was only processing the cells that had an assigned borough. 
I ignored cells with a borough that were not assigned. More than one neighborhood could exist in one postal code area. 
For example, in the table on the Wikipedia page, you will notice that M5A is listed twice and has two neighborhoods: Harbourfront and Regent Park. 
These two rows were combined into one row with the neighborhoods separated with a comma. 
If a cell has a borough but a Not assigned neighborhood, then the neighborhood will be the same as the borough. 
So for the 9th cell in the table on the Wikipedia page, the value of the Borough and the Neighborhood columns will be Queen's Park.

There are different website scraping libraries and packages in Python. One of the most common packages is BeautifulSoup and I'm using it in this project. 
Package's main documentation page: *http://beautiful-soup-4.readthedocs.io/en/latest/*

The missing maps were added as images.

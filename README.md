# CustomSearch

The objective is to find all the occurences of the entity which is of the form(first name,last name,organisation,location) with the help of google search.

## Getting Started

1. The website is hosted on github pages. To open the tool, go to the following url(https://nehamotlani.github.io/CustomSearch/) or click [here](https://nehamotlani.github.io/CustomSearch/).
2. Enter the required details.
3. Click on search. A new window will open with the search results.
4. Note: The sample folder contains images of results for some of the queries.

## Explanation

1. The code is written in Javascript.
2. The index.html is the landing page. Once you enter the details, and click search the preProcess() function is called.
3. The preprocess function first forms a query from given input. The idea behind the query is to search whether the webpage has the phrase "firstname + lastname" or "lastname+firstname" as they should occur together at least once. We do the same thing for organisation and location and join them by OR query.
4. Once the query is created, the EntityResolution(Results) page is called and the query is passed as a parameter.
5. The EntityResolution(Results) page is created with the help of Custom Google Search API. The code for this page is generated from the guides which help display the results of the google search on the page. 

## Future Work

1. The webpage might contain only the first name or last name along with other details.
2. Providing a layer after the search results to filter. 

# data-sourcing-challenge

## Overview
This project aims to integrate data from two different sources: The New York Times (NYT) API and The Movie Database (TMDB) API. By retrieving movie reviews from NYT and movie details from TMDB, we can create a comprehensive dataset for analysis and further use.

## Project Structure:

### Part 1: Access the New York Times API:
* Construct the query URL to retrieve movie reviews.
* Perform GET requests to the NYT API to fetch movie reviews data.
* Extract relevant information such as title, keywords, and other metadata from the response.
* Convert the extracted data into a Pandas DataFrame for further processing.

### Part 2: Access The Movie Database API:
* Prepare the TMDB query URL to search for movie details.
* Iterate through the list of movie titles obtained from NYT reviews.
* Make GET requests to the TMDB API to retrieve detailed movie information based on the titles.
* Extract specific fields such as genres, languages, and production countries from the TMDB response.
* Create a DataFrame containing movie details merged from both NYT and TMDB sources.

### Part 3: Merge and Clean the Data for Export:
* Merge the NYT reviews DataFrame and TMDB details DataFrame based on the movie titles.
* Clean the merged DataFrame by removing duplicate rows and unnecessary columns.
* Convert certain columns containing lists into strings by removing list characters ([, ], ').
* Export the cleaned DataFrame to a CSV file for further analysis.

#### Dependencies:
* Python 3.x
* Pandas
* Requests
* Time

#### Usage:
1. Clone the repository to your local machine.
2. Install the required dependencies using pip install -r requirements.txt.
3. Run the Python script to execute the data integration process.
4. Check the generated CSV file for the merged and cleaned data.

#### Acknowledgments:
* The New York Times and The Movie Database for their APIs and data sources.
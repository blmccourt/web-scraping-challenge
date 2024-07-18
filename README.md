# web-scraping-challenge

## Background
We are now ready to take on a full web-scraping and data analysis project. We’ve learned to identify HTML elements on a page, identify their `id` and `class` attributes, and use this knowledge to extract information via both automated browsing with Splinter and HTML parsing with Beautiful Soup. We’ve also learned to scrape various types of information. These include HTML tables and recurring elements, like multiple news articles on a webpage.

## Part 1: Scrape Titles and Preview Text from Mars News
1. Use automated browsing to visit the [Mars news site](https://static.bc-edx.com/data/web/mars_news/index.html). Inspect the page to identify which elements to scrape.
2. Create a Beautiful Soup object and use it to extract text elements from the website.
3. Extract the titles and preview text of the news articles that you scraped. Store the scraping results in Python data structures as follows:
    - Store each title-and-preview pair in a Python dictionary and, give each dictionary two keys: `title` and `preview`. 
    - Store all the dictionaries in a Python list.
    - Print the list in your notebook.

## Part 2: Scrape and Analyze Mars Weather Data
1. Use automated browsing to visit the [Mars Temperature Data Site](https://static.bc-edx.com/data/web/mars_facts/temperature.html). Inspect the page to identify which elements to scrape.
2. Create a Beautiful Soup object and use it to scrape the data in the HTML table. 
3. Assemble the scraped data into a Pandas DataFrame.
4. Examine the data types that are currently associated with each column. Cast (or convert) the data to the appropriate datetime, int, or float data types.
5. Analyze your dataset by using Pandas functions to answer the following questions:
    - How many months exist on Mars?
    - How many Martian (and not Earth) days worth of data exist in the scraped dataset?
    - What are the coldest and the warmest months on Mars (at the location of Curiosity)? To answer this question:
        - Find the average minimum daily temperature for all of the months.
        - Plot the results as a bar chart.
    - Which months have the lowest and the highest atmospheric pressure on Mars? To answer this question:
        - Find the average daily atmospheric pressure of all the months.
        - Plot the results as a bar chart.
    - About how many terrestrial (Earth) days exist in a Martian year? To answer this question:
    - Consider how many days elapse on Earth in the time that Mars circles the Sun once.
    - Visually estimate the result by plotting the daily minimum temperature.
6. Export the DataFrame to a CSV file.

## Folders and Files
1. **[part_1_mars_news.ipynb](https://)**
   - A Jupyter notebook containing code that scrapes the Mars news titles and preview text.
2. **[part_2_mars_weather.ipynb](https://)**
   - A Jupyter notebook containing code that scrapes the Mars weather data and that cleans, visualizes, and analyzes that data.
3. **[weather_data.csv](https://)**
   - Export of dataframe to CSV file.
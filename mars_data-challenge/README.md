# Mars_Data-Challenge

As exploration of Mars continues, it is important to monitor the weather on the planet. In this challenge, we will showcase our web-scraping and data analytics skills by analyzing the weather data for Mars. To collect the data, we will scrape the [Mars News](https://static.bc-edx.com/data/web/mars_news/index.html) and [Mars Weather](https://static.bc-edx.com/data/web/mars_facts/temperature.html) using Python's Beautiful Soup library. We will extract the relevant information from the sites and store it in a pandas dataframe.


## Part 1: Scrape Titles and Preview Text From Mars News

In this section we will use part_1_mars_news.ipynb to utilize Splinter and Beautiful Soup to perform automated browsing. We will be able to inspect the source code from the webpage to identify which elements to scrape.

We will then extract titles and preview texts to store in seperate python dictionaries. Once dictionaries have been formed we will then loop through and store into a python list. 


## Part 2: Scrape and Analyze Mars Weather Data

In this section we will use part_2_mars_weather.ipynb to utilize Splinter and Beautiful Soup to perform automated browsing. We will be able to inspect the source code from the webpage to identify which elements to scrape. 

Once the data has been scraped we will then assemble into a Pandas DataFrame with the same column headers as the website data as shown below with a description.

- id: the identification number of a single transmission from the Curiosity rover

- terrestrial_date: the date on Earth

- sol: the number of elapsed sols (Martian days) since Curiosity landed on Mars
    
- ls: the solar longitude

- month: the Martian month

- min_temp: the minimum temperature, in Celsius, of a single Martian day (sol)

- pressure: The atmospheric pressure at Curiosity's location

Once a DataFrame has been successfully made we can then analyze the data to answer a series of questions

- How many months exist on Mars?
    1. There are 12 months on Mars.

- How many Martian (and not Earth) days worth of data exist in the scraped dataset?
    2.There are 1867 Martian days worth of data.

- What are the coldest and the warmest months on Mars (at the location of Curiosity)? To answer this question:

    - Find the average minimum daily temperature for all of the months.
        ![Alt text](Images/Avg%20low%20temp%20DF.png)

    - Plot the results as a bar chart.
        ![Alt text](Images/Avg%20Temp%20Per%20Month.png)
- Which months have the lowest and the highest atmospheric pressure on Mars? To answer this question:

    - Find the average daily atmospheric pressure of all the months.
        ![Alt text](Images/Avg%20press%20DF.png)

    - Plot the results as a bar chart.
        ![Alt text](Images/Avg%20Press%20Per%20Month.png)

- About how many terrestrial (Earth) days exist in a Martian year? To answer this question:

    - Consider how many days elapse on Earth in the time that Mars circles the Sun once.

    - Visually estimate the result by plotting the daily minimum temperature.

        1. There are 686 terrestrial days in a Martian year.
        ![Alt text](Images/Min%20Temp%20Per%20Day.png)


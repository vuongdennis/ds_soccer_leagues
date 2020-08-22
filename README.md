# Data Science Project about Soccer Leagues

### Introduction
In order to conduct this experiment, we used Jupyter Notebook as a tool to help us analyze and answer questions about Soccer League data. We used data from Laliga, MLS, Premier, Serie A, and Bundesliga soccer leagues. 

### Data Sets
* [Laliga](https://www.statbunker.com/competitions/PlayerStandings?comp_id=622)
* [MLS](https://www.statbunker.com/competitions/PlayerStandings?comp_id=632)
* [Premier](https://www.statbunker.com/competitions/PlayerStandings?comp_id=614)
* [Serie A](https://www.statbunker.com/competitions/PlayerStandings?comp_id=623)
* [Bundesliga](https://www.statbunker.com/competitions/PlayerStandings?comp_id=620)

With this data we wanted to figure out:
* If there was a correlation between goals scored and positioning for a specific league.
* If there was a correlation between goals scored and positioning for leagues overall.
* How often does each league scores compared to other leagues?

### Required Libraries
* Matplotlib
* Pandas
* Requests
* BeautifulSoup
* Numpy
* sklearn.linear_model

### How to run our code
You will need the required libraries alongside Jupyter Notebook. You would open up the file in the Github repository using Jupyter Notebook then use the run button to run the code. An alternative is to click on the file and Github will display a preview of what our code looks like on the Jupyter Notebook machine. If you have no intention of editing or making changes to our code, then looking at the display will show all of the data analysis.

# Web Scraper
For our web scraper, we used Beautifulsoup to scrape the data set websites. 

Extracted:
* Player Name
* Team
* Position
* Appearances
* Goals
* Assists
* Yellow 
* Yellow-Red
* League

Overall, we wanted to scrape each player's data from their name to how many goals they scored, receiving yellow cards, etc. All of the data for each player was located in a HTML table row and we had to look at the table data for each item we listed in the extracted.

# Teams Contribution
Dennis Vuong:
* Web scraped the MLS 2019 season data
* Web scraped LaLiga 2007 - 2018 season
* Created the Overall Dataframe for all the Leagues
* Performed EDA on which player scored the most in each league
* Performed EDA on total goals scored in each league
* LaLiga League linear regression

Edwin Leon:
* Web scraped LaLiga 2019 season data
* Web scraped Premier, Serie A, Bundesliga 2019 season data
* Cleaned the data to perform EDA
* Performed EDA on goals per position in each league
* Performed EDA on which position scores the most
* Lionel Messi linear regression 

# Analysis
Main question: Is there a correlation between the position of the players and scoring goals?

To answer this question we first analyzed each league individually. First we decided to see which playered scored the most in each league. After obtaining the name of the highest scoring players we analyzed them and saw that all of them were forwards. This gave us a hint that playing in the forward position will lead you to scorig more goals. Next, we analyzed the total goals per position in each league and the total number of players in each position. Given the data we saw that in all the leagues the forward position scored the most goals and that the number of players in the forward position was lower than any other position. This data gave us the feeling that there was a correlation between a players position and scoring goals. However, we decided to keep analyzing the data and decided to see which position scored the most goals in all 5 leagues combined. The results were ery clear, the forward position once again came out on top. To finish our analysis we decided to get the averge goals per position and saw how the forward position scores apreoximately an average of 4 goals per player. This led us to conclude that there is a correlation between a players position ans scoring goals.

Small questions: 

In the process of answering our main question we wanted to answer some small questions like, is it easier to score in one league than another? For this question we created a graph to see the total goals in each league and all of them were very similar to each other except for the MLS. In the MLS the players aproximately scored 1200 goals while in the other leagues they scored aproximately 1000 goals each. Just by looking at this data we can see that it is easier to score in the MLS however, it is important to note that the MLS is the only league outside of Europe in this data.



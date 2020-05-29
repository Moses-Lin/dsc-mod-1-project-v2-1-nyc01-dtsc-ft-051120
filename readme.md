# Movie Industry Case-Study.
Flatiron School Module 1 project
Moses Lin & Jean-Paul Ventura

# Project summary

Microsoft has just created a new movie studio and would like to know more about the industry to guide what movies they make and maximize potential earnings. We've have been called upon to provide some preliminary insights into the industry by analyzing and visualizing public data about the market.


# Insights. 

* How are domestic and worldwide profits correlated?
* How has the market profit tracked over the last decade?
* What are the top profitable movie genres over the last decade?
* What are the average or exprected budgets or production costs of the top profitable genres?

# Data Sources, Acquisition, Cleaning & Structuring

 Our project was completed with the use of the pandas, numpy, matplotlib and seaborn analytics and visualization python libraries. We used data from [The Movie Database(TMDb)](#https://www.themoviedb.org/?language=en-US) and tn... To clean the data we made sure to remove rows where 0 dollar values in their budget and gross fields were, as we would go on to visualize profits (gross/box office earnings - production costs). Also to compile a time array we had to structure the date data for films by isolating the YYYY from the complete MM/DD/YYYY date format, and then cast the entries as integers so that we could sort them and identify our time frames of interest when looking at domestic/worldwide profit for all movies in our dataset.

# Using API requests
The requests python library was used to make TMDB API calls to source information about the movie genres in order to visualize how profitability tracked with genre over the last decade.


# Results & Discussion

Considering whether it is a good time to enter the movie industry, to first order, requires an assessment of the general worldwide profits for the sample of movies found here. Although the information shown here may conceal finer dynamics related to production costs, looking at profits alone serves as a proxy for generalized interest over time in the mainstream film medium. The bar for 2019 shows a drop in interest by this metric and should serve as an area for future investigation.

![Mean Worldwide Profit for Movies over the last 10 years](#https://github.com/Moses-Lin/dsc-mod-1-project-v2-1-nyc01-dtsc-ft-051120/blob/master/Mean%20Worldwide%20Profit%20for%20Movies%20over%20the%20last%2010%20years.png)


We wanted to start off making sure there was a positive correlation between domestic vs global profits in order to frame an assumption that profits and therefor domestic market strategy could be expanded worldwide. Of course this would require further investiagation for detailing specific movie campaigns based on regional popularity or interest.

![Domestic vs global success of movies](#https://github.com/Moses-Lin/dsc-mod-1-project-v2-1-nyc01-dtsc-ft-051120/blob/master/Domestic%20vs%20Global%20success%20of%20Movies.png)

Taking a look at worldwide profit over the last 10 years by genre can broadly map what areas to focus on as Microsoft studios debuts on the market stage. We can see that science fiction proves to be the most profitable genre by far with adventure, romance and fantasy following.

![Top Profitable Movie Genres over the last 10 years](#https://github.com/Moses-Lin/dsc-mod-1-project-v2-1-nyc01-dtsc-ft-051120/blob/master/Top%20Profitable%20Movie%20Genres%20over%20the%20last%2010%20years.png)

Considering the profitability of Sci-Fi at about 800 million dollars over the last 10 years (based on this sample) and the subsequent 4 most profitable genres, lets take a look at what the production costs are in comparison to assess the relative production costs. We can see that the frequency behavior reflects that of the genre-specific profitability somewhat. This isnt unexpected for Sci-Fi movies typically require a lot of CGI which can be expensive.

![Expected Budget for Top 5 "safest" Profitable Genres](#https://github.com/Moses-Lin/dsc-mod-1-project-v2-1-nyc01-dtsc-ft-051120/blob/master/Expected%20Budget%20for%20Top%205%20%22safest%22%20Profitable%20Genres.png)


# Recommendations

- Based on our data, we do indeed recommend that Microsoft enter the film industry in the current year 2020.
- Focus on accomodating films such that they are available in as many regions as possible.
- Focus on investing in film genres with a high chance of profit, such as Science Fiction, Adventure, Romance, and Fantasy.
- Expect to invest about $350 million on average when producing Sci-Fi, and around $100 million on average when investing in Adventure, Romance, Fantasy, and other genres.


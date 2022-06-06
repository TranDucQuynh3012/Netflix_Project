# Netflix Shows Project:

![alt text](https://github.com/TranDucQuynh3012/Netflix_Project/blob/main/Netflix%20Show%20Visualization.png)

This is a project with an interesting topic: Netflix shows. 

*('Netflix is a streaming service that offers a wide variety of award-winning TV shows, movies, anime, documentaries, and more on thousands of internet-connected devices')*

The dataset I got here contains the information of the shows that aired on Netflix till 25/09/2021. With this dataset, the target is learning about the situation of the Netflix shows from the past to now by answering several questions which come to me when I look at this. I hope this project will give you a general view of Netflix shows and you could earn more knowledge about this famous video streaming platform.

You can go to this link to find out more details about this dataset:
https://www.kaggle.com/datasets/shivamb/netflix-shows

The main tool I used for this Project is JupyterNotebook and the language is Python.
For a better version of JupyterNotebook which shows the Plotly charts, please go to this link below:
https://nbviewer.org/github/TranDucQuynh3012/Netflix_Project/blob/main/Netflix_Shows_%20Project.ipynb

To run this Notebook on your personal computer, please download & install JupyterNotebook by Anaconda:
https://www.anaconda.com/products/distribution

I also use Power BI to show important visualizations on a dashboard, to sum up what we did in this project, which is the one you saw at the top of this description.

I. Libraries used in this Project:
1. Numpy: working with data in array type.
2. Pandas: working with data in Series and Data Frame type.
3. Matplotlib, Seaborn, Plotly: create data visualizations.
4. WordCloud: create a plot for text data.

II. Dataset: 'netflix_titles.csv'

III. Code:

* Notebook: https://github.com/TranDucQuynh3012/Netflix_Project/blob/main/Netflix_Shows_%20Project.ipynb

* or (to show Plotly chart): https://nbviewer.org/github/TranDucQuynh3012/Netflix_Project/blob/main/Netflix_Shows_%20Project.ipynb

III. Target:  Understand what are the shows on Netflix. Finding out how they have changed throughout the years. We will know who the main target customers of Netflix are and how their entertainment habits are.

IV. Pre-processing the data:

The initial dataset was not ready for analysing so I have to do these cleaning works:

- Finding out the number of missing values.
- Determine which columns are unnecessary, or risky and delete them.
- Filling missing values with proper filling-values.
- Change the type of columns that have the wrong type.


V. Analysing the Netflix data:

After all the cleaning steps, now the data is ready for processing, and now it's time for us to ask questions about this dataset. Each answer for each question will help us understand more and more about the Netflix shows. So let's begin!

**1. What are the types of shows aired on Netflix?:** To answer this we will focus on the 'type' columns. This column will let us know there are two types of shows: Movies and TV Shows. And these charts below let us know how many shows they have:

barchart

piechart

*From the two charts above, we can see Movies type has larger shows than TV Shows. It occupies nearly 70% of the total. The point is Netflix is well known for being a great Movie streaming service. However, 30% of the shows air on this service are TV Shows. That means TV shows have been playing an important role in American life.*

barchart

 *Netflix started to add more shows from 2015 and they focus on increasing the number of movies more than TV Shows. But the percentage of TV Shows remains stable at 30%. In 2020, both numbers of Movies and TV Shows added to Netflix decreased slightly, the reason might be the adversely affecting of Covid-19. The data we have only have information of Netflix shows till 25/09/2021, not the whole year, so in the bar chart above, the figure for 2021 does not reflect the situation of Netflix shows precisely.*

**2. Which country provided the most shows on Netflix?:** Showing data of 'country' column by a bar chart and we'll get the answer. This is what it looks like:

[barchart]

*It is obvious that the USA is top 1 here among the countries in producing shows. We still get India, the United Kingdom, Japan... in the top list but the USA stands on the top with an outstanding number of shows added to Netflix. The reason we may have known is the USA is one of the countries which has the biggest film industry in the world. The quality of the movies or TV shows they made is great. The other reason is Netflix is an American company and the audiences are American mostly, so they prefer adding the shows provided by their country.

**3. How long are the durations of the shows? And how have they changed throughout the years?:** We can divide the shows on Netflix into 2 types: the series shows (which have 1 or more seasons) and the non-series shows (end in 1 episode) because the units of their durations are different. We will look at each type separately:

[distplot]

*The distribution of durations of non-series shows is following Normal distribution with the mean value is 99.5 min. Most non-series shows have a duration of around 100 min, that is the proper duration for a non-series show because people usually have 2-3 hours per day for entertainment. If the show is too long, they might have consider to watching another one which is shorter, or if they were really interested in that show, they might have to watch it in 2 days or more. In the future, this distribution of duration may change based on how much time people have to spend on watching online shows.*

[barchart]

*Most series shows only have 1 season. The shows which have 9 seasons and above are very few. The audiences might don't have too much time to spend on TV shows with a lot of seasons, or making a show like that will cost too much for the producer. The audiences start to follow a series show because the first season of it is really attractive, but if the next seasons become worse, they might don't want to watch the other season anymore, and the fame of the producer would be affected. So it is risky to make more seasons of a show.*

**4.What is the most rating of the shows on Netflix?**: The rating or content rating rates the suitability of a show to its audiences, such as TV-MA is the rating that shows that a program is intended for adults, TV-PG program contains material that parents may find unsuitable for younger children... This is the total ratings of shows on Netflix and we can see which one is on top:

[barchart]

*TV-MA (shows for adults), TV-14 (unsuitable for children under the age of 14) are the most ratings of shows on Netflix. It is easy to understand because Netflix requires a monthly fee to use their service, so the target clients should be adults, who can pay that charge. Because of that, you need to take a look at your children if they want to watch a show on Netflix.*

[linechart]

*The numbers of the shows rated 'TV-MA' and 'TV-14' are increasing, just like the increase of the number of total shows. The increase of 'TV-MA' rating is stronger than 'TV-14'. This ensures us that Netflix has been and will be focusing on serving adult customers.*

**5. How duration of the non-series shows have changed?:** With this question, we'll dig a little bit deeper in the non-series shows field. We already knew that the mean value of durations of non-series shows is nearly 100 min. But have it stayed stable at 100 min through all the years? Let's take a look at this chart below:

[linechart]

*What we can see from this chart is the durations of the non-series shows have extended longer, from 83 min in 2015 to 103 min in 2021. But the extension became slow since 2018 and we can predict that 100-110 min is the maximum mean value of duration for non-series shows in the future. We’ll need more data in the future to ensure this.*

**6. The number of the shows by released year:** We'll find out whether Netflix prefers choosing shows released from which years to add to their platform.

[linechart]

[barchart]

*From those charts above we can see that most of Movies and TV Shows aired on Netflix had been released since 2000 and the number of them has been increasing rapidly. The shows released before 2000 are very few because they are not suitable for the audiences of the 21st century. In the line chart of TV Shows, we can see a downtrend happening after 2020, that's because the data in 2021 are not completed right now so we have nothing to worry about it. But in the Movies chart, the downtrend happened during 2019 - 2020, this might be the effect of Covid-19 this time causing the number of movies produced in the world to decrease.*

**7.Take a little look at the most used words for Shows' Titles and Descriptions:** Here we can see how producers choose the words for their shows' titles and descriptions. We'll need the Wordcloud library to do this:

[chart1]

[chart2]

This is all information I need about Netflix shows for now. After all, I showed some of them (which I assumed are the most important) on a dashboard by Power BI, which you can see on the top of this description.

My Netflix shows project description ends here. You can see if the more questions we ask, the more insights we can obtain from this dataset. I hope you enjoy it and may this project could help you a little bit with your research or learning.


*Have a nice day!*

*Tran Duc Quynh*

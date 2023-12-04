# STAT-184-Final-Project.github.io
---
title: STAT 184 Final Project

Authors: Kaitlyn Klumb, Xinyi Bao, Samuel Quinn

date: 2023/12/6

---

**Background Information:**  
The primary dataset offers an avenue to analyze and gain valuable insights from the luminaries of the platform, including comprehensive details on top creators' subscriber counts, video views, upload frequency, country of origin, earnings, and more.   
The primary dataset come from [here](https://www.kaggle.com/datasets/nelgiriyewithana/global-youtube-statistics-2023)

***Research Question:*** where are Youtuber channels most popular in the world, and does their internet speed play a role? 

***Our Hypothesis:*** Internet speed may play a significant role in making the YouTube channels popular in the world.

***Challenge Encountered:***
* Conflicts with GitHub Desktop to collaborate on the code 
* We did our work on our local laptops, edited the main code on GitHub, and committed the changes. 
* Increase our efficiency


<br>


**Data Access:**
```{r}
head(GlobalYouTube)
head(GlobalInternet2019)
```
![GlobalYouTube](/1.png)
![GlobalInternet2019](/2.png)

**Data Wrangling:**


Ranking the popularity of countries, based on the amount of views they recieve. The highest number is the most popular. 
![Rank the popularity of countries](/3.png)

Ranking the internet speed of countries, the highest number is the highest speed. 
![Rank the internet speed of countries](/4.png)


Joining the data tables by the country's video views and internet speed 

![join the countries' video views and internet speed](/5.png)



# Wrangling, E
![Wangling Global Internet 2019](/6.png)

# Wrangling, C
![Narrow Table](/7.png)

**Data EDA:**

EDA for the primary dataset:

![EDA for 1st dataset](/8.png)

EDA for the secondary dataset:

![EDA for 2nd dataset](/9.png)


**Machine Learning**

The clustering and visualization of YouTube channels created between 2010 and 2023 with subscribers above the average value

![Clustering](/10.png)


**Data Visualization:**

Visualize World Map with INternet Speed

![Colered World Map](/11.png)

Visualize YouTube channels created between 2010 and 2023 based on their latitude and longitude

![Geographical Distribution between 2010 and 2023](/12.png)


Visualize Country Speed
![Country Speed](/13.png)


***Key Visualization:***

World Map:

![Gray World Map](/18.png)

Overlay the top 5 countries with the fastest internet speeds from the GlobalInternet2019 dataset onto your world map

![World Map with Top 5 Internet Speed](/14.png)


Combine the visualization of the top 5 countries with the fastest internet speeds with the locations of YouTube channels created between 2010 and 2023

![World Map with Top 5 Internet Speed and Youtubers](/15.png)


Compare the Youtube Views count and subscribers:

![Comparisons between Views and Subscribers](/16.png)



**Linear Regression:**

To figure out the statistical relationship between the number of Global Youtubers' subscribers and the Global Internet Speed, we decided to make a linear regression model to explain.

![Linear Regression Summary](/17.png)


***Analysis:***

The p-value for the Internet speed coefficient is 0.136, which is above common levels of significance, indicating that the effect of Internet speed on the number of YouTube subscribers is not statistically significant.

R-squared = 0.004814. This indicates that the Internet speed in the model explains a very low proportion (less than 0.5%) of the variation in the number of YouTube subscribers. In other words, the variation in the number of YouTube subscribers can hardly be explained by Internet speed.

Based on the results of this model, we can conclude that, there is no significant linear relationship between Internet speed and the number of YouTube subscribers. This may be due to the fact that subscriber numbers are influenced by a variety of factors that are not included in the current model.



**Conclusion:**

To answer the first question: Where are Youtuber channels most popular in the world

"United States" "Spain" "Germany" "France"  

For the second question: There is no significant linear relationship between Internet speed and the number of YouTube subscribers.


 

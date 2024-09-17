# Who is the best goalkeeper of the 2023/24 season from the top 5 leagues?

Following the Yashin trophy nominees for the best goalkeeper of the season, in this project, I will determine the top goalkeepers of the 2023/24 season from the top 5 football leagues, through data scrapped from the fbref.com . Using python and It's libraries available, let's explore the data and create a chart to show the goalkeepers that stoodout, for good and for bad.

#### Note

This study will include only the top 5 european leagues, England, Spain, Italy, Germany and France. Meaning that other leagues, national cups, continental tournaments, and international friendlies and tournaments will not be accounted. 

## Introduction

Using the links below, I was able to retrieve all the information I needed to create this notebook.
1st link: https://fbref.com/en/comps/Big5/2023-2024/keepers/players/2023-2024-Big-5-European-Leagues-Stats
2nd link: https://fbref.com/en/comps/Big5/2023-2024/keepersadv/players/2023-2024-Big-5-European-Leagues-Stats

The fbref.com site is free and has a good amount of data that can be used to create the analysis.
The first link will lead to standard goalkeeper stats, and the second link has advanced stats like PSxG and other data that I will not use.
Initially, I will restructure the tables, rename columns, delete columns, clean registers with NaN and merge the two tables.

![alt text](https://github.com/adonisdario/data-science/blob/main/best-gk-2023-24/images/1.png?raw=true)

### Note #2

Matz Sels is the only goalkeeper that played for two clubs in a season, Nottingham Forest and Strasbourg.

## Standards

For a goalkeeper to be considered top, It has to fulfill the following criterion: 

- Played at least 42% of the league season games;
> *16 games for the Premier League, La Liga or Serie A which have 20 teams for a total of 38 rounds or 14 games at Bundesliga or Ligue 1 which have 18 teams for a total of 34 rounds.*

- Have high % of saves;
> *The Save % is the number of balls saved devided by total of Shots On Target Against. Higher Save % means that the goalkeeper is saving a lot of the shots he is facing.*

- Have a high PSxG +/- for every 100 xG;

> *PSxG is a metric that tells the chance of the goal to be scored after the shot was taken, considering the position of the ball, the position of the defenders and the position of the goalkeeper, including penalties kicks.*

> *PSxG +/- is the difference between the sum of the PSxG from all the shots faced and the total goals allowed (GA, not including Own Goals). Positive PSxG +/- means that the goalkeeper avoided a lot of high chance goals. Negative means that the goalkeeper is conceding more low chance goals.*

> Finally, for this metric, we want to determine how many goals can a goalkeeper avoid when facing 100 expected goals.

- Observe the quantity of Saves/90;

> *This metric is going to show the weakness of the defensive linemen. If it's too high, means that the defensive linemen allowed a high volume of shots per game for the goalkeeper to save.*

## Chart

The scatterplot is built by the Save% v PSxG +/- for 100xG. The size of the points means the Save/90. The 'hotter' the collor more 90s the keepers have played. If a goalkeeper is at the top right of the chart, they are the best, and if it's at the bottom left of the chart, they are the worst.

## Top



## Worst



## Outliers


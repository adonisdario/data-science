# Who is the best goalkeeper of the 2023/24 season from the top 5 leagues?

Following the Yashin trophy nominees for the best goalkeeper of the season, in this project, I will determine the top goalkeepers of the 2023/24 season from the top 5 football leagues, through data scrapped from the fbref.com . Using python and It's libraries available, let's explore the data and create a chart to show the goalkeepers that stoodout, for good and for bad.

#### Note

This study will include only the top 5 european leagues, England, Spain, Italy, Germany and France. Meaning that other leagues, national cups, continental tournaments, and international friendlies and tournaments will not be accounted. 

## Introduction

Using the links below, I was able to retrieve all the information I needed to create this notebook.
https://fbref.com/en/comps/Big5/2023-2024/keepers/players/2023-2024-Big-5-European-Leagues-Stats
https://fbref.com/en/comps/Big5/2023-2024/keepersadv/players/2023-2024-Big-5-European-Leagues-Stats
The fbref.com site is free and has a good amount of data that can be used to create the analysis.
The first link will lead to standard goalkeeper stats, and the second link has advanced stats like PSxG and other data that I will not use.
Initially, I will restructure the tables, rename columns, delete columns, clean registers with NaN and merge the two tables.

## Note #2

Matz Sels is the only goalkeeper that played for two clubs in a season, Nottingham Forest and Strasbourg.

## Standards



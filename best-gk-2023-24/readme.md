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

![alt text](https://github.com/adonisdario/data-science/blob/main/best-gk-2023-24/images/0.png?raw=true)

### Note #2

Matz Sels is the only goalkeeper that played for two clubs in a season, Nottingham Forest and Strasbourg.

## Standards

For a goalkeeper to be considered top, It has to fulfill the following criteria: 

- Played at least 42% of the league season games;
> *16 games for the Premier League, La Liga or Serie A which have 20 teams for a total of 38 rounds or 14 games at Bundesliga or Ligue 1 which have 18 teams for a total of 34 rounds.*

- Have high % of saves;
> *The Save % is the number of balls saved devided by total of Shots On Target Against. Higher Save % means that the goalkeeper is saving a lot of the shots he is facing.*

- Have a high PSxG +/- for every 100 xG;

> *PSxG is a metric that tells the chance of the goal to be scored after the shot was taken, considering the position of the ball, the position of the defenders and the position of the goalkeeper, including penalties kicks.*

> *PSxG +/- is the difference between the sum of the PSxG from all the shots faced and the total goals allowed (GA, not including Own Goals). Positive PSxG +/- means that the goalkeeper avoided a lot of high chance goals. Negative means that the goalkeeper is conceding more low chance goals.*

> Finally, for this metric, we want to determine how many goals can a goalkeeper avoid when facing 100 expected goals.

- Consider the quantity of SoTA/90 and Saves/90;

> *This metrics are going to show the weakness of the defensive linemen. High number of Shots on Target Against /90 and a high number of Saves /90 means that the defence is weak and the goalkeeper is outstanding. The contrary means that the defence is good but the goalkeeper is failing.*

### Rejected metrics

Goals conceded and Clean sheets were discarded because these metrics are for the entire defensive system, not only for the goalkeeper.

## Chart

The scatterplot is built by the Save% v PSxG +/- for 100xG. The size of the points means the Save/90. The 'hotter' the collor means more 90s the keepers have played. If a goalkeeper is at the top right of the chart, they are the best, and if it's at the bottom left of the chart, they are the worst.
The Save% mean is 70.8%, and the PSxG +/- for 100xG mean is -1.69. The red line is the trendline of the chart.

![alt text](https://github.com/adonisdario/data-science/blob/main/best-gk-2023-24/images/1.png?raw=true)

## Top Goalkeepers

![alt text](https://github.com/adonisdario/data-science/blob/main/best-gk-2023-24/images/2.png?raw=true)

> Donnarumma, Sommer, Di Gregorio and Samba appears at the top 10 list of both Save% and Goals Avoided. And by looking at the chart, they appear over the trendline;

### Top Goalkeeper Analysis

Note: PSxG +/- for 100xG = Goals Avoided

- **G. Donnarumma:**
  -   GK: 1st in Save% (84.5%) 🔝 | 1st in Goals Avoided (+34.0) 🔝 | 16th in Saves/90 (3.7) | 71% of 90s played 
  - Team: 64th in SoTA/90 (4.6) | 39th in PSxG/90 (1.3)
    > *Only played 71% of available matches due to the coach's choice;*
    
    > *His team conceded a **high** amount of Shots on target with low value chances in average.*
- **Y. Sommer:**
  -   GK: 2nd in Save% (82.7%) | 2nd in Goals Avoided (+25.5) | 90th in Saves/90 (2.3) | 90% of 90s played 
  - Team: 3rd in SoTA/90 (2.9) | 2nd in PSxG/90 (0.8)
    > *His team conceded very few Shots on target with very low value chances in average.*
- **M. Di Gregorio:**
  -   GK: 4th in Save% (79.9%) | 4th in Goals Avoided (+22.9) | 13th in Saves/90 (3.8) | 84% of 90s played 
  - Team: 77th in SoTA/90 (5.0) | 58th in PSxG/90 (1.4)
    > *Missed some games due to injury;*
  
    > *His team conceded a **high** amount of Shots on target with regular value chances in average.*
- **B. Samba:**
  -   GK: 5th in Save% (78.7%) | 7th in Goals Avoided (+19.2) | 48th in Saves/90 (3.1) | 97% of 90s played
  - Team: 37th in SoTA/90 (4.1) | 44th in PSxG/90 (1.3)
    > *His team conceded a low amount of Shots on target with regular value chances in average.*

### Conclusion

**G. Donnarumma** stood out as the best goalkeeper from the top5 leagues. His defence was worse than Y. Sommer's, meaning, he had to work harder to achieve the top standards.

------

## Worst Goalkeepers

![alt text](https://github.com/adonisdario/data-science/blob/main/best-gk-2023-24/images/3.png?raw=true)

- **M. Sels (Strasbourg / N. Forest):**
  -   GK: 98th in Save% (60.2%) | 99th in Goals Avoided (-27.7) | 95th in Saves/90 (2.2) | 98% of 90s played
  - Team: 14th in SoTA/90 (3.5) | 21st in PSxG/90 (1.1)
    > *His team conceded few Shots on target and most of the high value ones were Avoided;*

- **Sam Johnstone:**
  -   GK: 96th in Save% (62.7%) | 100th in Goals Avoided (-30.0) | 98th in Saves/90 (2.1) | 53% of 90s played
  - Team: 11th in SoTA/90 (3.4) | 11th in PSxG/90 (1.0)
    > *Missed almost half the season due to injury;*
    
    > *His team conceded **very few** Shots on target with **very low** value chances. Still, he was bottom 4 of Save% and bottom 2 of Goals Avoided.*    

- **Alaa Bellaarouch:**
  -   GK: 92nd in Save% (63.5%) | 98th in Goals Avoided (-26.3) | 82nd in Saves/90 (2.5) | 44% of 90s played
  - Team: 44th in SoTA/90 (4.2) | 46th in PSxG/90 (1.3)
    > *Was 3rd choice goalkeeper for most of the season;*
       
    > *His team conceded low amount of Shots on target with low value chances. Still, he was bottom 9 of Save% and bottom 3 of Goals Avoided;* 

- **Andrea Consigli:**
  -   GK: 98th in Save% (61.6%) | 97th in Goals Avoided (-25.7) | 73rd in Saves/90 (2.7) | 92% of 90s played
  - Team: 62nd in SoTA/90 (4.5) | 67th in PSxG/90 (1.5)
    > *His team conceded few Shots on target and most of the high value ones were Avoided;* 

## Outliers


---
title: "Ratings"
date: 2023-04-28
weight: 10
description: >
  How ratings are calculated on LG
---

A standard Elo rating system is used to calculate the ratings. It is a method that was used for the first time in chess. A detailed description is at https://en.wikipedia.org/wiki/Elo_rating_system

For the implementation on the Little Golem server, an initial rating of 1500 is used. The K factor is determined by the number of games played. For the first game this coefficient is equal to 60 and after each game the coefficient decreases by 1. The minimum coefficient of K is 30, after that it does not decrease anymore. The rating cannot fall below 1000. The rating is calculated to four decimal places (one decimal place is displayed). The rating change in each completed game is displayed next to the player's rating. 

Ratings go up and down and do not have a permanent value like grandmaster titles have in chess - https://en.wikipedia.org/wiki/Grandmaster_(chess) .Therefore, ranks are also introduced on LG, taken from the game Go. More at https://en.wikipedia.org/wiki/Dan_(rank)

Rank starts at 20.kyu and for when the conditions are met so a higher rank is obtained. 1st kyu is followed by 1st dan. The rank is gained **forever** and never drops again. 

The prerequisite for the 19th kyu is to have a rating of 1200 and to have won 1 game. For 18th kyu is to get another 50 rating points (1250) and win 2 more games (ted total at least 3). So it goes on. For example, the condition for getting 1st Dan is to have a rating of 2200 and to have won at least 210 games. 

There is a button on the bottom right of the game page that allows you to toggle between rating and rank display. The toggle applies to all LG server pages. It's not necessary though, as the **tooltip** on the rating works at the same time. 

The rating is calculated separately for each game and variant.

## Table

Summary table of conditions for obtaining the rank.

| Rank  | Rating  | Number of winning games  |  
|:---:|:---:|---:|
 | 19k | 1250 | 1 | 
 | 18k | 1300 | 3 | 
 | 17k | 1350 | 6 | 
 | 16k | 1400 | 10 | 
 | 15k | 1450 | 15 | 
 | 14k | 1500 | 21 | 
 | 13k | 1550 | 28 | 
 | 12k | 1600 | 36 | 
 | 11k | 1650 | 45 | 
 | 10k | 1700 | 55 | 
 | 9k | 1750 | 66 | 
 | 8k | 1800 | 78 | 
 | 7k | 1850 | 91 | 
 | 6k | 1900 | 105 | 
 | 5k | 1950 | 120 | 
 | 4k | 2000 | 136 | 
 | 3k | 2050 | 153 | 
 | 2k | 2100 | 171 | 
 | 1k | 2150 | 190 | 
 | 1d | 2200 | 210 | 
 | 2d | 2250 | 231 | 
 | 3d | 2300 | 253 | 
 | 4d | 2350 | 276 | 
 | 5d | 2400 | 300 | 
 | 6d | 2450 | 325 | 
 | 7d | 2500 | 351 | 
 | 8d | 2550 | 378 | 
 | 9d | 2600 | 406 | 
 | 10d | 2650 | 435 | 
 | 13d | 2800 | 528 | 
 | 11d | 2700 | 465 | 
 | 12d | 2750 | 496 | 
| 13d | 2800 | 528 | 

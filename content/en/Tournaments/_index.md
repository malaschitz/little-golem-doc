
---
title: "Tournaments"
linkTitle: "Tournaments"
weight: 8
description: >
  Tournament description
lastmod: 2026-10-30
---

Little Golem runs tournaments for every game:

* Championship
* Mini Cup
* Ladder
* User tournaments

Players can also use the Waiting Room for rated casual games.

[Time control](/time/) is used in all tournaments.

## Championship

The championship is the main type of tournament on LG.
Players are divided into groups in each league.
There is only one group in the first league.
In the second league there are two groups.
In the third league there are four groups, and so on.
The championship is played as a double round-robin.

The winner of the first league is the champion.

The **top two** players in each group advance to the next higher league. 
Players finishing as low as **fifth** stay in their current league.

A new championship starts for each variant twice a year. The [calendar](calendar/) lists the start dates for each variant.


## Mini Cup

A Basic Round tournament starts as soon as three players have registered.
Each group is played as a double round-robin.
Players scoring more than **50% of the possible points will advance to the next level**. 

The same process continues at each level.
A player can play any number of tournaments. 
If a player advances to a level where they have already secured promotion, they will only play in one tournament at that level. 
However, if a tournament has already started at that level, the player has earned the additional right to play at that level.


## Ladder 

Each game has an ongoing ladder tournament.
Players are ranked in a list.
Players may challenge opponents up to CEIL(SQRT(position)) places above them.
Example:

| Position | CEIL(SQRT(position)) | Can challenge |
|----------|----------------------|---------------|
|    1     |          -           |       -       |
|    2     |          2           |       1       |
|    3     |          2           |      1-2      |
|    4     |          2           |      2-3      |
|    5     |          3           |      2-4      |
|    6     |          3           |      3-5      |
|    7     |          3           |      4-6      |
|    8     |          3           |      5-7      |
|    9     |          3           |      6-8      |
|    10    |          4           |      6-9      |

If the challenger wins the game, the challenger overtakes the opponent.
Each player can challenge at most one player and defend against at most two players at the same time.
A new ladder game with the same opponent is possible only 21 days after their previous game.
The game starts immediately when the player registers for the tournament.
Games are started automatically.
Players always challenge the player in the highest available position.

## Waiting Room

The Waiting Room is used for rated casual games. A game starts when another player accepts the open request.

## User tournaments

Players can create their own round-robin tournaments.

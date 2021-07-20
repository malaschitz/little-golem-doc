
---
title: "Tournaments"
linkTitle: "Tournaments"
weight: 8
description: >
  Tournament description
---

On *LittleGolem* are played tournaments for every game:

* Championship
* Monthly Cup
* Ladder
* User tournaments

There exists Waitting Room and is possible to invite to play some player.

## Championship

The championship is more or less the main type of tournament. 
The players are divided into groups in leagues. In the first league there is one group, in the second league there are two groups, and so on. 
Every player plays against every other player.
The first two players from each group in the lower league advance to the higher league.
Players up to fifth place stay in the same league.

When all games in all groups are completed, a new championship will be started on the 1st of the month.
The minimum number of players to start the championship is 20.

## Monthly Cup

The tournament starts immediately when 5 players are logged in. 
Each player plays against every other player.
The winners of all groups started during the month will play in the following month's tournament.
The winners of all monthly cups during the year play in the following year's tournament.

## Ladder 

For each game there is a running tournament. 
The players are lined up in a list.
Players challenge the player in the higher position, up to CEIL (SQRT (position)).
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
|    10    |          4           |      6-10     |

If the challenger wins the game, he overtakes his opponent. 
Players challenge a maximum of 1 player and defend against 2 players.
A new game with the same opponent is possible only after 14 days after the common game.
The game starts immediately when the player registers for the tournament.
The games are started automatically. 
Players always challenge the player in the highest available position.

## Waiting Room

Simple waiting room for playing rated games.

## User tournaments

Players can create their own round robin tournaments.

## Invite players

The player can invite another player to a game.

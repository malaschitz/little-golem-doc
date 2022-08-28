
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

[Time control](http://localhost:1313/time/) is used in all tournaments.

## Championship

The championship is the main type of tournament on LG.
Players are divided into groups in each league.
There is only one group in the first league.
In the second league there are two groups.
In the third four, etc.

The winner in the first league is the champion.

The top two players in each group advance to the next higher league. 
Players up to fifth stay playing in their league. 

A new championship starts for each variant once a year. 
There is a start date for each variant. 
Exceptions are championships where more than 30 players are entered. 
These start on the first day of the month following the end of the previous championship.

### Calendar

This is the calendar of when each variant starts if the number of registered players is less than 30.

#### January 1st
     Draughts - Dameo
     Go - Size 37x37
     WYPS - Italian 14
     WYPS - Japanese 8
     WYPS - Dutch 8
     Hex - Size 19
     Reversi - Size 6x6
     EinStein würfelt nicht! - 3-points match
     EinStein würfelt nicht! - Backwards capture
     Morelli - Size 9

#### February 1st
     WYPS - Slovak 5
     WYPS - Slovak 14
     WYPS - Russian 8
     QYPS - Size 5
     Twixt PP - Size 24
     Four in a row - Size 6x7
     Four in a row - Size 10x10
     Lines of Action - Scramble
     Lines of Action - Quick
     Lines of Action - Black Hole
     EinStein würfelt nicht! - 1-point game
     Havannah - Size 10
     Tumbleweed - Size 8

#### March 1st
     Go - Random100
     WYPS - English 14
     WYPS - English 5
     WYPS - Polish 8
     OSKI - French
     OSKI - Spanish
     Hex - Size 13
     Golem Word Game - 100 letters
     EinStein würfelt nicht! - 11-points match
     Slither - Size 13

#### April 1st
     Shogi - Shogi 5x6
     Shogi - Shogi 5x6 PLUS
     WYPS - Italian 8
     WYPS - Czech 8
     Polyomino - mini
     OSKI - Greek
     Twixt PP - Size 48

#### May 1st
     Draughts - English Draughts/Checkers
     Shogi - Shogi
     WYPS - German 14
     WYPS - Slovak 8
     QYPS - Size 8
     OSKI - Dutch
     Hex - Size 11
     Amazons - Cross
     StreetSoccer - Street Soccer
     Havannah - Size 4

#### June 1st
     Go - Toroidal Go
     Shogi - Mini Shogi
     WYPS - English 8
     LYNGK - Stack6
     Gomoku - Gomoku Pro 9x9
     Dots and Boxes - Size 4x4
     Lines of Action - Size 8x8
     EinStein würfelt nicht! - 5-points match
     EinStein würfelt nicht! - 50-points match
     Havannah - Size 5
     Morelli - Size 11

#### July 1st
     ConHex - ConHex
     Go - Size 13x13
     Polyomino - penta
     Twixt PP - Size 30
     Breakthrough - Size 8
     Havannah - Size 6

#### August 1st
     Draughts - International Draughts
     Go - Hahn Pointing System
     Chess - Chess
     WYPS - German 8
     WYPS - French 14
     WYPS - Spanish 14
     WYPS - Russian 11
     Polyomino - small
     OSKI - Italian
     Reversi - Size 10x10
     Amazons - Size 10
     Dots and Boxes - Size 6x6
     EinStein würfelt nicht! - 7-points match
     Havannah - Size 7
     Slither - Size 9
     Catchup - Random
     Morelli - Size 13
     Morelli - Size 31
     Tumbleweed - Size 11

#### September 1st
     WYPS - Greek 14
     Polyomino - hexa
     OSKI - Slovak
     Hex - Size 15
     Four in a row - Size 8x8
     Gomoku - Gomoku Pro
     Gomoku - Gomoku
     Dots and Boxes - Size 7x7
     EinStein würfelt nicht! - Black hole
     Havannah - Size 8 

#### October 1st
     Go - Size 19x19
     WYPS - Japanese 14
     WYPS - Dutch 14
     OSKI - English
     Reversi - Size 12x12
     Connect6 - Connect6
     Havannah - Size 9
     Tumbleweed - Size 4

#### November 1st
     XiangQi - XiangQi
     Shogi - Tori Shogi
     WYPS - French 8
     WYPS - Spanish 8
     WYPS - Slovak 11
     WYPS - Russian 5
     WYPS - Russian 14
     WYPS - Numeric small
     Reversi - Size 8x8
     DVONN - DVONN
     Four in a row - Size 9x9
     EinStein würfelt nicht! - 19-points match
     Catchup - Size 7

#### December 1st
     Go - Size 9x9
     Go - Size 27x27
     Chess - Chess960
     Shogi - Shogi 3x4
     WYPS - English 11
     WYPS - Polish 14
     WYPS - Greek 8
     WYPS - Numeric
     OSKI - German
     TZAAR - Random
     Dots and Boxes - Size 5x5
     Catchup - Size 5
     Tumbleweed - Size 6

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
|    10    |          4           |      6-9      |

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
